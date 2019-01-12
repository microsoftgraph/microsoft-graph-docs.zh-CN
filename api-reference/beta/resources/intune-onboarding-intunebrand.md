---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab8465390b6b0a9e4f35e8a713f082dfb9325eb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957681"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="1c526-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c526-103">intuneBrand resource type</span></span>

> <span data-ttu-id="1c526-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c526-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c526-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c526-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c526-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c526-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c526-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="1c526-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="1c526-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c526-108">Properties</span></span>
|<span data-ttu-id="1c526-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c526-109">Property</span></span>|<span data-ttu-id="1c526-110">类型</span><span class="sxs-lookup"><span data-stu-id="1c526-110">Type</span></span>|<span data-ttu-id="1c526-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c526-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c526-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1c526-112">displayName</span></span>|<span data-ttu-id="1c526-113">String</span><span class="sxs-lookup"><span data-stu-id="1c526-113">String</span></span>|<span data-ttu-id="1c526-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="1c526-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="1c526-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="1c526-115">contactITName</span></span>|<span data-ttu-id="1c526-116">String</span><span class="sxs-lookup"><span data-stu-id="1c526-116">String</span></span>|<span data-ttu-id="1c526-117">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="1c526-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1c526-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1c526-118">contactITPhoneNumber</span></span>|<span data-ttu-id="1c526-119">String</span><span class="sxs-lookup"><span data-stu-id="1c526-119">String</span></span>|<span data-ttu-id="1c526-120">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="1c526-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1c526-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1c526-121">contactITEmailAddress</span></span>|<span data-ttu-id="1c526-122">String</span><span class="sxs-lookup"><span data-stu-id="1c526-122">String</span></span>|<span data-ttu-id="1c526-123">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1c526-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1c526-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="1c526-124">contactITNotes</span></span>|<span data-ttu-id="1c526-125">String</span><span class="sxs-lookup"><span data-stu-id="1c526-125">String</span></span>|<span data-ttu-id="1c526-126">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="1c526-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="1c526-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="1c526-127">privacyUrl</span></span>|<span data-ttu-id="1c526-128">String</span><span class="sxs-lookup"><span data-stu-id="1c526-128">String</span></span>|<span data-ttu-id="1c526-129">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="1c526-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="1c526-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="1c526-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="1c526-131">String</span><span class="sxs-lookup"><span data-stu-id="1c526-131">String</span></span>|<span data-ttu-id="1c526-132">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="1c526-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1c526-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="1c526-133">onlineSupportSiteName</span></span>|<span data-ttu-id="1c526-134">String</span><span class="sxs-lookup"><span data-stu-id="1c526-134">String</span></span>|<span data-ttu-id="1c526-135">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="1c526-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="1c526-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="1c526-136">themeColor</span></span>|[<span data-ttu-id="1c526-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="1c526-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="1c526-138">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="1c526-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="1c526-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="1c526-139">showLogo</span></span>|<span data-ttu-id="1c526-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="1c526-140">Boolean</span></span>|<span data-ttu-id="1c526-141">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1c526-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="1c526-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1c526-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="1c526-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1c526-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1c526-144">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="1c526-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="1c526-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="1c526-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="1c526-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1c526-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1c526-147">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="1c526-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="1c526-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1c526-148">showNameNextToLogo</span></span>|<span data-ttu-id="1c526-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="1c526-149">Boolean</span></span>|<span data-ttu-id="1c526-150">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1c526-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="1c526-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="1c526-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="1c526-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1c526-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1c526-153">Compnay 门户应用程序登陆页面中显示的自定义的图像</span><span class="sxs-lookup"><span data-stu-id="1c526-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="1c526-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="1c526-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="1c526-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="1c526-155">Boolean</span></span>|<span data-ttu-id="1c526-156">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1c526-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c526-157">关系</span><span class="sxs-lookup"><span data-stu-id="1c526-157">Relationships</span></span>
<span data-ttu-id="1c526-158">无</span><span class="sxs-lookup"><span data-stu-id="1c526-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c526-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c526-159">JSON Representation</span></span>
<span data-ttu-id="1c526-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c526-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
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
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true
}
```





