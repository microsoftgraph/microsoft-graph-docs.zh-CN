---
title: 获取 cloudPcOrganizationSettings
description: 读取 cloudPcOrganizationSettings 对象的属性和关系。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 51f7cceeeaaaf04eadc657af0dfa1b029cc79fb3
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804225"
---
# <a name="get-cloudpcorganizationsettings"></a>获取 cloudPcOrganizationSettings
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从当前租户中读取 [cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) 的属性和关系。 租户只有一个 **cloudPcOrganizationSettings** 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.Read.All、CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.Read.All、CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/organizationSettings
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 OData `$select` 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_cloudpcorganizationsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/organizationSettings
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOrganizationSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
    "id": "8660bf17-bf17-8660-17bf-608617bfffff",
    "userAccountType": "standardUser",
    "osVersion": "windows11"
  }
}
```
