---
title: intuneBrandingProfile 资源类型
description: 此实体包含在自定义公司门户应用程序的租户级别外观和最终用户 web 门户时使用的数据。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f21cc97cd701f9826743475c4055aed6bafe9ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144700"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体包含在自定义公司门户应用程序的租户级别外观和最终用户 web 门户时使用的数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)集合|列出[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性和关系。|
|[获取 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|读取[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性和关系。|
|[创建 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。|
|[删除 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|无|删除[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)。|
|[更新 intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。|
|[assign 操作](../api/intune-wip-intunebrandingprofile-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|配置文件键|
|profileName|字符串|配置文件的名称|
|profileDescription|字符串|配置文件的说明|
|isDefaultProfile|布尔|显示配置文件是否用于默认设置。|
|createdDateTime|DateTimeOffset|创建 BrandingProfile 时。|
|lastModifiedDateTime|DateTimeOffset|上次修改 BrandingProfile 的时间。|
|displayName|字符串|向最终用户显示的公司/组织名称。|
|contactITName|字符串|负责 IT 支持的员工/组织名称。|
|contactITPhoneNumber|字符串|负责 IT 支持的员工/组织的电话号码。|
|contactITEmailAddress|字符串|负责 IT 支持的员工/组织的电子邮件地址。|
|contactITNotes|字符串|负责 IT 支持的员工/组织的文本注释。|
|privacyUrl|字符串|指向公司/组织隐私策略的 URL。|
|onlineSupportSiteUrl|字符串|指向公司/组织 IT 支持人员网站的 URL。|
|onlineSupportSiteName|String|显示公司/组织 IT 支持人员网站的名称。|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|公司门户应用程序和 Web 门户中使用的主要主题颜色。|
|showLogo|布尔|表示是否显示管理员提供的徽标图像的布尔值。|
|showDisplayNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在主题颜色背景上的公司门户应用程序中显示的徽标图像。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在 "浅色背景" 的公司门户应用程序中显示的徽标图像。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用登录页中显示的自定义图像|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)集合|品牌配置文件的组分配的列表。|

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
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
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
  }
}
```




