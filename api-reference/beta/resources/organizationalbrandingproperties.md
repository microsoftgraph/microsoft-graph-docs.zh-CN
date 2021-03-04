---
title: organizationalBrandingProperties 资源类型
description: 包含组织品牌的详细信息。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e27966381c5838ac7662b977c5061a46bb660f1c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442913"
---
# <a name="organizationalbrandingproperties-resource-type"></a>organizationalBrandingProperties 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>添加自定义品牌需要你使用 Azure Active Directory Premium 1、Premium 2 或 Basic 版本，或者拥有 Microsoft 365 许可证。 有关许可和版本的信息，请参阅注册 Azure [AD Premium。](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)<br><br>Azure AD Premium 和 Basic 版本适用于使用全球 Azure Active Directory 实例的中国客户。 Azure AD Premium 和 Basic 版本当前不受中国世纪通运营的 Azure 服务的支持。 有关详细信息，请通过 Azure Active [Directory](https://feedback.azure.com/forums/169401-azure-active-directory/)论坛与我们联系。

包含有关组织品牌的详细信息。

组织可以自定义其 Azure AD 登录页，这些页面在用户登录到其组织的租户特定应用时显示，或者当 Azure AD 通过用户名标识用户的租户时显示。 开发人员还可以阅读公司的品牌信息并自定义其应用体验，以使用其公司品牌专门为登录用户定制它。

公司可以基于区域设置添加不同的品牌。 区域设置在所有请求中都用作键。

>**注意：** 品牌打造作为组织下具有特定于区域设置本地化的集合的属性公开。 **organizationalBrandingProperties** 是一个抽象类，用于定义 **organizationalBranding 的属性**。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 使用 organizationalBrandingProperties 对象创建组织品牌。 |
| [获取](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 读取 organizationalBrandingProperties 对象的属性和关系。 |
| [更新](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 更新 organizationalBrandingProperties 对象。 |
| [删除](../api/organizationalbrandingproperties-delete.md) | 无 | 删除 organizationalBrandingProperties 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|backgroundColor|String| 将出现在低带宽连接中的背景图像的颜色。 建议在此处使用横幅徽标或组织颜色的主要颜色。 以十六进制值指定 (，例如，白色#FFFFFF) 。 |
|backgroundImage|Stream| 显示为登录页背景的图像。 .png 或 .jpg 不大于 1920x1080 且小于 300kb。 较小的图像将降低带宽要求，使页面加载性能提高。 |
|bannerLogo|Stream| 显示在登录页面上的公司徽标的横幅版本。 .png 或 .jpg 不大于 36x245px。 我们建议使用透明图像，徽标周围没有填充。 |
|id|String| 这是一个继承自 microsoft.graph.entity 的 ID，是指定语言 ISO 639 标准（例如英语为"en-us"或"en"）区域设置。 今后，如果我们公开功能以针对一个区域设置具有多个品牌，则这一点可以更改。 请注意，默认 /branding 的 ID 始终为"und"，直到有无键单一的 ID。 只读。 |
|signInPageText|String| 显示在登录框底部的文本。 可以使用此信息向技术支持或法律声明传达其他信息，例如电话号码。 此文本必须是 Unicode 且不超过 1024 个字符。 |
|squareLogo|Stream| 公司徽标的方形版本。 这将显示在 Windows 10 现 (OOBE) 和启用 Windows Autopilot 进行部署时。 .png 或 .jpg 大小不超过 240x240px，大小不超过 10kb。 我们建议使用透明图像，徽标周围没有填充。 |
|usernameHintText|String| 在登录屏幕上的用户名文本框中作为提示的字符串。 此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。 |

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
