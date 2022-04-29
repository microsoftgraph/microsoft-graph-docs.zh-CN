---
title: 列出用户的 cloudPC
description: 列出归属于已登录用户的 cloudPC 设备。
author: andrewku0409
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6d2e1427cf94c80c61426f15df7256c9ad917661
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126337"
---
# <a name="list-cloudpcs-for-user"></a>列出用户的 cloudPC
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出归属于已登录用户的 [cloudPC](../resources/cloudpc.md) 设备。 

>[!NOTE]
>此操作仅返回以下属性： **id**、 **displayName**、 **imageDisplayName**、 **servicePlanId**、 **servicePlanName**、 **servicePlanType**、 **status**、 **lastModifiedDateTime**、 **aadDeviceId**、 **statusDetails**、 **gracePeriodEndDateTime**。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.Read.All、CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/cloudPCs
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数，以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [cloudPC](../resources/cloudpc.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_cloudpc"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/cloudPCs
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "aadDeviceId": "f5ff445f-7488-40f8-8ab9-ee784a9c1f33",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Demo-1",
      "imageDisplayName": "Windows-10 19h1-evd",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "servicePlanType": "enterprise",
      "status": "provisioned",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null,
      "gracePeriodEndDateTime": "2020-11-010T20:00:34Z"
    }
  ]
}
```
