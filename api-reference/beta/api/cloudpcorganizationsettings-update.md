---
title: 更新 cloudPcOrganizationSettings
description: 更新 cloudPcOrganizationSettings 对象的属性。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c051f3dd21e2e6e8ad7071ee0a2980b66d1313fe
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072786"
---
# <a name="update-cloudpcorganizationsettings"></a>更新 cloudPcOrganizationSettings
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新租户 [中 cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) 对象的属性。

## <a name="permissions"></a>Permissions
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
PATCH /deviceManagement/virtualEndpoint/cloudPcOrganizationSettings
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|osVersion|cloudPcOperatingSystem|操作系统版本 (操作系统) 在云 PC 上预配。 可能的值包括 `windows10`、`windows11`、`unknownFutureValue`。 可选。|
|userAccountType|cloudPcUserAccountType|已预配云 PC 上的用户的帐户类型。 可能的值包括 `standardUser`、`administrator`、`unknownFutureValue`。 可选。|


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_cloudpcorganizationsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/organizationSettings
Content-Type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
  "userAccountType": "standardUser",
  "osVersion": "windows11"
}
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
