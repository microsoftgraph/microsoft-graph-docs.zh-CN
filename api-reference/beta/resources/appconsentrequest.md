---
title: appConsentRequest 资源类型
description: 一个代表特定应用程序的 userConsentRequest 对象集合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9c01fd4e752bca0fe9518553f52312e523da3a3
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697899"
---
# <a name="appconsentrequest-resource-type"></a>appConsentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定应用程序的 [userConsentRequest](../resources/userconsentrequest.md) 对象的集合。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 appConsentRequests](../api/appconsentrequest-list.md)|[appConsentRequest](../resources/appconsentrequest.md) 集合|检索 [appConsentRequest](appconsentrequest.md) 对象及其属性的集合。|
|[获取 appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。|
|[filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性，当前用户是这些对象的审阅者，并且用户同意请求的状态为 `InProgress` 。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appDisplayName|String|请求显示名称的应用的一部分。 必填。 仅 `$filter` (和 `eq` `$orderby`) 。 |
|appId|String|应用程序的标识符。 必填。 仅 `$filter` (和 `eq` `$orderby`) 。 |
|consentType|String|请求的同意类型。 可能的值是： `Static`   和  `Dynamic` 。 它们分别表示在同意工作流中请求的静态和动态权限。 仅 `$filter` (和 `eq` `$orderby`) 。 必需。|
|id|String|应用同意请求的标识符。 必填。|
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
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

