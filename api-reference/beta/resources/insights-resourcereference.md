---
title: resourceReference 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8ab2a79d66db6a45ecf3df748cf8f5740721ef80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874324"
---
# <a name="resourcereference-resource-type"></a>resourceReference 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含属性的[见解](insights.md)复杂类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>属性

| 属性      | 类型      | Description  |
| ------------- |-----------| -------------|
| WebUrl        | String    | 通向引用的项的 URL。 |
| id            | 字符串    | 项目的唯一标识符。           |
| type          | 字符串    | 一个 string 值，可以用于分类项目，如"microsoft.graph.driveItem" |
