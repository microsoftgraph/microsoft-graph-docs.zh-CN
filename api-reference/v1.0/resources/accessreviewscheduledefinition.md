---
title: accessReviewScheduleDefinition 资源类型
description: 表示 Azure AD 访问评审的计划。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9e2ee2d4296855d7f8fdf5ccd5a46252d7a3a7c70bdff83199c6aed51a7667e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121422"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>accessReviewScheduleDefinition 资源类型

命名空间：microsoft.graph

表示 Azure AD 访问评审 [的计划](accessreviewsv2-root.md)。

accessReviewScheduleDefinition 包含 [accessReviewInstance 对象](accessreviewinstance.md) 的列表。 每次重复执行计划定义时，将创建一个实例。 实例还表示要审阅的每个唯一资源。 如果计划定义审阅多个资源，则每个资源在每个重复周期中都有一个唯一实例。 对于一次评审，每个资源只创建一个实例。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 accessReviewScheduleDefinition。 结果中不包括关联的 accessReviewInstance 对象。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取具有指定 id 的 accessReviewScheduleDefinition。 结果中不包括关联的 accessReviewInstance 对象。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除具有指定 id 的 accessReviewScheduleDefinition。  |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定的 id 更新 accessReviewScheduleDefinition **的属性**。 |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|检索调用用户作为一个或多个实例的审阅者的所有定义。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| id | String | 访问评审的功能分配的唯一标识符。 支持 `$select`。 只读。|
| displayName | String   | 访问评审系列的名称。 支持 `$select` 和 `$orderBy`。 创建时为必需项。 |
| createdDateTime  |DateTimeOffset  | 创建访问评审系列时时间戳。 支持 `$select` 和 `$orderBy`。 只读。 |
| lastModifiedDateTime | DateTimeOffset   | 上次修改访问评审系列的时间戳。 支持 `$select`。 只读。|
| status  |String   | 此只读字段指定访问评审的状态。 典型状态包括 `Initializing` `NotStarted` `Starting` `InProgress` 、、、、、、 `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。  <br>仅 `$select` `$orderby` 支持 、 (`$filter` 和 `eq`) 。 只读。 |
| descriptionForAdmins  |string  |  评价创建者提供的用于向管理员提供评论的更多上下文的说明。 支持 `$select`。 |
| descriptionForReviewers |string | 审阅创建者提供的说明，用于向审阅者提供审阅的更多上下文。 审阅者将在发送给他们请求审阅的电子邮件中看到此说明。 支持 `$select`。 |
| createdBy  |[userIdentity](../resources/useridentity.md)  | 创建此评价的用户。 只读。 |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  | 定义要审阅的资源的范围。 有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 创建时为必需项。 仅 `$select` 支持 `$filter` (`contains` 和) 。 有关配置作用域的选项示例，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | 将审阅范围确定为来宾用户跨所有组的访问权限，并确定Microsoft 365组时Microsoft 365此属性。 每个组将成为访问评审系列 **的唯一 accessReviewInstance。**  有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。 支持 `$select`。 有关配置 instanceEnumerationScope 的选项示例，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置，请参阅下面的类型定义。 支持 `$select`。 创建时为必需项。 |
| reviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者。 只有在将单个用户分配为审阅者时，审阅者属性才可更新。 创建时为必需项。 支持 `$select`。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者[分配给你的访问Graph定义](/graph/accessreviews-reviewers-concept)。 |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。 替换 **backupReviewers**。 支持 `$select`。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
| instances|[accessReviewInstance](accessreviewinstance.md) 集合 | 如果 **accessReviewScheduleDefinition** 是定期访问评审，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示 **accessReviewScheduleDefinition 中正在审阅的每个唯一资源**。 如果审阅具有多个资源和多个实例，则每个资源将具有每个重复周期的唯一实例。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
