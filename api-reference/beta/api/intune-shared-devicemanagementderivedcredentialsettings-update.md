---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f94ac3eb5328cd8723008a25fd72e30347a1ac9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867852"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a>更新 deviceManagementDerivedCredentialSettings

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagementDerivedCredentialSettings 对象](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）||
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp;**资源访问策略** | DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序||
| &nbsp; &nbsp; **设备配置** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp;**资源访问策略** | DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagementDerivedCredentialSettings 时所需的属性](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|派生凭据的唯一标识符|
|**RA 策略**|
|helpUrl|String|最终用户在使用公司门户检索派生凭据时可访问的 URL。|
|displayName|String|配置文件显示名称的配置文件。|
|issuer|[deviceManagementDerivedCredentialIssuer](../resources/intune-rapolicy-devicemanagementderivedcredentialissuer.md)|要使用的派生凭据提供程序。 可取值为：`intercede`、`entrustDatacard`、`purebred`。|
|notificationType|[deviceManagementDerivedCredentialNotificationType](../resources/intune-rapolicy-devicemanagementderivedcredentialnotificationtype.md)|用于通知最终用户打开公司门户以将使用证书的 WLAN、VPN 或电子邮件配置文件发送到设备的方法。 可取值为：`none`、`companyPortal`、`email`。|


## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








