---
title: organizationalBrandingLocalization 资源类型
description: 包含组织品牌本地化的详细信息。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 847f5271250de49108dfcb7c680847121ea35063
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647012"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>organizationalBrandingLocalization 资源类型

命名空间：microsoft.graph

支持管理特定语言品牌的资源。 虽然你无法更改原始配置的语言，但此资源允许你为另一种语言创建新配置。

继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 organizationalBrandingLocalizations](../api/organizationalbranding-list-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 集合|获取 [organizationalBrandingLocalization 对象](../resources/organizationalbrandinglocalization.md) 及其属性的列表。|
|[创建 organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|创建新的 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。|
|[Get organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|读取 [organizationalBrandingLocalization 对象的属性和](../resources/organizationalbrandinglocalization.md) 关系。|
|[更新 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| 无 |更新 [organizationalBrandingLocalization 对象](../resources/organizationalbrandinglocalization.md) 的属性。|
|[删除 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|无|删除 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。|

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| backgroundColor | String | 将出现在低带宽连接中的背景图像上的颜色。 我们建议你使用横幅徽标的主要颜色或你的组织颜色。 以十六进制格式指定此参数，例如，white 为 `#FFFFFF` 。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB 且不超过 1920 × 1080 像素。 较小的图像将降低带宽要求，并加快页面加载速度。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| backgroundImageRelativeUrl | String | **backgroundImage** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| bannerLogo | Stream | 显示在登录页上的公司徽标的横幅版本。 允许的类型为 PNG 或 JPEG，不超过 36 × 245 像素。 我们建议使用透明图像，徽标周围没有填充。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| bannerLogoRelativeUrl | String | **bannerLogo** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN 提供的只读CDN。 只读。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| cdnList | 字符串集合 | 提供当前资源资产的所有可用CDN提供程序的基 URL 列表。 多个CDN提供程序同时用于读取请求的高可用性。 只读。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| id | String | 表示使用区域性名称指定的区域设置的标识符。 区域性名称遵循 RFC 1766 标准，格式为"languagecode2-country/regioncode2"，其中"languagecode2"是派生自 ISO 639-1 的大写两字母代码，而"country/regioncode2"是派生自 ISO 3166 的大写两字母代码。 例如，美国英语为 `en-US` 。 默认 /branding 的 **ID** 始终为 String `0` 类型或 `default` 。 只读。 <br/><br/>**注意：** 目前不支持单个区域设置的多个品牌。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| signInPageText | String | 显示在登录框底部的文本。 您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须是 Unicode 且不超过 1024 个字符。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| squareLogo | Stream | 现现Windows 10 OOBE (和启用 Windows Autopilot 进行部署时) 显示公司徽标的正方形版本。 允许的类型为 PNG 或 JPEG，不超过 240 x 240 像素，大小不超过 10 KB。 我们建议使用透明图像，徽标周围没有填充。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。|
| squareLogoRelativeUrl | String | **squareLogo** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |
| usernameHintText | String | 在登录屏幕的用户名文本框中显示为提示的字符串。 此文本必须是不带链接或代码的 Unicode，并且不能超过 64 个字符。 继承自 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String"
}
```
