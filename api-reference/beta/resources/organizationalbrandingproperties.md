---
title: organizationalBrandingProperties 资源类型
description: 包含组织品牌打造的详细信息。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f68c33e7a3cf81e5d3debedcd6162ec59ddcce03
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266820"
---
# <a name="organizationalbrandingproperties-resource-type"></a><span data-ttu-id="c144c-103">organizationalBrandingProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="c144c-103">organizationalBrandingProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="c144c-104">添加自定义品牌打造需要你使用 Azure Active Directory Premium 1、Premium 2 或 Basic 版本，或者拥有 Microsoft 365 许可证。</span><span class="sxs-lookup"><span data-stu-id="c144c-104">Adding custom branding requires you to use Azure Active Directory Premium 1, Premium 2, or Basic editions, or to have a Microsoft 365 license.</span></span> <span data-ttu-id="c144c-105">有关许可和版本详细信息，请参阅注册 Azure [AD Premium。](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)</span><span class="sxs-lookup"><span data-stu-id="c144c-105">For more information about licensing and editions, see [Sign up for Azure AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).</span></span><br><br><span data-ttu-id="c144c-106">Azure AD Premium 和 Basic 版本适用于使用 Azure Active Directory 全球实例的中国客户。</span><span class="sxs-lookup"><span data-stu-id="c144c-106">Azure AD Premium and Basic editions are available for customers in China using the worldwide instance of Azure Active Directory.</span></span> <span data-ttu-id="c144c-107">Azure AD Premium 和 Basic 版本当前在由世纪网络在中国运营的 Azure 服务中不受支持。</span><span class="sxs-lookup"><span data-stu-id="c144c-107">Azure AD Premium and Basic editions aren't currently supported in the Azure service operated by 21Vianet in China.</span></span> <span data-ttu-id="c144c-108">有关详细信息，请通过 Azure Active [Directory](https://feedback.azure.com/forums/169401-azure-active-directory/)论坛与我们联系。</span><span class="sxs-lookup"><span data-stu-id="c144c-108">For more information, talk to us using the [Azure Active Directory Forum](https://feedback.azure.com/forums/169401-azure-active-directory/).</span></span>

<span data-ttu-id="c144c-109">包含有关组织品牌的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c144c-109">Contains details about the organization's branding.</span></span>

<span data-ttu-id="c144c-110">组织可以自定义其 Azure AD 登录页面，当用户登录到其组织的租户特定应用时，或者当 Azure AD 通过用户名标识用户的租户时，会显示这些页面。</span><span class="sxs-lookup"><span data-stu-id="c144c-110">Organizations can customize their Azure AD sign-in pages which appear when users sign in to their organization's tenant-specific apps, or when Azure AD identifies the user's tenant from their username.</span></span> <span data-ttu-id="c144c-111">开发人员还可以阅读公司的品牌信息并自定义其应用体验，以使用其公司的品牌专门为登录用户定制它。</span><span class="sxs-lookup"><span data-stu-id="c144c-111">A developer can also read the company's branding information and customize their app experience to tailor it specifically for the signed-in user using their company's branding.</span></span>

<span data-ttu-id="c144c-112">公司可以基于区域设置添加不同的品牌。</span><span class="sxs-lookup"><span data-stu-id="c144c-112">Companies can add different branding based on locale.</span></span> <span data-ttu-id="c144c-113">区域设置在所有请求中都用作键。</span><span class="sxs-lookup"><span data-stu-id="c144c-113">Locale serves as a key in all requests.</span></span>

><span data-ttu-id="c144c-114">**注意：** 品牌打造作为组织下的属性公开，具有特定于区域设置本地化的集合。</span><span class="sxs-lookup"><span data-stu-id="c144c-114">**Note:** Branding is exposed as a property under organization with a collection of locale-specific localizations.</span></span> <span data-ttu-id="c144c-115">**organizationalBrandingProperties** 是一个抽象类，用于定义 **organizationalBranding 的属性**。</span><span class="sxs-lookup"><span data-stu-id="c144c-115">**organizationalBrandingProperties** is an abstract class which defines properties for **organizationalBranding**.</span></span>

## <a name="methods"></a><span data-ttu-id="c144c-116">方法</span><span class="sxs-lookup"><span data-stu-id="c144c-116">Methods</span></span>

| <span data-ttu-id="c144c-117">方法</span><span class="sxs-lookup"><span data-stu-id="c144c-117">Method</span></span>       | <span data-ttu-id="c144c-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="c144c-118">Return Type</span></span> | <span data-ttu-id="c144c-119">说明</span><span class="sxs-lookup"><span data-stu-id="c144c-119">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c144c-120">创建</span><span class="sxs-lookup"><span data-stu-id="c144c-120">Create</span></span>](../api/organizationalbrandingproperties-create.md) | [<span data-ttu-id="c144c-121">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c144c-121">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="c144c-122">使用 organizationalBrandingProperties 对象创建组织品牌。</span><span class="sxs-lookup"><span data-stu-id="c144c-122">Create organizational branding with organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="c144c-123">获取</span><span class="sxs-lookup"><span data-stu-id="c144c-123">Get</span></span>](../api/organizationalbrandingproperties-get.md) | [<span data-ttu-id="c144c-124">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c144c-124">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="c144c-125">读取 organizationalBrandingProperties 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c144c-125">Read properties and relationships of organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="c144c-126">更新</span><span class="sxs-lookup"><span data-stu-id="c144c-126">Update</span></span>](../api/organizationalbrandingproperties-update.md) | [<span data-ttu-id="c144c-127">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c144c-127">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="c144c-128">更新 organizationalBrandingProperties 对象。</span><span class="sxs-lookup"><span data-stu-id="c144c-128">Update organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="c144c-129">删除</span><span class="sxs-lookup"><span data-stu-id="c144c-129">Delete</span></span>](../api/organizationalbrandingproperties-delete.md) | <span data-ttu-id="c144c-130">无</span><span class="sxs-lookup"><span data-stu-id="c144c-130">None</span></span> | <span data-ttu-id="c144c-131">删除 organizationalBrandingProperties 对象。</span><span class="sxs-lookup"><span data-stu-id="c144c-131">Delete organizationalBrandingProperties object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c144c-132">属性</span><span class="sxs-lookup"><span data-stu-id="c144c-132">Properties</span></span>

| <span data-ttu-id="c144c-133">属性</span><span class="sxs-lookup"><span data-stu-id="c144c-133">Property</span></span>     | <span data-ttu-id="c144c-134">类型</span><span class="sxs-lookup"><span data-stu-id="c144c-134">Type</span></span>        | <span data-ttu-id="c144c-135">说明</span><span class="sxs-lookup"><span data-stu-id="c144c-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c144c-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="c144c-136">backgroundColor</span></span>|<span data-ttu-id="c144c-137">String</span><span class="sxs-lookup"><span data-stu-id="c144c-137">String</span></span>| <span data-ttu-id="c144c-138">将出现在低带宽连接中的背景图像上的颜色。</span><span class="sxs-lookup"><span data-stu-id="c144c-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="c144c-139">建议在此处使用横幅徽标或组织颜色的主要颜色。</span><span class="sxs-lookup"><span data-stu-id="c144c-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="c144c-140">以十六进制表示 (，例如，白色#FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="c144c-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span> |
|<span data-ttu-id="c144c-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="c144c-141">backgroundImage</span></span>|<span data-ttu-id="c144c-142">Stream</span><span class="sxs-lookup"><span data-stu-id="c144c-142">Stream</span></span>| <span data-ttu-id="c144c-143">显示为登录页背景的图像。</span><span class="sxs-lookup"><span data-stu-id="c144c-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="c144c-144">.png或 .jpg不超过 1920x1080 且小于 300kb。</span><span class="sxs-lookup"><span data-stu-id="c144c-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="c144c-145">较小的图像将降低带宽要求，提高页面加载性能。</span><span class="sxs-lookup"><span data-stu-id="c144c-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span> |
|<span data-ttu-id="c144c-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="c144c-146">bannerLogo</span></span>|<span data-ttu-id="c144c-147">Stream</span><span class="sxs-lookup"><span data-stu-id="c144c-147">Stream</span></span>| <span data-ttu-id="c144c-148">显示在登录页上的公司徽标的横幅版本。</span><span class="sxs-lookup"><span data-stu-id="c144c-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="c144c-149">.png或.jpg不超过 36x245px。</span><span class="sxs-lookup"><span data-stu-id="c144c-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="c144c-150">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="c144c-150">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="c144c-151">id</span><span class="sxs-lookup"><span data-stu-id="c144c-151">id</span></span>|<span data-ttu-id="c144c-152">String</span><span class="sxs-lookup"><span data-stu-id="c144c-152">String</span></span>| <span data-ttu-id="c144c-153">这是一个继承自 microsoft.graph.entity 的 id，是指定语言 ISO 639 标准（例如英语为"en-us"或"en"）区域设置。</span><span class="sxs-lookup"><span data-stu-id="c144c-153">This is an id, inherited from microsoft.graph.entity, is the locale specifying the ISO 639 standard for language, for example English is "en-us" or "en".</span></span> <span data-ttu-id="c144c-154">今后，如果我们公开功能以针对一个区域设置具有多个品牌，这一点可能会更改。</span><span class="sxs-lookup"><span data-stu-id="c144c-154">Going forward if we expose functionality to have multiple brandings for one locale, this can be changed.</span></span> <span data-ttu-id="c144c-155">请注意，默认 /branding 的 ID 始终为"und"，直到我们具有无键单一性。</span><span class="sxs-lookup"><span data-stu-id="c144c-155">Note that id for Default /branding is always 'und' until we have keyless singletons.</span></span> <span data-ttu-id="c144c-156">只读。</span><span class="sxs-lookup"><span data-stu-id="c144c-156">Read-only.</span></span> |
|<span data-ttu-id="c144c-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="c144c-157">signInPageText</span></span>|<span data-ttu-id="c144c-158">String</span><span class="sxs-lookup"><span data-stu-id="c144c-158">String</span></span>| <span data-ttu-id="c144c-159">显示在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="c144c-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="c144c-160">您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="c144c-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="c144c-161">此文本必须是 Unicode 且不超过 1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="c144c-161">This text must be Unicode and not exceed 1024 characters.</span></span> |
|<span data-ttu-id="c144c-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="c144c-162">squareLogo</span></span>|<span data-ttu-id="c144c-163">Stream</span><span class="sxs-lookup"><span data-stu-id="c144c-163">Stream</span></span>| <span data-ttu-id="c144c-164">公司徽标的方形版本。</span><span class="sxs-lookup"><span data-stu-id="c144c-164">Square version of your company logo.</span></span> <span data-ttu-id="c144c-165">这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。</span><span class="sxs-lookup"><span data-stu-id="c144c-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="c144c-166">.png或 .jpg不超过 240x240px 且大小不超过 10kb。</span><span class="sxs-lookup"><span data-stu-id="c144c-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="c144c-167">我们建议使用透明图像，徽标周围没有填充。</span><span class="sxs-lookup"><span data-stu-id="c144c-167">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="c144c-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="c144c-168">usernameHintText</span></span>|<span data-ttu-id="c144c-169">String</span><span class="sxs-lookup"><span data-stu-id="c144c-169">String</span></span>| <span data-ttu-id="c144c-170">字符串，在登录屏幕的用户名文本框中作为提示显示。</span><span class="sxs-lookup"><span data-stu-id="c144c-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="c144c-171">此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="c144c-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c144c-172">关系</span><span class="sxs-lookup"><span data-stu-id="c144c-172">Relationships</span></span>

<span data-ttu-id="c144c-173">无</span><span class="sxs-lookup"><span data-stu-id="c144c-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c144c-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c144c-174">JSON representation</span></span>

<span data-ttu-id="c144c-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c144c-175">The following is a JSON representation of the resource.</span></span>

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
