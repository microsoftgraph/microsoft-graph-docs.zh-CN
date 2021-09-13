---
title: 在 OneNote 页中创建绝对定位的元素
description: OneNote 页正文可以包含多个能在页面上独立定位的直接 `div`、`img` 和 `object` 子元素。
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 391ac7a7ed49f6b4eff22824ba649ae37eddd9c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019074"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a>在 OneNote 页中创建绝对定位元素

OneNote 页面的正文可以包含多个直接 `div`、`img` 和 `object` 子元素，可在页面上对其独立定位。

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a>属性和定位行为

使用 `data-absolute-enabled` 和 [`style`](#supported-css-style-attributes) 属性在页面上创建绝对定位的元素，如下所示：

- 正文元素必须指定 `data-absolute-enabled="true"`。 如果省略或设置为 `false`，则所有正文内容在 API 创建的 `_default` 绝对定位 div 内呈现，所有位置设置将被忽略。

- 只有 `div`、`img` 和 `object` 元素才能是绝对定位的元素。 

- 绝对定位的元素必须指定 `style="position:absolute"`。

- 绝对定位的元素必须是 `body` 元素的直接子级。 不是绝对定位的 `div`、`img` 或 `object` 元素正文的任何直接子级都将被呈现为绝对定位 `_default` div 内的静态内容。

- 绝对定位元素位于其指定的顶部和左侧坐标，与页面左上角（在标题区域上方）的 0:0 起始位置相关。

- 如果绝对定位的元素省略了顶部或左侧坐标，则缺少的坐标将被设置为其默认值：`top:120px` 或 `left:48px`。 这些默认坐标指定标题区域正下方的位置。 请注意，省略坐标可能会导致元素彼此相互堆叠。

- 绝对定位元素无法进行嵌套或无法包含定位的元素。 API 忽略在绝对定位的 div 中嵌套元素上指定的任何位置设置，在绝对定位的父 div 中呈现此嵌套内容，并在响应中返回 **api.diagnostics** 属性中的警告。


### <a name="example"></a>示例

下面的示例包含直接 `p` 子级、绝对定位的 div 和非绝对定位的 div。

#### <a name="input-html"></a>输入 HTML  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

API 在默认 div 中呈现非绝对定位 div。请注意，嵌套的 `<div>` 标记遭放弃，因为它们不定义任何语义信息（如 `data-id`）。

#### <a name="output-html"></a>输出 HTML 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a>示例

以下示例创建包含一个绝对定位的 div 和一个绝对定位的图像的页面。


#### <a name="input-html"></a>输入 HTML  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
OneNote API 评估输入 HTML 并保留所有语义内容和受 OneNote 支持的任何结构信息。 呈现结果页面，如以下图像所示（但不呈现 div 和图像的可见边框）。 

![含有绝对定位的 div 和图像的结果页面](images/abs-pos.png)

请注意，对来自输入 HTML 的非贡献嵌套 div 所做的更改。 API 保留 div 的内容，但丢弃 `<div>` 标记，因为 div 无法定义语义信息（如 `data-id`）。

有关 OneNote API 如何处理输入和输出 HTML 的详细信息，请参阅 [OneNote 页面的输入和输出 HTML](onenote-input-output-html.md)。

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a>受支持的 CSS 样式属性

所有绝对定位的元素都可以指定顶部和左侧位置。 div 和图像可以指定宽度，并且图像还可以指定高度。 例如：

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| 属性 | 支持的元素 | 说明 |  
|:------|:------|:------|  
| top | div, img, object | 仅以像素为单位的元素顶部边框的 y 轴坐标。 默认值为 120 个像素。<br/><br/>示例：`top:140px` |  
| left |  div, img, object  | 仅以像素为单位的元素左边框的 x 轴坐标。 默认值为 48 个像素。<br/><br/>示例：`left:95px` |  
| width |  div, img  | 仅以像素为单位的元素的宽度。<br/><br/>示例：`width:480px` |  
| height | img | 仅以像素为单位的元素的高度。 对于 div，高度是在运行时计算的，且任何指定的高度值都将被忽略。<br/><br/>示例：`height:665px` |  
 
其他位置属性（如 `z-index`）都将被忽略。 绝对定位的图像可以使用 `data-render-src` 或 `src` 属性。


<a name="request-response-info"></a>

## <a name="response-information"></a>响应信息

OneNote API 在响应中返回以下信息。

| 响应数据 | 说明 |  
|:------|:------|  
| 成功代码 | 成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。 |  
| 错误 | 请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。 |  
  


<a name="permissions"></a>

## <a name="permissions"></a>权限

若要创建或更新 OneNote 页面，需要请求相应的权限。 选择应用运行所需的最低级别的权限。

#### <a name="permissions-for-post-pages"></a>POST 页面的权限 

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  


#### <a name="permissions-for-patch-pages"></a>PATCH 页面的权限 

- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md#notes-permissions)。


<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [创建 OneNote 页](onenote-create-page.md)
- [更新 OneNote 页内容](onenote-update-page.md)
- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)
