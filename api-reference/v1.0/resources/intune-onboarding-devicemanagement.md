---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfac44b206a9cfa11e3d6b3a27d4d2284493698
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264799"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备管理功能的容器的单例实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-onboarding-devicemanagement-get.md)|[deviceManagement](../resources/intune-onboarding-devicemanagement.md)|读取 [deviceManagement](../resources/intune-onboarding-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-onboarding-devicemanagement-update.md)|[deviceManagement](../resources/intune-onboarding-devicemanagement.md)|更新 [deviceManagement](../resources/intune-onboarding-devicemanagement.md) 对象的属性。|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery.md)|布尔值|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceCategories|[deviceCategory](../resources/intune-onboarding-devicecategory.md) 集合|租户的设备类别列表。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 集合|由租户配置的 Exchange 连接器列表。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange 本地条件访问设置。 本地条件访问需要设备注册并符合邮件访问要求|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 集合|由租户配置的移动威胁防护连接器列表。|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合|由租户配置的设备管理合作伙伴列表。|
|complianceManagementPartners|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 集合|租户配置的合规性管理合作伙伴列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true,
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "privacyUrl": "String"
  }
}
```




