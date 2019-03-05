---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3e899f418ea9214530ac3b70e493a15655ca873
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167380"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="26895-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="26895-103">intuneBrand resource type</span></span>

> <span data-ttu-id="26895-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26895-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26895-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26895-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26895-106">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="26895-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="26895-107">属性</span><span class="sxs-lookup"><span data-stu-id="26895-107">Properties</span></span>
|<span data-ttu-id="26895-108">属性</span><span class="sxs-lookup"><span data-stu-id="26895-108">Property</span></span>|<span data-ttu-id="26895-109">类型</span><span class="sxs-lookup"><span data-stu-id="26895-109">Type</span></span>|<span data-ttu-id="26895-110">说明</span><span class="sxs-lookup"><span data-stu-id="26895-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26895-111">displayName</span><span class="sxs-lookup"><span data-stu-id="26895-111">displayName</span></span>|<span data-ttu-id="26895-112">字符串</span><span class="sxs-lookup"><span data-stu-id="26895-112">String</span></span>|<span data-ttu-id="26895-113">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="26895-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="26895-114">contactITName</span><span class="sxs-lookup"><span data-stu-id="26895-114">contactITName</span></span>|<span data-ttu-id="26895-115">String</span><span class="sxs-lookup"><span data-stu-id="26895-115">String</span></span>|<span data-ttu-id="26895-116">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="26895-116">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="26895-117">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="26895-117">contactITPhoneNumber</span></span>|<span data-ttu-id="26895-118">String</span><span class="sxs-lookup"><span data-stu-id="26895-118">String</span></span>|<span data-ttu-id="26895-119">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="26895-119">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="26895-120">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="26895-120">contactITEmailAddress</span></span>|<span data-ttu-id="26895-121">String</span><span class="sxs-lookup"><span data-stu-id="26895-121">String</span></span>|<span data-ttu-id="26895-122">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="26895-122">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="26895-123">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="26895-123">contactITNotes</span></span>|<span data-ttu-id="26895-124">String</span><span class="sxs-lookup"><span data-stu-id="26895-124">String</span></span>|<span data-ttu-id="26895-125">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="26895-125">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="26895-126">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="26895-126">privacyUrl</span></span>|<span data-ttu-id="26895-127">String</span><span class="sxs-lookup"><span data-stu-id="26895-127">String</span></span>|<span data-ttu-id="26895-128">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="26895-128">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="26895-129">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="26895-129">onlineSupportSiteUrl</span></span>|<span data-ttu-id="26895-130">String</span><span class="sxs-lookup"><span data-stu-id="26895-130">String</span></span>|<span data-ttu-id="26895-131">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="26895-131">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="26895-132">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="26895-132">onlineSupportSiteName</span></span>|<span data-ttu-id="26895-133">String</span><span class="sxs-lookup"><span data-stu-id="26895-133">String</span></span>|<span data-ttu-id="26895-134">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="26895-134">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="26895-135">themeColor</span><span class="sxs-lookup"><span data-stu-id="26895-135">themeColor</span></span>|[<span data-ttu-id="26895-136">rgbColor</span><span class="sxs-lookup"><span data-stu-id="26895-136">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="26895-137">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="26895-137">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="26895-138">showLogo</span><span class="sxs-lookup"><span data-stu-id="26895-138">showLogo</span></span>|<span data-ttu-id="26895-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="26895-139">Boolean</span></span>|<span data-ttu-id="26895-140">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26895-140">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="26895-141">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="26895-141">lightBackgroundLogo</span></span>|[<span data-ttu-id="26895-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26895-142">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26895-143">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="26895-143">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="26895-144">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="26895-144">darkBackgroundLogo</span></span>|[<span data-ttu-id="26895-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26895-145">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26895-146">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="26895-146">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="26895-147">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="26895-147">showNameNextToLogo</span></span>|<span data-ttu-id="26895-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="26895-148">Boolean</span></span>|<span data-ttu-id="26895-149">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26895-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="26895-150">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="26895-150">landingPageCustomizedImage</span></span>|[<span data-ttu-id="26895-151">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26895-151">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26895-152">在 Compnay 门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="26895-152">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="26895-153">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="26895-153">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="26895-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="26895-154">Boolean</span></span>|<span data-ttu-id="26895-155">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="26895-155">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26895-156">关系</span><span class="sxs-lookup"><span data-stu-id="26895-156">Relationships</span></span>
<span data-ttu-id="26895-157">无</span><span class="sxs-lookup"><span data-stu-id="26895-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26895-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26895-158">JSON Representation</span></span>
<span data-ttu-id="26895-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26895-159">Here is a JSON representation of the resource.</span></span>
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




