---
title: organizationalBrandingProperties 资源类型
description: 包含组织品牌的详细信息。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b96d4453f07ce317eb41902ed33282d961c74f16
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031903"
---
# <a name="organizationalbrandingproperties-resource-type"></a>organizationalBrandingProperties 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>若要添加自定义品牌打造，需要使用 Azure Active Directory Premium 1、Premium 2 或 Basic 版本，或者使用 Microsoft 365 许可证。 有关许可和版本的详细信息，请参阅 [注册 AZURE AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)。<br><br>Azure AD Premium 和 Basic 版本可供中国的客户使用 Azure Active Directory 的全球实例。 在中国由世纪互联运营的 Azure 服务中目前不支持 azure AD Premium 和基本版。 有关详细信息，请使用 [Azure Active Directory 论坛](https://feedback.azure.com/forums/169401-azure-active-directory/)与我们联系。

包含有关组织品牌的详细信息。

组织可以自定义其 Azure AD 登录页面，当用户登录到组织的特定租户应用程序时，或者当 Azure AD 从用户名中标识用户的租户时，将显示这些页面。 开发人员还可以阅读公司的品牌打造信息并自定义其应用程序体验，以使用其公司品牌专门针对登录用户进行量身定制。

公司可以根据区域设置添加不同品牌。 区域设置充当所有请求中的密钥。

>**注意：** 品牌化作为 "组织中的属性" 公开为特定于区域设置的 localizations 的集合。 **organizationalBrandingProperties** 是一个定义 **organizationalBranding** 属性的抽象类。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 创建具有 organizationalBrandingProperties 对象的组织品牌。 |
| [获取](../api/organizationalbrandingproperties-get.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 读取 organizationalBrandingProperties 对象的属性和关系。 |
| [更新](../api/organizationalbrandingproperties-update.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | 更新 organizationalBrandingProperties 对象。 |
| [删除](../api/organizationalbrandingproperties-delete.md) | 无 | 删除 organizationalBrandingProperties 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|backgroundColor|String| 将在低带宽连接中的背景图像处显示的颜色。 建议在此处使用横幅徽标的主要颜色或您的组织颜色。 在十六进制 (中指定此项例如，白色为 #FFFFFF) 。 |
|backgroundImage|Stream| 显示为登录页的背景的图像。 .png 或 .jpg 不大于1920x1080 且小于300kb。 较小的图像将降低带宽要求并使页面加载更具性能。 |
|bannerLogo|Stream| 显示在登录页面上的公司徽标的标题版本。 .png 或 .jpg 不大于36x245px。 我们建议使用透明图像，而不在徽标周围进行填充。 |
|id|String| 这是一个从 microsoft. entity 继承的 id，是指定语言的 ISO 639 标准的区域设置，例如英语为 "en-us" 或 "en"。 如果我们公开功能对一个区域设置具有多个 brandings，则会进行转发，这可以更改。 请注意，默认/branding 的 id 始终为 "und"，直到我们有 keyless singletons。 只读。 |
|signInPageText|String| 出现在登录框底部的文本。 您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。 此文本必须是 Unicode，且不能超过1024个字符。 |
|squareLogo|Stream| 公司徽标的平方版本。 在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。 .png 或 .jpg 不大于240x240px，且大小不超过10kb。 我们建议使用透明图像，而不在徽标周围进行填充。 |
|usernameHintText|String| 在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。 此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "baseType": "",
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
