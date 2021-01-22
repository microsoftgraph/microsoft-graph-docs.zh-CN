---
title: accessPackageResourceRequest 资源类型
description: 访问包资源请求是请求将资源添加到目录，以便资源的角色可在目录的一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ddddea13ceb2840c61ec31238c03e7ab6e43d2d4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934801"
---
# <a name="accesspackageresourcerequest-resource-type"></a>accessPackageResourceRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD](entitlementmanagement-root.md)权利管理中，访问包资源请求是请求将资源添加到目录，以便资源的角色可在目录的一个或多个访问包中使用，或者从访问包不再需要的目录中删除资源。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [accessPackageResourceRequest](accesspackageresourcerequest.md) 集合 | 检索 **accessPackageResourceRequest 对象** 的列表。 |
| [创建 accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | 创建新的 **accessPackageResourceRequest** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|catalogId|String|访问包目录的唯一 ID。|
|expirationDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String| 只读。|
|isValidationOnly|Boolean|如果设置，则不添加资源。|
|justification|String|请求者添加或删除资源的理由。|
|requestState|String| 服务能否将资源添加到目录的结果。  该值是 `Delivered` 添加或删除资源。 只读。|
|requestStatus|String|只读。|
|requestType|String|用于 `AdminAdd` 添加资源（如果调用方是管理员或资源所有者） `AdminRemove` 或删除资源。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| 可为 Null。|
|requestor|[accessPackageSubject](accesspackagesubject.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


