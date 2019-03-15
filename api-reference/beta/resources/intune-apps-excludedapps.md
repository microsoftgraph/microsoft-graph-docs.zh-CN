---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571688"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="f1dd4-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1dd4-103">excludedApps resource type</span></span>

> <span data-ttu-id="f1dd4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1dd4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1dd4-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="f1dd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1dd4-107">Properties</span></span>
|<span data-ttu-id="f1dd4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1dd4-108">Property</span></span>|<span data-ttu-id="f1dd4-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1dd4-109">Type</span></span>|<span data-ttu-id="f1dd4-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1dd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1dd4-111">访问</span><span class="sxs-lookup"><span data-stu-id="f1dd4-111">access</span></span>|<span data-ttu-id="f1dd4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-112">Boolean</span></span>|<span data-ttu-id="f1dd4-113">如果应排除 MS Office Access, 则该值为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-114">excel</span><span class="sxs-lookup"><span data-stu-id="f1dd4-114">excel</span></span>|<span data-ttu-id="f1dd4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-115">Boolean</span></span>|<span data-ttu-id="f1dd4-116">如果不应排除 MS Office Excel 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-117">为止</span><span class="sxs-lookup"><span data-stu-id="f1dd4-117">groove</span></span>|<span data-ttu-id="f1dd4-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-118">Boolean</span></span>|<span data-ttu-id="f1dd4-119">如果要排除 MS Office OneDrive for business-Groove 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="f1dd4-120">infoPath</span></span>|<span data-ttu-id="f1dd4-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-121">Boolean</span></span>|<span data-ttu-id="f1dd4-122">如果不应排除 MS Office InfoPath, 则值为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-123">lync</span><span class="sxs-lookup"><span data-stu-id="f1dd4-123">lync</span></span>|<span data-ttu-id="f1dd4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-124">Boolean</span></span>|<span data-ttu-id="f1dd4-125">如果要排除 MS Office Skype for business-Lync 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-126">for</span><span class="sxs-lookup"><span data-stu-id="f1dd4-126">oneDrive</span></span>|<span data-ttu-id="f1dd4-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-127">Boolean</span></span>|<span data-ttu-id="f1dd4-128">如果不应排除 MS Office OneDrive, 则值为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="f1dd4-129">oneNote</span></span>|<span data-ttu-id="f1dd4-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-130">Boolean</span></span>|<span data-ttu-id="f1dd4-131">如果不应排除 MS Office OneNote 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-132">outlook</span><span class="sxs-lookup"><span data-stu-id="f1dd4-132">outlook</span></span>|<span data-ttu-id="f1dd4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-133">Boolean</span></span>|<span data-ttu-id="f1dd4-134">如果不应排除 MS Office Outlook 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="f1dd4-135">powerPoint</span></span>|<span data-ttu-id="f1dd4-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-136">Boolean</span></span>|<span data-ttu-id="f1dd4-137">如果不应排除 MS Office PowerPoint, 则值为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-138">发布者</span><span class="sxs-lookup"><span data-stu-id="f1dd4-138">publisher</span></span>|<span data-ttu-id="f1dd4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-139">Boolean</span></span>|<span data-ttu-id="f1dd4-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="f1dd4-141">sharePointDesigner</span></span>|<span data-ttu-id="f1dd4-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-142">Boolean</span></span>|<span data-ttu-id="f1dd4-143">如果不应排除 MS Office SharePointDesigner 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-144">协作</span><span class="sxs-lookup"><span data-stu-id="f1dd4-144">teams</span></span>|<span data-ttu-id="f1dd4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-145">Boolean</span></span>|<span data-ttu-id="f1dd4-146">如果不应排除 MS Office 团队, 则值为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-147">visio</span><span class="sxs-lookup"><span data-stu-id="f1dd4-147">visio</span></span>|<span data-ttu-id="f1dd4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-148">Boolean</span></span>|<span data-ttu-id="f1dd4-149">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="f1dd4-150">word</span><span class="sxs-lookup"><span data-stu-id="f1dd4-150">word</span></span>|<span data-ttu-id="f1dd4-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1dd4-151">Boolean</span></span>|<span data-ttu-id="f1dd4-152">如果不应排除 MS Office Word 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1dd4-153">关系</span><span class="sxs-lookup"><span data-stu-id="f1dd4-153">Relationships</span></span>
<span data-ttu-id="f1dd4-154">无</span><span class="sxs-lookup"><span data-stu-id="f1dd4-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1dd4-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1dd4-155">JSON Representation</span></span>
<span data-ttu-id="f1dd4-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1dd4-156">Here is a JSON representation of the resource.</span></span>
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




