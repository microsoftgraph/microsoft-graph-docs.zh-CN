---
title: '显示 Microsoft Graph Toolkit组件从右到左 (rtl) '
description: 介绍 Microsoft (组件) 从右到左Graph Toolkit rtl Graph Toolkit支持。
ms.localizationpriority: medium
author: vogtn
ms.openlocfilehash: a573016903f68883dc733e596de2519640a6acac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129570"
---
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a>显示 Microsoft Graph Toolkit组件从右到左 (rtl) 

Microsoft Graph Toolkit 组件支持从右向左语言脚本的双向标记。

若要更改页面上所有组件的方向，请设置 document 或 tag 上的 属性 `dir` `html` `body` ， `rtl` 如以下示例所示。

```html
<body dir="rtl"></body>
```

或

```html
<html dir="rtl"></html>
```

![从右向左](../images/rightToLeft.png)
