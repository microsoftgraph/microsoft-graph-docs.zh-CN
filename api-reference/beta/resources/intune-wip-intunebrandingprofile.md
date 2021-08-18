---
title: intuneBrandingProfile 资源类型
description: 此实体包含用于自定义应用程序以及最终用户 Web 门户公司门户租户级别外观的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 15fbf2802b078214c0c78e11576364ee074560645f471122d56bda2cccfc7dc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209775"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体包含用于自定义应用程序以及最终用户 Web 门户公司门户租户级别外观的数据。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 集合|列出 [intuneBrandingProfile 对象的属性和](../resources/intune-wip-intunebrandingprofile.md) 关系。|
|[获取 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|读取 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象的属性和关系。|
|[创建 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|创建新的 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象。|
|[删除 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|无|删除 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)。|
|[更新 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|更新 [intuneBrandingProfile 对象](../resources/intune-wip-intunebrandingprofile.md) 的属性。|
|[分配操作](../api/intune-wip-intunebrandingprofile-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件密钥|
|profileName|String|配置文件的名称|
|profileDescription|String|配置文件的说明|
|isDefaultProfile|布尔值|表示配置文件是否用作默认配置文件的布尔值|
|createdDateTime|DateTimeOffset|BrandingProfile 创建时间|
|lastModifiedDateTime|DateTimeOffset|BrandingProfile 上次修改的时间|
|displayName|字符串|向最终用户显示的公司/组织名称|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|应用程序应用程序和 Web 门户公司门户主题颜色|
|showLogo|布尔值|表示是否显示管理员提供的徽标图像的布尔值|
|showDisplayNameNextToLogo|布尔值|Boolean 值，表示管理员显示名称是否显示在徽标图像旁边|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|徽标在徽标公司门户具有主题颜色背景的应用中显示的徽标图像|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|徽标显示在徽标公司门户背景浅色的应用中显示的徽标图像|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|自定义图像显示在应用公司门户页面中|
|contactITName|String|负责 IT 支持人员/组织的名称|
|contactITPhoneNumber|String|电话 IT 支持人员/组织的数量|
|contactITEmailAddress|String|负责 IT 支持的人/组织的电子邮件地址|
|contactITNotes|String|有关负责 IT 支持的人/组织的文本注释|
|onlineSupportSiteUrl|String|指向公司/组织的 IT 支持人员网站的 URL|
|onlineSupportSiteName|String|公司/组织的 IT 支持人员网站的显示名称|
|privacyUrl|String|指向公司/组织隐私策略的 URL|
|customPrivacyMessage|String|有关管理员在设备上无法访问的内容的文本注释|
|customCanSeePrivacyMessage|String|有关管理员在设备上有权访问的内容的文本注释|
|customCantSeePrivacyMessage|字符串|有关管理员在设备上无法访问的内容的文本注释|
|isRemoveDeviceDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"删除设备"操作。|
|isFactoryResetDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"恢复出厂设置"操作。|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合|根据平台和设备所有权类型，在公司门户上阻止的操作的集合。|
|showAzureADEnterpriseApps|布尔值|Boolean 值，指示 AzureAD Enterprise应用是否将显示在 公司门户|
|showOfficeWebApps|布尔值|Boolean 值，Office WebApps 是否将显示在 公司门户|
|sendDeviceOwnershipChangePushNotification|布尔值|指示当用户的设备所有权类型从个人更改到公司时是否向用户发送推送通知的布尔值|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|向最终用户显示的自定义设备注册流。 可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。|
|disableClientTelemetry|布尔值|适用于从所有客户端发送到 Intune 服务的遥测。 禁用后，将关闭客户端内的所有主动故障排除和发出警告，并且遥测设置对设备用户显示为非活动或隐藏。|
|roleScopeTagIds|String collection|分配给品牌配置文件的范围标记列表|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) 集合|品牌配置文件的组分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




