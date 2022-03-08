---
title: resourceData 资源类型
description: 表示附加到发送给订阅者更改通知的数据源。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: c8cb63331cdd2252f40eef8be468499832bca9d6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333643"
---
# <a name="resourcedata-resource-type"></a>resourceData 资源类型

命名空间：microsoft.graph

表示附加到发送给订阅者更改通知的资源数据。 此资源是一个开放类型，允许传入其他属性。

有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无，Outlook **resourceData** 包含以下字段的资源除外：

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| @odata.type | String | Microsoft Graph 中描述所表示对象的 OData 实体类型。 |
| @odata.id | String | 对象的 OData 标识符。 |
| @odata.etag | String | 表示对象版本的 HTTP 实体标记。 |
| id | String | 对象的标识符。 |

> **注意：****resourceData** 中提供的 id **值** 在生成更改通知时有效。 某些操作（如将邮件 `id` 移动到另一个文件夹）可能会导致处理更改通知时不再有效。

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "@odata.type",
    "@odata.id",
    "@odata.etag",
    "id"
  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "@odata.type": "#microsoft.graph.resourceData"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

