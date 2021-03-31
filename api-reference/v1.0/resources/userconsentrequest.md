---
title: userConsentRequest 资源类型
description: 用户创建以使用需要访问组织数据的应用的请求，用户未经授权向自身授予同意。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9aab98b448333412b8982fc80e68702e4255f66b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469547"
---
# <a name="userconsentrequest-resource-type"></a>userConsentRequest 资源类型

命名空间：microsoft.graph

[userConsentRequest](../resources/userconsentrequest.md)是由用户请求访问需要管理员授权才能访问的应用程序时创建的。 

## <a name="methods"></a>方法

方法|返回类型|说明|
|:---|:---|:---|
|[列出 userConsentRequests](../api/userconsentrequest-list.md)|[userConsentRequest](../resources/userconsentrequest.md) 集合|获取 [userConsentRequest](../resources/userconsentrequest.md) 对象及其属性的列表。|
|[获取 userConsentRequest](../api/userconsentrequest-get.md)|[userConsentRequest](../resources/userconsentrequest.md)|读取 [userConsentRequest](../resources/userconsentrequest.md) 对象的属性和关系。|
|[列出 userConsentRequests：filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md)|[userConsentRequest](../resources/userconsentrequest.md) 集合|获取 [userConsentRequest](../resources/userconsentrequest.md) 对象及其属性的列表。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|approvalId|String|审批的 ID。 此值等于 的值 `id` 。|
|completedDateTime|DateTimeOffset|将请求状态 **标记为** 的日期和时间 `Completed` 。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|createdBy|[identitySet](../resources/identityset.md)|创建请求的用户。|
|createdDateTime|DateTimeOffset|创建请求的日期和时间。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br>仅 `$filter` (和 `eq` `$orderby`) 。|
|customData|String|自由文本字段，用于定义用户同意请求的任何自定义数据。 未使用。|
|id|String|请求的标识符。 |
|reason|String|用户要求访问应用的理由。 仅 `$filter` (和 `eq` `$orderby`) 。  |
|状态|String|用户的应用同意请求的状态。 可能的值是 `Initializing` ：、 `InProgress` 和 `Completed` 。 仅 `$filter` (和 `eq` `$orderby`) 。 |

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|审批|[审批](../resources/approval.md)|与请求相关的审批决策。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```
