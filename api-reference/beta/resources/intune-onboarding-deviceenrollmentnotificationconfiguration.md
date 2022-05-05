---
title: deviceEnrollmentNotificationConfiguration 资源类型
description: 用于发送通知的注册通知配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 370fd69ef878051dca2a62ef98b84f93de806ed3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213114"
---
# <a name="deviceenrollmentnotificationconfiguration-resource-type"></a>deviceEnrollmentNotificationConfiguration 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于发送通知的注册通知配置


继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceEnrollmentNotificationConfigurations](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-list.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) 集合|列出 [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) 对象的属性和关系。|
|[获取 deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-get.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|读取 [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) 对象的属性和关系。|
|[创建 deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-create.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|创建新的 [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) 对象。|
|[删除 deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-delete.md)|无|删除 [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)。|
|[更新 deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-update.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|更新 [deviceEnrollmentNotificationConfiguration 对象的](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的帐户的唯一标识符|
|displayName|String|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的显示名称|
|说明|字符串|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的说明|
|priority|Int32|当用户存在于分配了注册配置的多个组中时，将使用优先级。 用户仅受优先级最低的配置的约束。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|在 UTC 中创建的设备注册配置的日期时间继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的 UTC 中上次修改的日期时间|
|version|Int32|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备注册配置的版本|
|roleScopeTagIds|字符串集合|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|支持从 [deviceEnrollmentConfiguration 继承的](../resources/intune-shared-deviceenrollmentconfiguration.md)注册配置类型。 可能的值是：`unknown`、`limit`、`platformRestrictions`、`windowsHelloForBusiness`、`defaultLimit`、`defaultPlatformRestrictions`、`defaultWindowsHelloForBusiness`、`defaultWindows10EnrollmentCompletionPageConfiguration`、`windows10EnrollmentCompletionPageConfiguration`、`deviceComanagementAuthorityConfiguration`、`singlePlatformRestriction`、`unknownFutureValue`、`enrollmentNotificationsConfiguration`。|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|注册通知的平台类型。 可取值为：`allPlatforms`、`ios`、`windows`、`windowsPhone`、`android`、`androidForWork` 或 `mac`。|
|templateType|[enrollmentNotificationTemplateType](../resources/intune-onboarding-enrollmentnotificationtemplatetype.md)|注册通知的模板类型。 可取值为：`email`、`push`、`unknownFutureValue`。|
|notificationMessageTemplateId|Guid|通知消息模板 ID|
|brandingOptions|[enrollmentNotificationBrandingOptions](../resources/intune-onboarding-enrollmentnotificationbrandingoptions.md)|注册通知的品牌选项。 可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`、`includeCompanyPortalLink`、`includeDeviceDetails`。|
|defaultLocale|String|注册通知的 DefaultLocale|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|从 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 继承的设备配置文件的组分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentNotificationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentNotificationConfiguration",
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
  "platformType": "String",
  "templateType": "String",
  "notificationMessageTemplateId": "Guid",
  "brandingOptions": "String",
  "defaultLocale": "String"
}
```




