---
title: 更新 embeddedSIMActivationCodePool
description: 更新嵌入式SIMActivationCodePool 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6d0f85a3a0348d8a6ec3b89fb3b0e5712135e00
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020635"
---
# <a name="update-embeddedsimactivationcodepool"></a>更新 embeddedSIMActivationCodePool

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新嵌入式 [SIMActivationCodePool 对象](../resources/intune-esim-embeddedsimactivationcodepool.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象的 JSON 表示形式。

下表显示创建 [embeddedSIMActivationCodePool 时所需的属性](../resources/intune-esim-embeddedsimactivationcodepool.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入式 SIM 卡激活代码池的唯一标识符。 创建时分配的系统生成值。|
|displayName|String|管理员定义的嵌入式 SIM 卡激活代码池的名称。|
|createdDateTime|DateTimeOffset|嵌入式 SIM 卡激活代码池的创建时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入式 SIM 卡激活代码池的时间。 更新的服务器端。|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) 集合|属于此池的激活代码。 此导航属性用于将激活代码张贴到 Intune，但不能用于从 Intune 读取激活代码。|
|activationCodeCount|Int32|属于此池的激活代码总数。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```



