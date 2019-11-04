---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定使用者可以通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: acb7c7b355d2a03d78cad1127882f272135fc4a2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939206"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>accessPackageAssignmentPolicy 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配策略指定了主题可以通过访问包分配请求或分配访问包的策略。 访问包可以有零个或多个策略。 收到来自接受者的请求时，主题将与每个策略相匹配，以查找该主题的策略（如果有）。 然后，该策略将确定请求是否需要审批以及访问包分配的持续时间。

若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合 | 检索 accessPackageAssignmentPolicy 对象的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 创建新的 accessPackageAssignmentPolicy 对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取 accessPackageAssignmentPolicy 对象的属性和关系。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除 accessPackageAssignmentPolicy。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackageId|字符串|访问包的 ID。|
|canExtend|Boolean|指示用户是否可以在批准后扩展访问包分配的持续时间。|
|createdBy|字符串|只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|description|String|策略的说明。|
|displayName|String|策略的显示名称。|
|durationInDays|Int32|此策略中的工作分配在过期之前持续的天数。|
|expirationDateTime|DateTimeOffset|在此策略中创建的工作分配的到期日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|字符串| 只读。|
|isEnabled|Boolean|可以将此策略用于新的请求。|
|modifiedBy|字符串|只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| 具有此策略的访问包。 此为只读属性。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "isEnabled": false,
    "canExtend": false,
    "durationInDays": 365
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
