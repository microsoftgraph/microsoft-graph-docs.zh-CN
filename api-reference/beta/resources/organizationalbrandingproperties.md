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
# <a name="organizationalbrandingproperties-resource-type"></a><span data-ttu-id="65012-103">organizationalBrandingProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="65012-103">organizationalBrandingProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="65012-104">若要添加自定义品牌打造，需要使用 Azure Active Directory Premium 1、Premium 2 或 Basic 版本，或者使用 Microsoft 365 许可证。</span><span class="sxs-lookup"><span data-stu-id="65012-104">Adding custom branding requires you to use Azure Active Directory Premium 1, Premium 2, or Basic editions, or to have a Microsoft 365 license.</span></span> <span data-ttu-id="65012-105">有关许可和版本的详细信息，请参阅 [注册 AZURE AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)。</span><span class="sxs-lookup"><span data-stu-id="65012-105">For more information about licensing and editions, see [Sign up for Azure AD Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).</span></span><br><br><span data-ttu-id="65012-106">Azure AD Premium 和 Basic 版本可供中国的客户使用 Azure Active Directory 的全球实例。</span><span class="sxs-lookup"><span data-stu-id="65012-106">Azure AD Premium and Basic editions are available for customers in China using the worldwide instance of Azure Active Directory.</span></span> <span data-ttu-id="65012-107">在中国由世纪互联运营的 Azure 服务中目前不支持 azure AD Premium 和基本版。</span><span class="sxs-lookup"><span data-stu-id="65012-107">Azure AD Premium and Basic editions aren't currently supported in the Azure service operated by 21Vianet in China.</span></span> <span data-ttu-id="65012-108">有关详细信息，请使用 [Azure Active Directory 论坛](https://feedback.azure.com/forums/169401-azure-active-directory/)与我们联系。</span><span class="sxs-lookup"><span data-stu-id="65012-108">For more information, talk to us using the [Azure Active Directory Forum](https://feedback.azure.com/forums/169401-azure-active-directory/).</span></span>

<span data-ttu-id="65012-109">包含有关组织品牌的详细信息。</span><span class="sxs-lookup"><span data-stu-id="65012-109">Contains details about the organization's branding.</span></span>

<span data-ttu-id="65012-110">组织可以自定义其 Azure AD 登录页面，当用户登录到组织的特定租户应用程序时，或者当 Azure AD 从用户名中标识用户的租户时，将显示这些页面。</span><span class="sxs-lookup"><span data-stu-id="65012-110">Organizations can customize their Azure AD sign-in pages which appear when users sign in to their organization's tenant-specific apps, or when Azure AD identifies the user's tenant from their username.</span></span> <span data-ttu-id="65012-111">开发人员还可以阅读公司的品牌打造信息并自定义其应用程序体验，以使用其公司品牌专门针对登录用户进行量身定制。</span><span class="sxs-lookup"><span data-stu-id="65012-111">A developer can also read the company's branding information and customize their app experience to tailor it specifically for the signed-in user using their company's branding.</span></span>

<span data-ttu-id="65012-112">公司可以根据区域设置添加不同品牌。</span><span class="sxs-lookup"><span data-stu-id="65012-112">Companies can add different branding based on locale.</span></span> <span data-ttu-id="65012-113">区域设置充当所有请求中的密钥。</span><span class="sxs-lookup"><span data-stu-id="65012-113">Locale serves as a key in all requests.</span></span>

><span data-ttu-id="65012-114">**注意：** 品牌化作为 "组织中的属性" 公开为特定于区域设置的 localizations 的集合。</span><span class="sxs-lookup"><span data-stu-id="65012-114">**Note:** Branding is exposed as a property under organization with a collection of locale-specific localizations.</span></span> <span data-ttu-id="65012-115">**organizationalBrandingProperties** 是一个定义 **organizationalBranding** 属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="65012-115">**organizationalBrandingProperties** is an abstract class which defines properties for **organizationalBranding**.</span></span>

## <a name="methods"></a><span data-ttu-id="65012-116">方法</span><span class="sxs-lookup"><span data-stu-id="65012-116">Methods</span></span>

| <span data-ttu-id="65012-117">方法</span><span class="sxs-lookup"><span data-stu-id="65012-117">Method</span></span>       | <span data-ttu-id="65012-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="65012-118">Return Type</span></span> | <span data-ttu-id="65012-119">说明</span><span class="sxs-lookup"><span data-stu-id="65012-119">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="65012-120">创建</span><span class="sxs-lookup"><span data-stu-id="65012-120">Create</span></span>](../api/organizationalbrandingproperties-create.md) | [<span data-ttu-id="65012-121">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="65012-121">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="65012-122">创建具有 organizationalBrandingProperties 对象的组织品牌。</span><span class="sxs-lookup"><span data-stu-id="65012-122">Create organizational branding with organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="65012-123">获取</span><span class="sxs-lookup"><span data-stu-id="65012-123">Get</span></span>](../api/organizationalbrandingproperties-get.md) | [<span data-ttu-id="65012-124">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="65012-124">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="65012-125">读取 organizationalBrandingProperties 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65012-125">Read properties and relationships of organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="65012-126">更新</span><span class="sxs-lookup"><span data-stu-id="65012-126">Update</span></span>](../api/organizationalbrandingproperties-update.md) | [<span data-ttu-id="65012-127">organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="65012-127">organizationalBrandingProperties</span></span>](organizationalbrandingproperties.md) | <span data-ttu-id="65012-128">更新 organizationalBrandingProperties 对象。</span><span class="sxs-lookup"><span data-stu-id="65012-128">Update organizationalBrandingProperties object.</span></span> |
| [<span data-ttu-id="65012-129">删除</span><span class="sxs-lookup"><span data-stu-id="65012-129">Delete</span></span>](../api/organizationalbrandingproperties-delete.md) | <span data-ttu-id="65012-130">无</span><span class="sxs-lookup"><span data-stu-id="65012-130">None</span></span> | <span data-ttu-id="65012-131">删除 organizationalBrandingProperties 对象。</span><span class="sxs-lookup"><span data-stu-id="65012-131">Delete organizationalBrandingProperties object.</span></span> |

## <a name="properties"></a><span data-ttu-id="65012-132">属性</span><span class="sxs-lookup"><span data-stu-id="65012-132">Properties</span></span>

| <span data-ttu-id="65012-133">属性</span><span class="sxs-lookup"><span data-stu-id="65012-133">Property</span></span>     | <span data-ttu-id="65012-134">类型</span><span class="sxs-lookup"><span data-stu-id="65012-134">Type</span></span>        | <span data-ttu-id="65012-135">Description</span><span class="sxs-lookup"><span data-stu-id="65012-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65012-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="65012-136">backgroundColor</span></span>|<span data-ttu-id="65012-137">String</span><span class="sxs-lookup"><span data-stu-id="65012-137">String</span></span>| <span data-ttu-id="65012-138">将在低带宽连接中的背景图像处显示的颜色。</span><span class="sxs-lookup"><span data-stu-id="65012-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="65012-139">建议在此处使用横幅徽标的主要颜色或您的组织颜色。</span><span class="sxs-lookup"><span data-stu-id="65012-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="65012-140">在十六进制 (中指定此项例如，白色为 #FFFFFF) 。</span><span class="sxs-lookup"><span data-stu-id="65012-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span> |
|<span data-ttu-id="65012-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="65012-141">backgroundImage</span></span>|<span data-ttu-id="65012-142">Stream</span><span class="sxs-lookup"><span data-stu-id="65012-142">Stream</span></span>| <span data-ttu-id="65012-143">显示为登录页的背景的图像。</span><span class="sxs-lookup"><span data-stu-id="65012-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="65012-144">.png 或 .jpg 不大于1920x1080 且小于300kb。</span><span class="sxs-lookup"><span data-stu-id="65012-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="65012-145">较小的图像将降低带宽要求并使页面加载更具性能。</span><span class="sxs-lookup"><span data-stu-id="65012-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span> |
|<span data-ttu-id="65012-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="65012-146">bannerLogo</span></span>|<span data-ttu-id="65012-147">Stream</span><span class="sxs-lookup"><span data-stu-id="65012-147">Stream</span></span>| <span data-ttu-id="65012-148">显示在登录页面上的公司徽标的标题版本。</span><span class="sxs-lookup"><span data-stu-id="65012-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="65012-149">.png 或 .jpg 不大于36x245px。</span><span class="sxs-lookup"><span data-stu-id="65012-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="65012-150">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="65012-150">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="65012-151">id</span><span class="sxs-lookup"><span data-stu-id="65012-151">id</span></span>|<span data-ttu-id="65012-152">String</span><span class="sxs-lookup"><span data-stu-id="65012-152">String</span></span>| <span data-ttu-id="65012-153">这是一个从 microsoft. entity 继承的 id，是指定语言的 ISO 639 标准的区域设置，例如英语为 "en-us" 或 "en"。</span><span class="sxs-lookup"><span data-stu-id="65012-153">This is an id, inherited from microsoft.graph.entity, is the locale specifying the ISO 639 standard for language, for example English is "en-us" or "en".</span></span> <span data-ttu-id="65012-154">如果我们公开功能对一个区域设置具有多个 brandings，则会进行转发，这可以更改。</span><span class="sxs-lookup"><span data-stu-id="65012-154">Going forward if we expose functionality to have multiple brandings for one locale, this can be changed.</span></span> <span data-ttu-id="65012-155">请注意，默认/branding 的 id 始终为 "und"，直到我们有 keyless singletons。</span><span class="sxs-lookup"><span data-stu-id="65012-155">Note that id for Default /branding is always 'und' until we have keyless singletons.</span></span> <span data-ttu-id="65012-156">只读。</span><span class="sxs-lookup"><span data-stu-id="65012-156">Read-only.</span></span> |
|<span data-ttu-id="65012-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="65012-157">signInPageText</span></span>|<span data-ttu-id="65012-158">String</span><span class="sxs-lookup"><span data-stu-id="65012-158">String</span></span>| <span data-ttu-id="65012-159">出现在登录框底部的文本。</span><span class="sxs-lookup"><span data-stu-id="65012-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="65012-160">您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。</span><span class="sxs-lookup"><span data-stu-id="65012-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="65012-161">此文本必须是 Unicode，且不能超过1024个字符。</span><span class="sxs-lookup"><span data-stu-id="65012-161">This text must be Unicode and not exceed 1024 characters.</span></span> |
|<span data-ttu-id="65012-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="65012-162">squareLogo</span></span>|<span data-ttu-id="65012-163">Stream</span><span class="sxs-lookup"><span data-stu-id="65012-163">Stream</span></span>| <span data-ttu-id="65012-164">公司徽标的平方版本。</span><span class="sxs-lookup"><span data-stu-id="65012-164">Square version of your company logo.</span></span> <span data-ttu-id="65012-165">在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。</span><span class="sxs-lookup"><span data-stu-id="65012-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="65012-166">.png 或 .jpg 不大于240x240px，且大小不超过10kb。</span><span class="sxs-lookup"><span data-stu-id="65012-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="65012-167">我们建议使用透明图像，而不在徽标周围进行填充。</span><span class="sxs-lookup"><span data-stu-id="65012-167">We recommend using a transparent image with no padding around the logo.</span></span> |
|<span data-ttu-id="65012-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="65012-168">usernameHintText</span></span>|<span data-ttu-id="65012-169">String</span><span class="sxs-lookup"><span data-stu-id="65012-169">String</span></span>| <span data-ttu-id="65012-170">在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。</span><span class="sxs-lookup"><span data-stu-id="65012-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="65012-171">此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。</span><span class="sxs-lookup"><span data-stu-id="65012-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span> |

## <a name="relationships"></a><span data-ttu-id="65012-172">关系</span><span class="sxs-lookup"><span data-stu-id="65012-172">Relationships</span></span>

<span data-ttu-id="65012-173">无</span><span class="sxs-lookup"><span data-stu-id="65012-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65012-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65012-174">JSON representation</span></span>

<span data-ttu-id="65012-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65012-175">The following is a JSON representation of the resource.</span></span>

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
