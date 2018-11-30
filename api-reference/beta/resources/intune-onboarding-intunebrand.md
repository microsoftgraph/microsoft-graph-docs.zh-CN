---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
ms.openlocfilehash: b8ed558e2be032110470cc4e2c64d27d8011af1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047180"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="d1579-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1579-103">intuneBrand resource type</span></span>

> <span data-ttu-id="d1579-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1579-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1579-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1579-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1579-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d1579-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1579-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="d1579-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="d1579-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1579-108">Properties</span></span>
|<span data-ttu-id="d1579-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1579-109">Property</span></span>|<span data-ttu-id="d1579-110">类型</span><span class="sxs-lookup"><span data-stu-id="d1579-110">Type</span></span>|<span data-ttu-id="d1579-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1579-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1579-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d1579-112">displayName</span></span>|<span data-ttu-id="d1579-113">String</span><span class="sxs-lookup"><span data-stu-id="d1579-113">String</span></span>|<span data-ttu-id="d1579-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="d1579-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="d1579-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="d1579-115">contactITName</span></span>|<span data-ttu-id="d1579-116">String</span><span class="sxs-lookup"><span data-stu-id="d1579-116">String</span></span>|<span data-ttu-id="d1579-117">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="d1579-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d1579-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d1579-118">contactITPhoneNumber</span></span>|<span data-ttu-id="d1579-119">String</span><span class="sxs-lookup"><span data-stu-id="d1579-119">String</span></span>|<span data-ttu-id="d1579-120">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="d1579-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d1579-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d1579-121">contactITEmailAddress</span></span>|<span data-ttu-id="d1579-122">String</span><span class="sxs-lookup"><span data-stu-id="d1579-122">String</span></span>|<span data-ttu-id="d1579-123">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d1579-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d1579-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="d1579-124">contactITNotes</span></span>|<span data-ttu-id="d1579-125">String</span><span class="sxs-lookup"><span data-stu-id="d1579-125">String</span></span>|<span data-ttu-id="d1579-126">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="d1579-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="d1579-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="d1579-127">privacyUrl</span></span>|<span data-ttu-id="d1579-128">String</span><span class="sxs-lookup"><span data-stu-id="d1579-128">String</span></span>|<span data-ttu-id="d1579-129">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="d1579-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="d1579-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="d1579-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="d1579-131">String</span><span class="sxs-lookup"><span data-stu-id="d1579-131">String</span></span>|<span data-ttu-id="d1579-132">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="d1579-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="d1579-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="d1579-133">onlineSupportSiteName</span></span>|<span data-ttu-id="d1579-134">String</span><span class="sxs-lookup"><span data-stu-id="d1579-134">String</span></span>|<span data-ttu-id="d1579-135">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="d1579-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="d1579-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="d1579-136">themeColor</span></span>|[<span data-ttu-id="d1579-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="d1579-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="d1579-138">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="d1579-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="d1579-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="d1579-139">showLogo</span></span>|<span data-ttu-id="d1579-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="d1579-140">Boolean</span></span>|<span data-ttu-id="d1579-141">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d1579-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="d1579-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="d1579-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="d1579-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d1579-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d1579-144">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="d1579-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="d1579-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="d1579-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="d1579-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d1579-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d1579-147">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="d1579-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="d1579-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="d1579-148">showNameNextToLogo</span></span>|<span data-ttu-id="d1579-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="d1579-149">Boolean</span></span>|<span data-ttu-id="d1579-150">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d1579-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="d1579-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="d1579-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="d1579-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d1579-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d1579-153">Compnay 门户应用程序登陆页面中显示的自定义的图像</span><span class="sxs-lookup"><span data-stu-id="d1579-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="d1579-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="d1579-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="d1579-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="d1579-155">Boolean</span></span>|<span data-ttu-id="d1579-156">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d1579-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1579-157">关系</span><span class="sxs-lookup"><span data-stu-id="d1579-157">Relationships</span></span>
<span data-ttu-id="d1579-158">无</span><span class="sxs-lookup"><span data-stu-id="d1579-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1579-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1579-159">JSON Representation</span></span>
<span data-ttu-id="d1579-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1579-160">Here is a JSON representation of the resource.</span></span>
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





