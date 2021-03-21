---
title: appConsentRequest 资源类型
description: 表示特定应用程序的 userConsentRequests 聚合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f823f64d4c0324aeca74c3268d6fc95d313e2f00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965115"
---
# <a name="appconsentrequest-resource-type"></a>appConsentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定应用程序的 [userConsentRequests](../resources/userconsentrequest.md) 聚合。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 appConsentRequests](../api/appconsentrequest-list.md)|[appConsentRequest](../resources/appconsentrequest.md) 集合|获取 [appConsentRequest](../resources/appconsentrequest.md) 对象及其属性的列表。|
|[获取 appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。|
|[列出 appConsentRequests：filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|当前用户是审阅者的 [appConsentRequests](../resources/appconsentrequest.md) 的列表|

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

