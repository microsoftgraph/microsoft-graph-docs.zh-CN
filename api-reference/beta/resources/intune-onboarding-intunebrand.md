---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4e1e4a4a4042b9a4dd9382f1310d737ac1c9678
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398602"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="df1ea-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="df1ea-103">intuneBrand resource type</span></span>

> <span data-ttu-id="df1ea-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="df1ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df1ea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df1ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df1ea-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df1ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df1ea-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="df1ea-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="df1ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="df1ea-108">Properties</span></span>
|<span data-ttu-id="df1ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="df1ea-109">Property</span></span>|<span data-ttu-id="df1ea-110">类型</span><span class="sxs-lookup"><span data-stu-id="df1ea-110">Type</span></span>|<span data-ttu-id="df1ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="df1ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df1ea-112">displayName</span><span class="sxs-lookup"><span data-stu-id="df1ea-112">displayName</span></span>|<span data-ttu-id="df1ea-113">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-113">String</span></span>|<span data-ttu-id="df1ea-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="df1ea-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="df1ea-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="df1ea-115">contactITName</span></span>|<span data-ttu-id="df1ea-116">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-116">String</span></span>|<span data-ttu-id="df1ea-117">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="df1ea-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df1ea-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="df1ea-118">contactITPhoneNumber</span></span>|<span data-ttu-id="df1ea-119">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-119">String</span></span>|<span data-ttu-id="df1ea-120">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="df1ea-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df1ea-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="df1ea-121">contactITEmailAddress</span></span>|<span data-ttu-id="df1ea-122">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-122">String</span></span>|<span data-ttu-id="df1ea-123">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="df1ea-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df1ea-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="df1ea-124">contactITNotes</span></span>|<span data-ttu-id="df1ea-125">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-125">String</span></span>|<span data-ttu-id="df1ea-126">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="df1ea-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="df1ea-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="df1ea-127">privacyUrl</span></span>|<span data-ttu-id="df1ea-128">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-128">String</span></span>|<span data-ttu-id="df1ea-129">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="df1ea-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="df1ea-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="df1ea-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="df1ea-131">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-131">String</span></span>|<span data-ttu-id="df1ea-132">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="df1ea-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="df1ea-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="df1ea-133">onlineSupportSiteName</span></span>|<span data-ttu-id="df1ea-134">String</span><span class="sxs-lookup"><span data-stu-id="df1ea-134">String</span></span>|<span data-ttu-id="df1ea-135">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="df1ea-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="df1ea-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="df1ea-136">themeColor</span></span>|[<span data-ttu-id="df1ea-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="df1ea-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="df1ea-138">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="df1ea-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="df1ea-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="df1ea-139">showLogo</span></span>|<span data-ttu-id="df1ea-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="df1ea-140">Boolean</span></span>|<span data-ttu-id="df1ea-141">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="df1ea-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="df1ea-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="df1ea-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="df1ea-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df1ea-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df1ea-144">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="df1ea-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="df1ea-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="df1ea-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="df1ea-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df1ea-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df1ea-147">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="df1ea-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="df1ea-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="df1ea-148">showNameNextToLogo</span></span>|<span data-ttu-id="df1ea-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="df1ea-149">Boolean</span></span>|<span data-ttu-id="df1ea-150">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="df1ea-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="df1ea-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="df1ea-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="df1ea-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df1ea-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df1ea-153">Compnay 门户应用程序登陆页面中显示的自定义的图像</span><span class="sxs-lookup"><span data-stu-id="df1ea-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="df1ea-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="df1ea-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="df1ea-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="df1ea-155">Boolean</span></span>|<span data-ttu-id="df1ea-156">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="df1ea-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df1ea-157">关系</span><span class="sxs-lookup"><span data-stu-id="df1ea-157">Relationships</span></span>
<span data-ttu-id="df1ea-158">无</span><span class="sxs-lookup"><span data-stu-id="df1ea-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df1ea-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df1ea-159">JSON Representation</span></span>
<span data-ttu-id="df1ea-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df1ea-160">Here is a JSON representation of the resource.</span></span>
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




