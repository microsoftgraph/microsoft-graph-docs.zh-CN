---
title: 更新 sideLoadingKey
description: 更新 sideLoadingKey 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72d620984f7d6d3e69c04339cae8ada43740e133
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59070025"
---
# <a name="update-sideloadingkey"></a>更新 sideLoadingKey

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [sideLoadingKey 对象](../resources/intune-onboarding-sideloadingkey.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的 JSON 表示形式。

下表显示创建 [sideLoadingKey 时所需的属性](../resources/intune-onboarding-sideloadingkey.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|旁加载密钥唯一 ID。|
|value|String|Side Loading Key Value， it is 5x5 value， seperated by hiphens.|
|displayName|String|向 ITPro 管理员显示的旁加载密钥名称。|
|说明|String|旁加载 向 ITPro 管理员显示的密钥说明。|
|totalActivation|Int32|向 ITPro 管理员显示的旁加载密钥总激活。|
|lastUpdatedDateTime|String|向 ITPro 管理员显示的"旁加载密钥上次更新日期"。|



## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新 [的 sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```



