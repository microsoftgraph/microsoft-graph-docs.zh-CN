---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 062a42cced84afc4205e4f78511a5cf058da8626
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066381"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="c7662-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7662-103">intuneBrand resource type</span></span>

<span data-ttu-id="c7662-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7662-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7662-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7662-106">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="c7662-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="c7662-107">属性</span><span class="sxs-lookup"><span data-stu-id="c7662-107">Properties</span></span>
|<span data-ttu-id="c7662-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7662-108">Property</span></span>|<span data-ttu-id="c7662-109">类型</span><span class="sxs-lookup"><span data-stu-id="c7662-109">Type</span></span>|<span data-ttu-id="c7662-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7662-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7662-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c7662-111">displayName</span></span>|<span data-ttu-id="c7662-112">String</span><span class="sxs-lookup"><span data-stu-id="c7662-112">String</span></span>|<span data-ttu-id="c7662-113">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="c7662-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="c7662-114">contactITName</span><span class="sxs-lookup"><span data-stu-id="c7662-114">contactITName</span></span>|<span data-ttu-id="c7662-115">String</span><span class="sxs-lookup"><span data-stu-id="c7662-115">String</span></span>|<span data-ttu-id="c7662-116">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="c7662-116">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c7662-117">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c7662-117">contactITPhoneNumber</span></span>|<span data-ttu-id="c7662-118">String</span><span class="sxs-lookup"><span data-stu-id="c7662-118">String</span></span>|<span data-ttu-id="c7662-119">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c7662-119">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c7662-120">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c7662-120">contactITEmailAddress</span></span>|<span data-ttu-id="c7662-121">String</span><span class="sxs-lookup"><span data-stu-id="c7662-121">String</span></span>|<span data-ttu-id="c7662-122">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c7662-122">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c7662-123">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="c7662-123">contactITNotes</span></span>|<span data-ttu-id="c7662-124">String</span><span class="sxs-lookup"><span data-stu-id="c7662-124">String</span></span>|<span data-ttu-id="c7662-125">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="c7662-125">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c7662-126">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="c7662-126">privacyUrl</span></span>|<span data-ttu-id="c7662-127">String</span><span class="sxs-lookup"><span data-stu-id="c7662-127">String</span></span>|<span data-ttu-id="c7662-128">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="c7662-128">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="c7662-129">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c7662-129">onlineSupportSiteUrl</span></span>|<span data-ttu-id="c7662-130">String</span><span class="sxs-lookup"><span data-stu-id="c7662-130">String</span></span>|<span data-ttu-id="c7662-131">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="c7662-131">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c7662-132">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="c7662-132">onlineSupportSiteName</span></span>|<span data-ttu-id="c7662-133">String</span><span class="sxs-lookup"><span data-stu-id="c7662-133">String</span></span>|<span data-ttu-id="c7662-134">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="c7662-134">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c7662-135">themeColor</span><span class="sxs-lookup"><span data-stu-id="c7662-135">themeColor</span></span>|[<span data-ttu-id="c7662-136">rgbColor</span><span class="sxs-lookup"><span data-stu-id="c7662-136">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="c7662-137">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="c7662-137">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="c7662-138">showLogo</span><span class="sxs-lookup"><span data-stu-id="c7662-138">showLogo</span></span>|<span data-ttu-id="c7662-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="c7662-139">Boolean</span></span>|<span data-ttu-id="c7662-140">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c7662-140">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="c7662-141">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c7662-141">lightBackgroundLogo</span></span>|[<span data-ttu-id="c7662-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c7662-142">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c7662-143">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="c7662-143">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="c7662-144">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c7662-144">darkBackgroundLogo</span></span>|[<span data-ttu-id="c7662-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c7662-145">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c7662-146">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="c7662-146">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="c7662-147">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c7662-147">showNameNextToLogo</span></span>|<span data-ttu-id="c7662-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="c7662-148">Boolean</span></span>|<span data-ttu-id="c7662-149">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c7662-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c7662-150">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c7662-150">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="c7662-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="c7662-151">Boolean</span></span>|<span data-ttu-id="c7662-152">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c7662-152">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7662-153">关系</span><span class="sxs-lookup"><span data-stu-id="c7662-153">Relationships</span></span>
<span data-ttu-id="c7662-154">无</span><span class="sxs-lookup"><span data-stu-id="c7662-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7662-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7662-155">JSON Representation</span></span>
<span data-ttu-id="c7662-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7662-156">Here is a JSON representation of the resource.</span></span>
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
  "showDisplayNameNextToLogo": true
}
```









