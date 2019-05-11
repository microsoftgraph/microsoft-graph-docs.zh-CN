---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37abd83b34fde565aa78e62454c4ce7d47ea192a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950408"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="bfb8d-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfb8d-103">excludedApps resource type</span></span>

> <span data-ttu-id="bfb8d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfb8d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfb8d-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="bfb8d-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfb8d-107">Properties</span></span>
|<span data-ttu-id="bfb8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="bfb8d-108">Property</span></span>|<span data-ttu-id="bfb8d-109">类型</span><span class="sxs-lookup"><span data-stu-id="bfb8d-109">Type</span></span>|<span data-ttu-id="bfb8d-110">说明</span><span class="sxs-lookup"><span data-stu-id="bfb8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfb8d-111">访问</span><span class="sxs-lookup"><span data-stu-id="bfb8d-111">access</span></span>|<span data-ttu-id="bfb8d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-112">Boolean</span></span>|<span data-ttu-id="bfb8d-113">如果应排除 MS Office Access, 则该值为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-114">excel</span><span class="sxs-lookup"><span data-stu-id="bfb8d-114">excel</span></span>|<span data-ttu-id="bfb8d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-115">Boolean</span></span>|<span data-ttu-id="bfb8d-116">如果不应排除 MS Office Excel 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-117">为止</span><span class="sxs-lookup"><span data-stu-id="bfb8d-117">groove</span></span>|<span data-ttu-id="bfb8d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-118">Boolean</span></span>|<span data-ttu-id="bfb8d-119">如果要排除 MS Office OneDrive for Business-Groove 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="bfb8d-120">infoPath</span></span>|<span data-ttu-id="bfb8d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-121">Boolean</span></span>|<span data-ttu-id="bfb8d-122">如果不应排除 MS Office InfoPath, 则值为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-123">lync</span><span class="sxs-lookup"><span data-stu-id="bfb8d-123">lync</span></span>|<span data-ttu-id="bfb8d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-124">Boolean</span></span>|<span data-ttu-id="bfb8d-125">如果要排除 MS Office Skype for Business-Lync 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-126">For</span><span class="sxs-lookup"><span data-stu-id="bfb8d-126">oneDrive</span></span>|<span data-ttu-id="bfb8d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-127">Boolean</span></span>|<span data-ttu-id="bfb8d-128">如果不应排除 MS Office OneDrive, 则值为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="bfb8d-129">oneNote</span></span>|<span data-ttu-id="bfb8d-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-130">Boolean</span></span>|<span data-ttu-id="bfb8d-131">如果不应排除 MS Office OneNote 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-132">outlook</span><span class="sxs-lookup"><span data-stu-id="bfb8d-132">outlook</span></span>|<span data-ttu-id="bfb8d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-133">Boolean</span></span>|<span data-ttu-id="bfb8d-134">如果不应排除 MS Office Outlook 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="bfb8d-135">powerPoint</span></span>|<span data-ttu-id="bfb8d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-136">Boolean</span></span>|<span data-ttu-id="bfb8d-137">如果不应排除 MS Office PowerPoint, 则值为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-138">发布者</span><span class="sxs-lookup"><span data-stu-id="bfb8d-138">publisher</span></span>|<span data-ttu-id="bfb8d-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-139">Boolean</span></span>|<span data-ttu-id="bfb8d-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="bfb8d-141">sharePointDesigner</span></span>|<span data-ttu-id="bfb8d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-142">Boolean</span></span>|<span data-ttu-id="bfb8d-143">如果不应排除 MS Office SharePointDesigner 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-144">协作</span><span class="sxs-lookup"><span data-stu-id="bfb8d-144">teams</span></span>|<span data-ttu-id="bfb8d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-145">Boolean</span></span>|<span data-ttu-id="bfb8d-146">如果不应排除 MS Office 团队, 则值为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-147">visio</span><span class="sxs-lookup"><span data-stu-id="bfb8d-147">visio</span></span>|<span data-ttu-id="bfb8d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-148">Boolean</span></span>|<span data-ttu-id="bfb8d-149">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="bfb8d-150">word</span><span class="sxs-lookup"><span data-stu-id="bfb8d-150">word</span></span>|<span data-ttu-id="bfb8d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb8d-151">Boolean</span></span>|<span data-ttu-id="bfb8d-152">如果不应排除 MS Office Word 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb8d-153">关系</span><span class="sxs-lookup"><span data-stu-id="bfb8d-153">Relationships</span></span>
<span data-ttu-id="bfb8d-154">无</span><span class="sxs-lookup"><span data-stu-id="bfb8d-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfb8d-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfb8d-155">JSON Representation</span></span>
<span data-ttu-id="bfb8d-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfb8d-156">Here is a JSON representation of the resource.</span></span>
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




