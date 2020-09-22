---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2df3a5c21f181ed48bbb2410677f08bcfee7bea7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045066"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a>更新 deviceEnrollmentWindowsHelloForBusinessConfiguration

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。

下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符|
|displayName|String|从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称|
|description|String|从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配有注册配置的多个组中时，将使用优先级。 用户仅限于具有最低优先级值的配置。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间|
|lastModifiedDateTime|DateTimeOffset|从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间|
|version|Int32|继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本|
|roleScopeTagIds|String 集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|控制 Windows Hello 企业版 PIN 所需的最小字符数。  此值必须介于4和127之间（含这两个值），且小于或等于为最大 PIN 设置的值。|
|pinMaximumLength|Int32|控制 Windows Hello 企业版 PIN 所允许的最大字符数。 此值必须介于4和127之间（含这两个值）。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用大写字母的功能。  允许使用大写字母 (s) ，而必需的则可确保这些字母存在。 如果设置为 "不允许"，则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用小写字母的功能。  允许使用小写字母 (s) ，而必需的则可确保它们存在。 如果设置为 "不允许"，则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用特殊字符的功能。  允许使用特殊字符 (s) ，而必需的则可确保它们存在。 如果设置为 "不允许"，则不允许使用特殊字符 (s) 。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[启用](../resources/intune-shared-enablement.md)|控制是否允许为 Windows Hello 企业版配置设备。 如果设置为 "禁用"，则用户将无法预配 Windows Hello 企业版，除非在其他情况下有必要时在 Azure Active Directory 加入移动电话上。 如果设置为 "未配置"，Intune 将不会覆盖客户端默认设置。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要受信任的平台模块 (TPM) 来设置 Windows Hello 企业版。 TPM 在其他设备上不能使用存储在其上的数据带来额外的安全性优势。 如果设置为 False，即使没有可用的 TPM，所有设备也可以预配 Windows Hello 企业版。|
|unlockWithBiometricsEnabled|Boolean|控制使用生物特征手势（如面孔和指纹）作为 Windows Hello 企业版 PIN 的替代方法。  如果设置为 False，则不允许使用生物特征手势。 用户仍必须在发生故障时将 PIN 配置为备份。|
|remotePassportEnabled|Boolean|控制远程 Windows Hello 企业版的使用。 远程 Windows Hello 企业版使便携式、注册设备可用作桌面身份验证的配套功能。 桌面必须已加入 Azure AD，且配套设备必须具有 Windows Hello 企业版 PIN。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去的 Pin 的功能。 必须在0和50之间设置此值（包括这两个值），并且用户的当前 PIN 包含在该计数中。 如果设置为0，则不存储以前的 Pin。 PIN 历史记录不会通过 PIN 重置来保留。|
|pinExpirationInDays|Int32|控制在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）)  (。 必须在0和730之间设置此值（包括这两个值）。 如果设置为0，则用户的 PIN 永不过期|
|enhancedBiometricsState|[启用](../resources/intune-shared-enablement.md)|控制在支持它的设备上使用反欺骗功能进行面部识别。 如果设置为 "禁用"，则不允许反欺骗功能。 如果设置为 "未配置"，则用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityKeyForSignIn|[启用](../resources/intune-shared-enablement.md)|登录的安全密钥提供远程开启/关闭 Windows Hello Sercurity Keyl 的容量。未配置将服从在 clinet 上完成的配置。 可取值为：`notConfigured`、`enabled`、`disabled`。|



## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 729

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```






