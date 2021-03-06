---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型
description: WindowsHello 企业设置允许用户使用手势（如生物识别身份验证或 PIN）访问其设备。 配置注册用户、Windows 10 Windows 10 移动版及更高版本的设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb1e1533f37be13eb40e0775e34879bd721c3319
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751599"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsHello 企业设置允许用户使用手势（如生物识别身份验证或 PIN）访问其设备。 配置注册用户、Windows 10 Windows 10 移动版及更高版本的设置。


继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 集合|列出 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性和关系。|
|[获取 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|读取 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性和关系。|
|[创建 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。|
|[删除 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|无|删除 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)。|
|[更新 deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|说明|String|设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|priority|Int32|如果用户位于分配了注册配置的多个组中，则使用优先级。 用户仅受优先级值最低的配置使用。 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|version|Int32|设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|控制 Hello 企业 PIN 所需的最少Windows字符数。  此值必须介于 4 到 127 之间（包含 4 和 127 之间，并且小于或等于为最大 PIN 设置的值）。|
|pinMaximumLength|Int32|控制 Hello 企业 PIN 允许的最大Windows数。 此值必须介于 4 和 127 之间（包含两者）。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Hello 企业 PIN Windows大写字母的能力。  Allowed 允许使用大写字母 (大写) ，而 Required 可确保它们存在。 如果设置为"不允许"，则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Hello 企业 PIN 中Windows小写字母的能力。  Allowed 允许使用小写字母 () ，而 Required 可确保它们存在。 如果设置为"不允许"，则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Hello 企业 PIN 中Windows字符的能力。  允许允许使用特殊字符 (字符) ，而 Required 可确保它们存在。 如果设置为"不允许"， (不允许) 特殊字符。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[enablement](../resources/intune-onboarding-enablement.md)|控制是否允许为 Hello 企业Windows设备。 如果设置为禁用，则用户无法预配 Windows Hello 企业版，除非Azure Active Directory已加入的移动电话上（如果需要）。 如果设置为"未配置"，Intune 将不会覆盖客户端默认值。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要受信任的平台模块 (TPM) Hello 企业Windows预配。 TPM 提供了额外的安全优势，因为存储在 TPM 上的数据不能用于其他设备。 如果设置为 False，则所有设备都可以预配 Windows Hello 企业，即使没有可用 TPM。|
|unlockWithBiometricsEnabled|Boolean|控制将生物识别手势（如人脸和指纹）用作 Windows Hello 企业 PIN 的替代方法。  如果设置为 False，则不允许生物识别手势。 用户仍必须将 PIN 配置为备份，以防发生故障。|
|remotePassportEnabled|Boolean|控制使用远程 Windows Hello 企业。 通过Windows Hello 企业版，可移植的已注册设备可以用作桌面身份验证的配套设备。 桌面必须加入 Azure AD，配套设备必须具有 Windows Hello 企业版 PIN。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去 PIN 的能力。 必须将其设置为 0 到 50（含 0 和 50）之间，并且用户的当前 PIN 包含在该计数中。 如果设置为 0，则不存储以前的 PIN。 PIN 历史记录不会通过 PIN 重置保留。|
|pinExpirationInDays|Int32|控制在系统 (PIN 之前) PIN 的时间段（以天表示）。 这必须设置为 0 到 730 之间（包含这两者）。 如果设置为 0，则用户的 PIN 永不过期|
|enhancedBiometricsState|[enablement](../resources/intune-onboarding-enablement.md)|控制在支持防欺骗功能的设备上使用反欺骗功能进行面部识别的能力。 如果设置为禁用，则不允许使用反欺骗功能。 如果设置为"未配置"，用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|设备配置文件的组分配列表 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

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
  "enhancedBiometricsState": "String"
}
```




