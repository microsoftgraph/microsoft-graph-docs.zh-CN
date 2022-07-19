---
title: 获取 operationalInsightsConnection
description: 读取 operationalInsightsConnection 对象的属性和关系。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: bd9eadd6e960043c5035e1a6d4dd6bbccc03a0b7
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856545"
---
# <a name="get-operationalinsightsconnection"></a>获取 operationalInsightsConnection
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [operationalInsightsConnection 对象的](../resources/windowsupdates-operationalinsightsconnection.md) 属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|WindowsUpdates.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/resourceConnections/{operationalInsightsConnectionId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "get_operationalinsightsconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/resourceConnections/fbb71b85-4173-0bf6-d2bc-ee7921b80cb0
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
    "id": "fbb71b85-4173-0bf6-d2bc-ee7921b80cb0",
    "state": "connected",
    "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
    "azureResourceGroupName": "target-resource-group",
    "workspaceName": "my-workspace"
  }
}
```

