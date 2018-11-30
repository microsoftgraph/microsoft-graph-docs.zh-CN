---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045789"
---
# <a name="contenttypeinfo-resource-type"></a>ContentTypeInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**contentTypeInfo** 资源指示项的 SharePoint 内容类型。

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentTypeInfo** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | 内容类型的 ID。
| **name**       | string  | 内容类型的名称。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
