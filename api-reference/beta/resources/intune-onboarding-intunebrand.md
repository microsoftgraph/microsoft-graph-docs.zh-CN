---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7790c970ce7cee1cfcef9e2dfa07eb08dfeb864c4730c24b7e2cdf576fa8644
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226271"
---
# <a name="intunebrand-resource-type"></a>intuneBrand 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|向最终用户显示的公司/组织名称。|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|公司门户应用程序和 Web 门户中使用的主要主题颜色。|
|showLogo|布尔值|表示是否显示管理员提供的徽标图像的布尔值。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用中显示的徽标图像，徽标后有浅色背景。|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用中显示的徽标图像，徽标后有深色背景。|
|showNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|在应用登录公司门户中显示的自定义图像|
|showDisplayNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|roleScopeTagIds|String collection|分配给默认品牌配置文件的范围标记列表|
|contactITName|String|负责 IT 支持的员工/组织名称。|
|contactITPhoneNumber|String|负责 IT 支持的员工/组织的电话号码。|
|contactITEmailAddress|String|负责 IT 支持的员工/组织的电子邮件地址。|
|contactITNotes|String|负责 IT 支持的员工/组织的文本注释。|
|onlineSupportSiteUrl|String|指向公司/组织 IT 支持人员网站的 URL。|
|onlineSupportSiteName|String|显示公司/组织 IT 支持人员网站的名称。|
|privacyUrl|String|指向公司/组织隐私策略的 URL。|
|customPrivacyMessage|String|用于说明组织在托管设备上看不到或无法执行哪些操作的自定义隐私消息。|
|customCantSeePrivacyMessage|String|用于说明组织在托管设备上看不到或无法执行哪些操作的自定义隐私消息。|
|customCanSeePrivacyMessage|字符串|用于说明组织可在托管设备上查看和执行哪些操作的自定义隐私消息。|
|isRemoveDeviceDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"删除设备"操作。|
|isFactoryResetDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"恢复出厂设置"操作。|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合|根据平台和设备所有权类型，在公司门户上阻止的操作的集合。|
|showAzureADEnterpriseApps|布尔值|Boolean 值，指示 AzureAD Enterprise应用是否将显示在 公司门户|
|showOfficeWebApps|布尔值|Boolean 值，Office WebApps 是否将显示在公司门户|
|sendDeviceOwnershipChangePushNotification|布尔值|指示当用户的设备所有权类型从个人更改到公司时是否向用户发送推送通知的布尔值|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|向最终用户显示的自定义设备注册流。 可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。|
|disableClientTelemetry|布尔值|适用于从所有客户端发送到 Intune 服务的遥测。 禁用后，将关闭客户端内的所有主动故障排除和发出警告，并且遥测设置对设备用户显示为非活动或隐藏。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
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
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "disableClientTelemetry": true
}
```




