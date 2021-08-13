---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00ef217ce79409b2152327f36303396eb3feacee6cb7c662392c11ccbb4f51db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229120"
---
# <a name="intunebrand-resource-type"></a>intuneBrand 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|向最终用户显示的公司/组织名称。|
|themeColor|[rgbColor](../resources/intune-onboarding-rgbcolor.md)|公司门户应用程序和 Web 门户中使用的主要主题颜色。|
|showLogo|布尔值|表示是否显示管理员提供的徽标图像的布尔值。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用中显示的徽标图像，徽标后有浅色背景。|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用中显示的徽标图像，徽标后有深色背景。|
|showNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|showDisplayNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|contactITName|String|负责 IT 支持的员工/组织名称。|
|contactITPhoneNumber|String|负责 IT 支持的员工/组织的电话号码。|
|contactITEmailAddress|String|负责 IT 支持的员工/组织的电子邮件地址。|
|contactITNotes|String|负责 IT 支持的员工/组织的文本注释。|
|onlineSupportSiteUrl|String|指向公司/组织 IT 支持人员网站的 URL。|
|onlineSupportSiteName|String|显示公司/组织 IT 支持人员网站的名称。|
|privacyUrl|String|指向公司/组织隐私策略的 URL。|

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
  "showDisplayNameNextToLogo": true,
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String"
}
```




