## Ahhh, the core of the onion. Thankfully, NENT handles all the heavy-lifting with regard to routing so you aren't left weeping!

Below is the actual code used in the root of the app to create this route:

```
<n-views>...
  <n-view path="/route-start"
    page-title="Route"
    content-src="/pages/deep-routes/route-start.html">
      <n-view path="/child"
        page-title="Child Route"
        content-src="/pages/deep-routes/route-child.html">
          <n-view path="/deep"
            page-title="Deep Route"
            content-src="/pages/deep-routes/route-deep.html">
          </n-view>
      </n-view>
  </n-view>
...</n-views>  
```