---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37877f36d51b010e7d0adaeecf0c2a7889416b6a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212026"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>创建 deviceEnrollmentWindowsHelloForBusinessConfiguration

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。

下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持从 [deviceEnrollmentConfiguration 继承的](../resources/intune-shared-deviceenrollmentconfiguration.md)注册配置类型。 可能的值是：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`、`enrollmentNotificationsConfiguration`。|
|pinMinimumLength|Int32|控制Windows Hello 企业版 PIN 所需的最小字符数。  此值必须介于 4 和 127 之间，包括，并且小于或等于为最大 PIN 设置的值。|
|pinMaximumLength|Int32|控制允许Windows Hello 企业版 PIN 的最大字符数。 此值必须介于 4 和 127 之间，包括在内。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在Windows Hello 企业版 PIN 中使用大写字母的功能。  允许使用大写字母 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在Windows Hello 企业版 PIN 中使用小写字母的功能。  允许使用小写字母 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在Windows Hello 企业版 PIN 中使用特殊字符的功能。  允许使用特殊字符 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用特殊字符 () 。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[支持](../resources/intune-shared-enablement.md)|控制是否允许为Windows Hello 企业版配置设备。 如果设置为“已禁用”，则用户无法预配Windows Hello 企业版（Azure Active Directory联接的移动电话除外（如果另有需要）。 如果设置为“未配置”，Intune不会重写客户端默认值。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要受信任的平台模块 (TPM) 来预配Windows Hello 企业版。 TPM 提供额外的安全优势，因为存储在它上的数据不能在其他设备上使用。 如果设置为 False，则所有设备都可以预配Windows Hello 企业版即使没有可用的 TPM。|
|unlockWithBiometricsEnabled|Boolean|控制使用生物识别手势（如人脸和指纹）作为Windows Hello 企业版 PIN 的替代方法。  如果设置为 False，则不允许使用生物识别手势。 如果发生故障，用户仍必须将 PIN 配置为备份。|
|remotePassportEnabled|Boolean|控制远程Windows Hello 企业版的使用。 远程Windows Hello 企业版使可移植的已注册设备能够用作桌面身份验证的配套设备。 必须Azure AD联接桌面，配套设备必须具有Windows Hello 企业版 PIN。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去 PIN 的功能。 这必须设置在 0 到 50 之间，包括在内，并且该计数中包含用户的当前 PIN。 如果设置为 0，则不会存储以前的 PIN。 PIN 历史记录不会通过 PIN 重置来保留。|
|pinExpirationInDays|Int32|控制在系统要求用户更改 PIN 之前可以使用 PIN 的时间段 (天) 。 这必须设置在 0 到 730 之间，包括在内。 如果设置为 0，则用户的 PIN 永远不会过期|
|enhancedBiometricsState|[支持](../resources/intune-shared-enablement.md)|控制在支持它的设备上使用防欺骗功能进行面部识别的能力。 如果设置为禁用，则不允许使用反欺骗功能。 如果设置为“未配置”，用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityKeyForSignIn|[支持](../resources/intune-shared-enablement.md)|登录的安全密钥提供远程打开/关闭的容量Windows Hello未配置的 Sercurity Keyl 将遵循在 clinet 上执行的配置。 可取值为：`notConfigured`、`enabled`、`disabled`。|



## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 778

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 950

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
  "deviceEnrollmentConfigurationType": "limit",
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




