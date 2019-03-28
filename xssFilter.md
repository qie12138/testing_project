#### 参考文献:   

[1] https://github.com/markdown-it/markdown-it/blob/master/test/fixtures/markdown-it/xss.txt   

[2] http://louiszhai.github.io/2016/03/05/xss/

#### 刷新历史

| 时间 | 说明 | 更新人 |
| ---- | ---- | ------ |
|2019-03-28 | 首次刷新 | ZHD |

---

## Blockquote
> hello <a name="n"
> href="javascript:alert('xss')">*you*</a>

## Html element event

<div style="padding: 20px; opacity: 0;height: 20px;" onmouseout="alert('Gotcha!')">1</div>

![XSS Img]("onerror="alert('XSS'))

![XSS Img](https://www.example.com/image.png"onload="alert('XSS'))

## Script 
<script>alert('gotcha');</script>

[normal link](javascript)

<p><a href="javascript">normal link</a></p>

## Should not allow some protocols in links and images

[xss link](javascript:alert(1))

[xss link](JAVASCRIPT:alert(1))

[xss link](vbscript:alert(1))

[xss link](VBSCRIPT:alert(1))

[xss link](file:///123)

[xss link](&#34;&#62;&#60;script&#62;alert&#40;&#34;xss&#34;&#41;&#60;/script&#62;)

[xss link](&#74;avascript:alert(1))

[xss link](&#x26;#74;avascript:alert(1))

[xss link](\&#74;avascript:alert(1))

[xss link](<javascript:alert(1)>)

[xss link](javascript&#x3A;alert(1))

## <p> tag link
<p>[xss link](javascript:alert(1))</p>

<p>[xss link](JAVASCRIPT:alert(1))</p>

<p>[xss link](vbscript:alert(1))</p>

<p>[xss link](VBSCRIPT:alert(1))</p>

<p>[xss link](file:///123)</p>

<p><a href="%22%3E%3Cscript%3Ealert(%22xss%22)%3C/script%3E">xss link</a></p>

<p>[xss link](Javascript:alert(1))</p>

<p><a href="&amp;#74;avascript:alert(1)">xss link</a></p>

<p><a href="&amp;#74;avascript:alert(1)">xss link</a></p>

<p>[xss link](&lt;javascript:alert(1)&gt;)</p>

<p>[xss link](javascript:alert(1))</p>

## Should not allow data-uri except some whitelisted mimes

![](data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7)

<p><img src="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" alt=""></p>

[xss link](data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4K)

<p>[xss link](data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4K)</p>

[normal link](/javascript:link)

<p><a href="/javascript:link">normal link</a></p>

## Image parser use the same code base as link.

![xss link](javascript:alert(1))

<p>![xss link](javascript:alert(1))</p>

## Autolinks

<javascript&#x3A;alert(1)>

<javascript:alert(1)>

<p>&lt;javascript:alert(1)&gt;</p>

<p>&lt;javascript:alert(1)&gt;</p>

## Linkifier

javascript&#x3A;alert(1)

javascript:alert(1)

<p>javascript:alert(1)</p>

<p>javascript:alert(1)</p>

## References

[test]: javascript:alert(1)

<p>[test]: javascript:alert(1)</p>

## Make sure we decode entities before split:

```js&#32;custom-class
test1
```

```js&#x0C;custom-class
test2
```

<pre><code class="js">test1
</code></pre>
<pre><code class="js">test2
</code></pre>

