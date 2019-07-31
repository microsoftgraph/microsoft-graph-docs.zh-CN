---
title: intuneBrandingProfile 资源类型
description: 此实体包含在自定义公司门户应用程序的租户级别外观和最终用户 web 门户时使用的数据。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e922634ec08e1fab412c160d2d8fe7f45d0dde5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010152"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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
|[分配操作](../api/intune-wip-intunebrandingprofile-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件键|
|profileName|String|配置文件的名称|
|profileDescription|String|配置文件的说明|
|isDefaultProfile|Boolean|一个 Boolean 类型的值, 该值表示是否将配置文件用作默认配置文件|
|createdDateTime|DateTimeOffset|创建 BrandingProfile 的时间|
|lastModifiedDateTime|DateTimeOffset|上次修改 BrandingProfile 的时间|
|displayName|字符串|向最终用户显示的公司/组织名称|
|contactITName|String|负责 IT 支持的人员/组织的名称|
|contactITPhoneNumber|String|负责 IT 支持的个人/组织的电话号码|
|contactITEmailAddress|String|负责 IT 支持的个人/组织的电子邮件地址|
|contactITNotes|String|关于负责 IT 支持的人员/组织的文本注释|
|privacyUrl|String|指向公司/组织的隐私策略的 URL|
|onlineSupportSiteUrl|String|指向公司/组织的 IT 支持人员网站的 URL|
|onlineSupportSiteName|String|公司/组织的 IT 支持人员网站的显示名称|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|公司门户应用程序和 web 门户中使用的主要主题颜色|
|showLogo|Boolean|Boolean 类型的值, 该值表示是否显示管理员提供的徽标图像|
|showDisplayNameNextToLogo|布尔值|一个 Boolean 类型的值, 该值表示是否在徽标图像旁边显示管理员提供的显示名称|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用程序中显示的徽标图像, 其徽标后面有主题颜色背景|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用程序中显示的徽标图像, 徽标后面有浅背景|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用登录页中显示的自定义图像|
|customPrivacyMessage|String|有关管理员在设备上有权访问的内容的文本注释|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)集合|品牌配置文件的组分配列表|

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
  },
  "customPrivacyMessage": "String"
}
```





