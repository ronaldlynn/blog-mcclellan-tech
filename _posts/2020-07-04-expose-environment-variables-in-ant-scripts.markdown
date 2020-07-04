---
layout: post
title:  "Expose Environment Variables in Ant Scripts"
date:   2020-07-04 14:02:18 -0400
categories: java "build tools"
---
### Add Environment Variable awareness to Ant `build.xml`:

```xml
<property environment="env" />
```

### Use Environment Variables in Ant tasks:

```xml
<target name="echo.env">
  <echo message="HOME environment variable: ${env.HOME}" />
  <echo message="PATH environment variable: ${env.PATH}" />
</target>
```