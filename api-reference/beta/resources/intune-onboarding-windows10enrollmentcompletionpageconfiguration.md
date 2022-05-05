---
title: windows10EnrollmentCompletionPageConfiguration 资源类型
description: Windows 10注册状态页配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19ff052b64aff545d4030d7f4491084ef9009d64
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209196"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>windows10EnrollmentCompletionPageConfiguration 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10注册状态页配置


继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10EnrollmentCompletionPageConfigurations](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 集合|列出 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象的属性和关系。|
|[获取 windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|读取 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象的属性和关系。|
|[创建 windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|创建新的 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 对象。|
|[删除 windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|无|删除 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)。|
|[更新 windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|更新 [windows10EnrollmentCompletionPageConfiguration 对象的](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持从 [deviceEnrollmentConfiguration 继承的](../resources/intune-shared-deviceenrollmentconfiguration.md)注册配置类型。 可能的值是：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`、`enrollmentNotificationsConfiguration`。|
|showInstallationProgress|Boolean|向用户显示或隐藏安装进度|
|blockDeviceSetupRetryByUser|Boolean|允许用户在安装失败时重试安装程序|
|allowDeviceResetOnInstallFailure|Boolean|在安装失败时允许或阻止设备重置|
|allowLogCollectionOnInstallFailure|Boolean|在安装失败时允许或阻止日志收集|
|customErrorMessage|字符串|设置安装失败时显示的自定义错误消息|
|installProgressTimeoutInMinutes|Int32|设置安装进度超时（以分钟为单位）|
|allowDeviceUseOnInstallFailure|Boolean|允许用户在安装失败时继续使用设备|
|selectedMobileAppIds|String collection|用于跟踪安装状态的选定应用程序|
|trackInstallProgressForAutopilotOnly|Boolean|仅显示 Autopilot 注册方案的安装进度|
|disableUserStatusTrackingAfterFirstUser|Boolean|仅显示第一个用户注册后的安装进度|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备配置文件的组分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "String"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```




