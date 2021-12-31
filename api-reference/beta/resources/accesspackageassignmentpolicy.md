---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定主题可以通过访问包分配请求或分配访问包的策略。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9045cc88e5e68fd49e85b8333c035cabba2bc5b9
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651258"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>accessPackageAssignmentPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD](entitlementmanagement-overview.md)中，访问包分配策略指定主题可以通过访问包分配请求或分配访问包的策略。 访问包可以具有零个或多个策略。 收到主题的请求时，主题将针对每个策略进行匹配，以查找包含该主题 (如果) requestorSettings 包含该主题的策略。 然后，该策略确定请求是否需要审批、访问包分配的持续时间以及分配是否需要定期检查。

若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合 | 检索 accessPackageAssignmentPolicy 对象的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 创建新的 accessPackageAssignmentPolicy 对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取 accessPackageAssignmentPolicy 对象的属性和关系。 |
| [更新 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 更新 accessPackageAssignmentPolicy 对象的属性。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除 accessPackageAssignmentPolicy。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageId|String|访问包的标识符。|
|accessReviewSettings|[assignmentReviewSettings](assignmentreviewsettings.md)|Who必须检查此策略中访问包的分配以及分配时间。 如果不需要审阅，则此属性为 null。|
|canExtend|Boolean|指示用户是否可以在审批后延长访问包分配持续时间。|
|createdBy|String|只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|说明|String|策略的说明。|
|displayName|String|策略显示名称。 支持 `$filter`（`eq`）。|
|durationInDays|Int32|此策略中的分配在到期之前持续等待的天数。|
|expirationDateTime|DateTimeOffset|在此策略中创建的工作分配的到期日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String| 只读。|
|modifiedBy|String|只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Who必须批准此策略中的访问包请求。|
|requestorSettings|[requestorSettings](requestorsettings.md)|Who从此策略请求此访问包。|
|问题|[accessPackageQuestion](accesspackagequestion.md) 集合|向请求者提出问题。|


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| 具有此策略的访问包。 只读。 可为 NULL。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
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

