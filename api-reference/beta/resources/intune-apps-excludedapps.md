---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e391c713324b69747e0528285580e3300e71868
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459102"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="9e1d4-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e1d4-103">excludedApps resource type</span></span>

<span data-ttu-id="9e1d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e1d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e1d4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e1d4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e1d4-107">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="9e1d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e1d4-108">Properties</span></span>
|<span data-ttu-id="9e1d4-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e1d4-109">Property</span></span>|<span data-ttu-id="9e1d4-110">类型</span><span class="sxs-lookup"><span data-stu-id="9e1d4-110">Type</span></span>|<span data-ttu-id="9e1d4-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e1d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e1d4-112">访问</span><span class="sxs-lookup"><span data-stu-id="9e1d4-112">access</span></span>|<span data-ttu-id="9e1d4-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-113">Boolean</span></span>|<span data-ttu-id="9e1d4-114">如果应排除 MS Office Access，则该值为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-115">excel</span><span class="sxs-lookup"><span data-stu-id="9e1d4-115">excel</span></span>|<span data-ttu-id="9e1d4-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-116">Boolean</span></span>|<span data-ttu-id="9e1d4-117">如果不应排除 MS Office Excel 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-118">为止</span><span class="sxs-lookup"><span data-stu-id="9e1d4-118">groove</span></span>|<span data-ttu-id="9e1d4-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-119">Boolean</span></span>|<span data-ttu-id="9e1d4-120">如果要排除 MS Office OneDrive for Business-Groove 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="9e1d4-121">infoPath</span></span>|<span data-ttu-id="9e1d4-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-122">Boolean</span></span>|<span data-ttu-id="9e1d4-123">如果不应排除 MS Office InfoPath，则值为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-124">lync</span><span class="sxs-lookup"><span data-stu-id="9e1d4-124">lync</span></span>|<span data-ttu-id="9e1d4-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-125">Boolean</span></span>|<span data-ttu-id="9e1d4-126">如果要排除 MS Office Skype for Business-Lync 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-127">For</span><span class="sxs-lookup"><span data-stu-id="9e1d4-127">oneDrive</span></span>|<span data-ttu-id="9e1d4-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-128">Boolean</span></span>|<span data-ttu-id="9e1d4-129">如果不应排除 MS Office OneDrive，则值为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="9e1d4-130">oneNote</span></span>|<span data-ttu-id="9e1d4-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-131">Boolean</span></span>|<span data-ttu-id="9e1d4-132">如果不应排除 MS Office OneNote 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-133">outlook</span><span class="sxs-lookup"><span data-stu-id="9e1d4-133">outlook</span></span>|<span data-ttu-id="9e1d4-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-134">Boolean</span></span>|<span data-ttu-id="9e1d4-135">如果不应排除 MS Office Outlook 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="9e1d4-136">powerPoint</span></span>|<span data-ttu-id="9e1d4-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-137">Boolean</span></span>|<span data-ttu-id="9e1d4-138">如果不应排除 MS Office PowerPoint，则值为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-139">发布者</span><span class="sxs-lookup"><span data-stu-id="9e1d4-139">publisher</span></span>|<span data-ttu-id="9e1d4-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-140">Boolean</span></span>|<span data-ttu-id="9e1d4-141">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="9e1d4-142">sharePointDesigner</span></span>|<span data-ttu-id="9e1d4-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-143">Boolean</span></span>|<span data-ttu-id="9e1d4-144">如果不应排除 MS Office SharePointDesigner 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-145">协作</span><span class="sxs-lookup"><span data-stu-id="9e1d4-145">teams</span></span>|<span data-ttu-id="9e1d4-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-146">Boolean</span></span>|<span data-ttu-id="9e1d4-147">如果不应排除 MS Office 团队，则值为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-147">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-148">visio</span><span class="sxs-lookup"><span data-stu-id="9e1d4-148">visio</span></span>|<span data-ttu-id="9e1d4-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-149">Boolean</span></span>|<span data-ttu-id="9e1d4-150">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-150">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="9e1d4-151">word</span><span class="sxs-lookup"><span data-stu-id="9e1d4-151">word</span></span>|<span data-ttu-id="9e1d4-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e1d4-152">Boolean</span></span>|<span data-ttu-id="9e1d4-153">如果不应排除 MS Office Word 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-153">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e1d4-154">关系</span><span class="sxs-lookup"><span data-stu-id="9e1d4-154">Relationships</span></span>
<span data-ttu-id="9e1d4-155">无</span><span class="sxs-lookup"><span data-stu-id="9e1d4-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e1d4-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e1d4-156">JSON Representation</span></span>
<span data-ttu-id="9e1d4-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e1d4-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "teams": true,
  "visio": true,
  "word": true
}
```



