---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 446106067a445b7367878480eef2d6bcfbe4235e
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630000"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>创建 deviceEnrollmentWindowsHelloForBusinessConfiguration

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。

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
|id|String|帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|设备注册显示名称继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|说明|String|设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|如果用户位于分配了注册配置的多个组中，则使用优先级。 用户仅受优先级值最低的配置使用。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|String 集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持注册配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)。 可取值为：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`。|
|pinMinimumLength|Int32|控制用户 PIN 所需的最少Windows Hello 企业版数。  此值必须介于 4 到 127 之间（包含 4 和 127 之间，并且小于或等于为最大 PIN 设置的值）。|
|pinMaximumLength|Int32|控制 PIN 允许的最大Windows Hello 企业版数。 此值必须介于 4 和 127 之间（包含两者）。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 PIN 中能否使用大Windows Hello 企业版字母。  允许允许使用大写字母 (大) ，而 Required 可确保它们存在。 如果设置为"不允许"，则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 PIN 中能否使用小Windows Hello 企业版字母。  允许允许使用小写字母 () ，而 Required 可确保它们存在。 如果设置为"不允许"，则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 PIN 中使用特殊Windows Hello 企业版的能力。  Allowed 允许使用特殊字符 (字符) ，而 Required 可确保它们存在。 如果设置为"不允许"， (不允许) 特殊字符。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[enablement](../resources/intune-shared-enablement.md)|控制是否允许为设备配置Windows Hello 企业版。 如果设置为禁用，用户将无法预配Windows Hello 企业版加入 Azure Active Directory 的移动电话上除外（如果需要）。 如果设置为"未配置"，Intune将不会覆盖客户端默认值。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要受信任的平台模块 (TPM) 来预配Windows Hello 企业版。 TPM 提供了额外的安全优势，因为存储在 TPM 上的数据不能用于其他设备。 如果设置为 False，则所有设备都可以预配Windows Hello 企业版，即使不存在可用 TPM。|
|unlockWithBiometricsEnabled|Boolean|控制将生物识别手势（如人脸和指纹）用作安全 PIN 的Windows Hello 企业版。  如果设置为 False，则不允许生物识别手势。 用户仍必须将 PIN 配置为备份，以防发生故障。|
|remotePassportEnabled|Boolean|控制远程远程Windows Hello 企业版。 远程Windows Hello 企业版使可移植的已注册设备能够用作桌面身份验证的配套设备。 桌面必须加入 Azure AD，并且配套设备必须具有Windows Hello 企业版 PIN。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去 PIN 的能力。 这必须在 0 和 50 之间（包含 0 和 50）进行设置，并且用户的当前 PIN 包含在该计数中。 如果设置为 0，则不存储以前的 PIN。 PIN 历史记录不会通过 PIN 重置保留。|
|pinExpirationInDays|Int32|控制在系统 (PIN 之前) PIN 的时间段（以天表示）。 这必须设置为 0 到 730 之间（包含两者）。 如果设置为 0，则用户的 PIN 永不过期|
|enhancedBiometricsState|[enablement](../resources/intune-shared-enablement.md)|控制在支持防欺骗功能的设备上使用反欺骗功能进行面部识别的能力。 如果设置为禁用，则不允许使用反欺骗功能。 如果设置为"未配置"，用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityKeyForSignIn|[enablement](../resources/intune-shared-enablement.md)|登录安全密钥提供远程打开/关闭功能Windows Hello未配置的 Sercurity Keyl 将采用在 clinet 上完成的配置。 可取值为：`notConfigured`、`enabled`、`disabled`。|



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




