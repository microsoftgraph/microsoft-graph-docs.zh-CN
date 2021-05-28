---
title: organizationalBrandingProperties 资源类型
description: 包含组织品牌打造的详细信息。
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7fb68fb65974e177e3fa55408ee1b90e59d419e9
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682315"
---
# <a name="organizationalbrandingproperties-resource-type"></a>organizationalBrandingProperties 资源类型

>[!NOTE]
>添加自定义品牌打造需要Azure Active Directory 高级版 1 高级版 2 或 Basic 版本，或拥有 Microsoft 365 许可证。 有关许可和版本详细信息，请参阅注册 Azure [AD 高级版。](/azure/active-directory/fundamentals/active-directory-get-started-premium)<br><br>Azure AD 高级版 和 Basic 版本适用于使用全球 Azure Active Directory 中国客户。 Azure AD 高级版和 Basic 版本当前在中国由世纪网络运营的 Azure 服务中不受支持。 有关详细信息，请通过 Azure Active Directory[论坛与我们联系](https://feedback.azure.com/forums/169401-azure-active-directory/)。

包含有关组织品牌的详细信息。

组织可以自定义其 Azure AD 登录页面，当用户登录到其组织的租户特定应用时，或者当 Azure AD 通过用户名标识用户的租户时，会显示这些页面。 开发人员还可以阅读公司的品牌信息并自定义其应用体验，以使用其公司的品牌专门为登录用户定制它。

公司可以基于区域设置添加不同的品牌。 区域设置在所有请求中都用作键。

>**注意：** 品牌打造作为组织下的属性公开，具有特定于区域设置本地化的集合。 **organizationalBrandingProperties** 是一个抽象类，用于定义 **organizationalBranding 的属性**。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 使用 organizationalBrandingProperties 对象创建组织品牌。 |
| [获取](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 读取 organizationalBrandingProperties 对象的属性和关系。 |
| [更新](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 更新 organizationalBrandingProperties 对象。 |
| [删除](../api/organizationalbrandingproperties-delete.md) | 无 | 删除 organizationalBrandingProperties 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|backgroundColor|String| 将出现在低带宽连接中的背景图像上的颜色。 建议在此处使用横幅徽标或组织颜色的主要颜色。 以十六进制表示 (，例如，白色#FFFFFF) 。 |
|backgroundImage|Stream| 显示为登录页背景的图像。 .png或 .jpg不超过 1920x1080 且小于 300kb。 较小的图像将降低带宽要求，提高页面加载性能。 |
|bannerLogo|Stream| 显示在登录页上的公司徽标的横幅版本。 .png或.jpg不超过 36x245px。 我们建议使用透明图像，徽标周围没有填充。 |
|id|String| 这是一个继承自 microsoft.graph.entity 的 id，是指定语言 ISO 639 标准（例如英语为"en-us"或"en"）区域设置。 今后，如果我们公开功能以针对一个区域设置具有多个品牌，这一点可能会更改。 请注意，默认 /branding 的 ID 始终为"und"，直到我们具有无键单一性。 只读。 |
|signInPageText|String| 显示在登录框底部的文本。 您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须是 Unicode 且不超过 1024 个字符。 |
|squareLogo|Stream| 公司徽标的方形版本。 这将显示在Windows 10 OOBE 体验 (OOBE) ，以及启用 Windows Autopilot 进行部署时。 .png或 .jpg不超过 240x240px 且大小不超过 10kb。 我们建议使用透明图像，徽标周围没有填充。 |
|usernameHintText|String| 字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "keyProperty": "id"
}-->

```json
{
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "id": "String (identifier)",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationalBrandingProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
