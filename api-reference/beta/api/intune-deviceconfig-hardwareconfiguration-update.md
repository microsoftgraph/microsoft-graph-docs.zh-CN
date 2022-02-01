---
title: 更新 hardwareConfiguration
description: 更新 hardwareConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6fac95e1e99fd4548668fb336f8d2661b399830
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291013"
---
# <a name="update-hardwareconfiguration"></a>更新 hardwareConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [hardwareConfiguration 对象](../resources/intune-deviceconfig-hardwareconfiguration.md) 的属性。

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
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [hardwareConfiguration 时所需的属性](../resources/intune-deviceconfig-hardwareconfiguration.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置的唯一标识符|
|version|Int32|硬件配置版本 (例如 1、2、3 ...) |
|displayName|字符串|硬件配置的名称|
|description|String|硬件配置说明|
|createdDateTime|DateTimeOffset|创建硬件配置的时间戳。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|修改硬件配置的时间戳。 此属性是只读的。|
|fileName|String|硬件配置的文件名|
|configurationFileContent|Binary|硬件配置的文件内容|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|硬件配置的 Oem (例如 DELL、HP、Surface 和 SurfaceDock) 。 可取值为：`dell`、`surface`、`surfaceDock`。|
|roleScopeTagIds|字符串集合|硬件配置的范围标记标识列表|
|perDevicePasswordDisabled|Boolean|一个值，指示是否禁用每个开发密码|



## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "da410f27-0f27-da41-270f-41da270f41da",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "configurationFileContent": "Y29uZmlndXJhdGlvbkZpbGVDb250ZW50",
  "hardwareConfigurationFormat": "surface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "perDevicePasswordDisabled": true
}
```




