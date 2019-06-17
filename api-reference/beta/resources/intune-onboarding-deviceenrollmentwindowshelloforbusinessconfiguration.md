---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型
description: Windows Hello 企业版设置允许用户使用笔势 (如生物特征身份验证或 PIN) 访问其设备。 为已注册的 Windows 10、Windows 10 移动版和更高版本配置设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5fcc6d83083d79d71f5e7393dd11d23febd92bd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993121"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows Hello 企业版设置允许用户使用笔势 (如生物特征身份验证或 PIN) 访问其设备。 为已注册的 Windows 10、Windows 10 移动版和更高版本配置设置。


继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 集合|列出 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性和关系。|
|[获取 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|读取 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性和关系。|
|[创建 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。|
|[删除 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|无|删除 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)。|
|[更新 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符|
|displayName|String|从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称|
|说明|String|从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配有注册配置的多个组中时, 将使用优先级。 用户仅限于具有最低优先级值的配置。 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间|
|lastModifiedDateTime|DateTimeOffset|从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间|
|version|Int32|继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本|
|pinMinimumLength|Int32|控制 Windows Hello 企业版 PIN 所需的最小字符数。  此值必须介于4和127之间 (含这两个值), 且小于或等于为最大 PIN 设置的值。|
|pinMaximumLength|Int32|控制 Windows Hello 企业版 PIN 所允许的最大字符数。 此值必须介于4和127之间 (含这两个值)。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用大写字母的功能。  允许使用大写字母 (s), 而必需的字符可确保它们存在。 如果设置为 "不允许", 则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用小写字母的功能。  允许使用小写字母, 而必需的则可确保它们存在。 如果设置为 "不允许", 则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello 企业版 PIN 中使用特殊字符的功能。  允许使用特殊字符, 而必需的字符可确保它们存在。 如果设置为 "不允许", 则不允许使用特殊字符。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[启用](../resources/intune-shared-enablement.md)|控制是否允许为 Windows Hello 企业版配置设备。 如果设置为 "禁用", 则用户将无法预配 Windows Hello 企业版, 除非在其他情况下有必要时在 Azure Active Directory 加入移动电话上。 如果设置为 "未配置", Intune 将不会覆盖客户端默认设置。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要用于设置 Windows Hello 企业版的受信任的平台模块 (TPM)。 TPM 在其他设备上不能使用存储在其上的数据带来额外的安全性优势。 如果设置为 False, 即使没有可用的 TPM, 所有设备也可以预配 Windows Hello 企业版。|
|unlockWithBiometricsEnabled|Boolean|控制使用生物特征手势 (如面孔和指纹) 作为 Windows Hello 企业版 PIN 的替代方法。  如果设置为 False, 则不允许使用生物特征手势。 用户仍必须在发生故障时将 PIN 配置为备份。|
|remotePassportEnabled|Boolean|控制远程 Windows Hello 企业版的使用。 远程 Windows Hello 企业版使便携式、注册设备可用作桌面身份验证的配套功能。 桌面必须已加入 Azure AD, 且配套设备必须具有 Windows Hello 企业版 PIN。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去的 Pin 的功能。 必须在0和50之间设置此值 (包括这两个值), 并且用户的当前 PIN 包含在该计数中。 如果设置为 0, 则不存储以前的 Pin。 PIN 历史记录不会通过 PIN 重置来保留。|
|pinExpirationInDays|Int32|控制在系统要求用户更改 PIN 之前可以使用 PIN 的时间段 (以天为单位)。 必须在0和730之间设置此值 (包括这两个值)。 如果设置为 0, 则用户的 PIN 永不过期|
|enhancedBiometricsState|[启用](../resources/intune-shared-enablement.md)|控制在支持它的设备上使用反欺骗功能进行面部识别。 如果设置为 "禁用", 则不允许反欺骗功能。 如果设置为 "未配置", 则用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityKeyForSignIn|[启用](../resources/intune-shared-enablement.md)|登录的安全密钥提供远程开启/关闭 Windows Hello Sercurity Keyl 的容量。未配置将服从在 clinet 上完成的配置。 可取值为：`notConfigured`、`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String",
  "securityKeyForSignIn": "String"
}
```





