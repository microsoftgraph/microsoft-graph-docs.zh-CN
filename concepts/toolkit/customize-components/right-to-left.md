---
title: '显示 Microsoft Graph Toolkit组件从右到左 (rtl) '
description: 介绍 Microsoft (组件) 从右到左Graph Toolkit rtl Graph Toolkit支持。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 189ffe24f42b2302d0992bcc5ca63c9cd7ff6934
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589222"
---
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a>显示 Microsoft Graph Toolkit组件从右到左 (rtl) 

Microsoft Graph Toolkit 组件支持从右向左语言脚本的双向标记。

若要更改页面上所有组件 `dir` 的方向，请设置 document `html` `body` 或 tag 上的 属性， `rtl`如以下示例所示。

```html
<body dir="rtl"></body>
```

或者

```html
<html dir="rtl"></html>
```

![从右向左](../images/rightToLeft.png)
