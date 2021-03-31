---
title: appConsentRequest 资源类型
description: 表示特定应用程序的 userConsentRequests 聚合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac7e9f2ea8e727a285016641bac10ea3d2e38f9b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469534"
---
# <a name="appconsentrequest-resource-type"></a>appConsentRequest 资源类型

命名空间：microsoft.graph

特定应用程序的 [userConsentRequests](../resources/userconsentrequest.md) 聚合。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 appConsentRequests](../api/appconsentrequest-list.md)|[appConsentRequest](../resources/appconsentrequest.md) 集合|获取 [appConsentRequest](../resources/appconsentrequest.md) 对象及其属性的列表。|
|[获取 appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。|
|[appConsentRequests：filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|当前用户是审阅者的 [appConsentRequests](../resources/appconsentrequest.md) 的列表|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|appDisplayName|String|请求显示名称的应用的一部分。 必需。 仅 `$filter` (和 `eq` `$orderby`) 。 |
|appId|String|应用程序的标识符。 必需。 仅 `$filter` (和 `eq` `$orderby`) 。 |
|id|String|应用同意请求的标识符。 必需。|
|pendingScopes|[appConsentRequestScope](../resources/appconsentrequestscope.md) 集合|等待审批的挂起范围列表。 如果 consentType 为 ，则为空 `Static` 。 必填。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|userConsentRequests|[userConsentRequest](../resources/userconsentrequest.md) 集合|挂起的用户同意请求列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
