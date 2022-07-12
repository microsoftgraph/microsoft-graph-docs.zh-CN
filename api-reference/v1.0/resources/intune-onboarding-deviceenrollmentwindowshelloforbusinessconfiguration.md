---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型
description: Windows Hello企业版设置允许用户使用手势（例如生物识别身份验证或 PIN）访问其设备。 配置已注册Windows 10、Windows 10 移动版及更高版本的设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 762486463ee207107b36e7a93c5d8b3f0db43ac0
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734933"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows Hello企业版设置允许用户使用手势（例如生物识别身份验证或 PIN）访问其设备。 配置已注册Windows 10、Windows 10 移动版及更高版本的设置。


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
|id|String|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|String|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|pinMinimumLength|Int32|控制业务 PIN Windows Hello所需的最小字符数。  此值必须介于 4 和 127 之间，包括，并且小于或等于为最大 PIN 设置的值。|
|pinMaximumLength|Int32|控制业务 PIN Windows Hello允许的最大字符数。 此值必须介于 4 和 127 之间，包括在内。 此值必须大于或等于为最小 PIN 设置的值。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在业务 PIN Windows Hello中使用大写字母的功能。  允许使用大写字母 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用大写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello for Business PIN 中使用小写字母的功能。  允许使用小写字母 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用小写字母。 可取值为：`allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|控制在 Windows Hello for Business PIN 中使用特殊字符的功能。  允许使用特殊字符 () ，而“必需”则确保它们存在。 如果设置为“不允许”，则不允许使用特殊字符 () 。 可取值为：`allowed`、`required`、`disallowed`。|
|state|[支持](../resources/intune-onboarding-enablement.md)|控制是否允许为 Windows Hello for Business 配置设备。 如果设置为已禁用，则用户无法为业务预配Windows Hello（如果需要，则在已加入 Azure Active Directory 的移动电话上除外）。 如果设置为“未配置”，Intune 不会重写客户端默认值。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|Boolean|控制是否需要受信任的平台模块 (TPM) 来预配业务Windows Hello。 TPM 提供额外的安全优势，因为存储在它上的数据不能在其他设备上使用。 如果设置为 False，即使没有可用的 TPM，所有设备都可以为 Business 预配Windows Hello。|
|unlockWithBiometricsEnabled|Boolean|控制使用生物识别手势（如人脸和指纹）作为业务 PIN Windows Hello的替代方法。  如果设置为 False，则不允许使用生物识别手势。 如果发生故障，用户仍必须将 PIN 配置为备份。|
|remotePassportEnabled|Boolean|控制远程Windows Hello商业版的使用。 适用于企业的远程Windows Hello使可移植的已注册设备能够用作桌面身份验证的配套设备。 桌面必须已加入 Azure AD，配套设备必须具有适用于 Business PIN 的Windows Hello。|
|pinPreviousBlockCount|Int32|控制阻止用户使用过去 PIN 的功能。 这必须设置在 0 到 50 之间，包括在内，并且该计数中包含用户的当前 PIN。 如果设置为 0，则不会存储以前的 PIN。 PIN 历史记录不会通过 PIN 重置来保留。|
|pinExpirationInDays|Int32|控制在系统要求用户更改 PIN 之前可以使用 PIN 的时间段 (天) 。 这必须设置在 0 到 730 之间，包括在内。 如果设置为 0，则用户的 PIN 永远不会过期|
|enhancedBiometricsState|[支持](../resources/intune-onboarding-enablement.md)|控制在支持它的设备上使用防欺骗功能进行面部识别的能力。 如果设置为禁用，则不允许使用反欺骗功能。 如果设置为“未配置”，用户可以选择是否要使用反欺骗。 可取值为：`notConfigured`、`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|从 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 继承的设备配置文件的组分配列表|

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





