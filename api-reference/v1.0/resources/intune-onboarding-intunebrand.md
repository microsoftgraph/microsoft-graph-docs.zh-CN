---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 346966fdcb3cfc8b3c4c24e55f4a07e46c97a612
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751270"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="c3da8-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3da8-103">intuneBrand resource type</span></span>

<span data-ttu-id="c3da8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3da8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3da8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3da8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3da8-106">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="c3da8-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="c3da8-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3da8-107">Properties</span></span>
|<span data-ttu-id="c3da8-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3da8-108">Property</span></span>|<span data-ttu-id="c3da8-109">类型</span><span class="sxs-lookup"><span data-stu-id="c3da8-109">Type</span></span>|<span data-ttu-id="c3da8-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3da8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3da8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c3da8-111">displayName</span></span>|<span data-ttu-id="c3da8-112">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-112">String</span></span>|<span data-ttu-id="c3da8-113">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="c3da8-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="c3da8-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="c3da8-114">themeColor</span></span>|[<span data-ttu-id="c3da8-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="c3da8-115">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="c3da8-116">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="c3da8-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="c3da8-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="c3da8-117">showLogo</span></span>|<span data-ttu-id="c3da8-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="c3da8-118">Boolean</span></span>|<span data-ttu-id="c3da8-119">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c3da8-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="c3da8-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c3da8-120">lightBackgroundLogo</span></span>|[<span data-ttu-id="c3da8-121">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3da8-121">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3da8-122">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="c3da8-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="c3da8-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="c3da8-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="c3da8-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3da8-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3da8-125">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="c3da8-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="c3da8-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c3da8-126">showNameNextToLogo</span></span>|<span data-ttu-id="c3da8-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="c3da8-127">Boolean</span></span>|<span data-ttu-id="c3da8-128">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c3da8-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c3da8-129">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="c3da8-129">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="c3da8-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="c3da8-130">Boolean</span></span>|<span data-ttu-id="c3da8-131">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c3da8-131">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="c3da8-132">contactITName</span><span class="sxs-lookup"><span data-stu-id="c3da8-132">contactITName</span></span>|<span data-ttu-id="c3da8-133">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-133">String</span></span>|<span data-ttu-id="c3da8-134">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="c3da8-134">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c3da8-135">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c3da8-135">contactITPhoneNumber</span></span>|<span data-ttu-id="c3da8-136">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-136">String</span></span>|<span data-ttu-id="c3da8-137">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c3da8-137">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c3da8-138">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c3da8-138">contactITEmailAddress</span></span>|<span data-ttu-id="c3da8-139">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-139">String</span></span>|<span data-ttu-id="c3da8-140">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c3da8-140">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c3da8-141">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="c3da8-141">contactITNotes</span></span>|<span data-ttu-id="c3da8-142">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-142">String</span></span>|<span data-ttu-id="c3da8-143">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="c3da8-143">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="c3da8-144">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c3da8-144">onlineSupportSiteUrl</span></span>|<span data-ttu-id="c3da8-145">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-145">String</span></span>|<span data-ttu-id="c3da8-146">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="c3da8-146">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c3da8-147">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="c3da8-147">onlineSupportSiteName</span></span>|<span data-ttu-id="c3da8-148">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-148">String</span></span>|<span data-ttu-id="c3da8-149">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="c3da8-149">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="c3da8-150">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="c3da8-150">privacyUrl</span></span>|<span data-ttu-id="c3da8-151">String</span><span class="sxs-lookup"><span data-stu-id="c3da8-151">String</span></span>|<span data-ttu-id="c3da8-152">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="c3da8-152">URL to the company/organization’s privacy policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3da8-153">关系</span><span class="sxs-lookup"><span data-stu-id="c3da8-153">Relationships</span></span>
<span data-ttu-id="c3da8-154">无</span><span class="sxs-lookup"><span data-stu-id="c3da8-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3da8-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3da8-155">JSON Representation</span></span>
<span data-ttu-id="c3da8-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3da8-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
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
  "showDisplayNameNextToLogo": true,
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String"
}
```




