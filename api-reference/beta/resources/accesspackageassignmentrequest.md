---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6be3fa431a2216ef8b31b673a5f73ef6067fff9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939199"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。 如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合 | 检索 accesspackageassignmentrequest 对象的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 accessPackageAssignmentRequest。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 accessPackageAssignmentRequest 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|请求的处理结束日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|id|字符串| 只读。|
|isValidationOnly|Boolean|如果请求不处理工作分配，则为 True。|
|合理化|字符串|请求者提供的理由。|
|requestState|字符串|、 `Denied` `Delivered`、中`PartiallyDelivered`的一个。 只读。|
|requestStatus|字符串|有关请求处理状态的详细信息。 只读。|
|requestType|字符串|一个`UserAdd`或`UserRemove`。 只读。|


## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|请求程序|[accessPackageSubject](accesspackagesubject.md)| 分配了请求的主题或分配了直接分配的主题。 此为只读属性。 可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
 
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
