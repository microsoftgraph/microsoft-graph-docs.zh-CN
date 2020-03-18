---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24813edf732d73905a6b45b9e4fe584b6312a13c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798138"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="e0fb7-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0fb7-103">excludedApps resource type</span></span>

> <span data-ttu-id="e0fb7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0fb7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0fb7-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="e0fb7-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0fb7-107">Properties</span></span>
|<span data-ttu-id="e0fb7-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0fb7-108">Property</span></span>|<span data-ttu-id="e0fb7-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0fb7-109">Type</span></span>|<span data-ttu-id="e0fb7-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0fb7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fb7-111">访问</span><span class="sxs-lookup"><span data-stu-id="e0fb7-111">access</span></span>|<span data-ttu-id="e0fb7-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-112">Boolean</span></span>|<span data-ttu-id="e0fb7-113">如果应排除 MS Office Access，则该值为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-114">excel</span><span class="sxs-lookup"><span data-stu-id="e0fb7-114">excel</span></span>|<span data-ttu-id="e0fb7-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-115">Boolean</span></span>|<span data-ttu-id="e0fb7-116">如果不应排除 MS Office Excel 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-117">为止</span><span class="sxs-lookup"><span data-stu-id="e0fb7-117">groove</span></span>|<span data-ttu-id="e0fb7-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-118">Boolean</span></span>|<span data-ttu-id="e0fb7-119">如果要排除 MS Office OneDrive for Business-Groove 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="e0fb7-120">infoPath</span></span>|<span data-ttu-id="e0fb7-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-121">Boolean</span></span>|<span data-ttu-id="e0fb7-122">如果不应排除 MS Office InfoPath，则值为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-123">lync</span><span class="sxs-lookup"><span data-stu-id="e0fb7-123">lync</span></span>|<span data-ttu-id="e0fb7-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-124">Boolean</span></span>|<span data-ttu-id="e0fb7-125">如果要排除 MS Office Skype for Business-Lync 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-126">For</span><span class="sxs-lookup"><span data-stu-id="e0fb7-126">oneDrive</span></span>|<span data-ttu-id="e0fb7-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-127">Boolean</span></span>|<span data-ttu-id="e0fb7-128">如果不应排除 MS Office OneDrive，则值为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="e0fb7-129">oneNote</span></span>|<span data-ttu-id="e0fb7-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-130">Boolean</span></span>|<span data-ttu-id="e0fb7-131">如果不应排除 MS Office OneNote 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-132">outlook</span><span class="sxs-lookup"><span data-stu-id="e0fb7-132">outlook</span></span>|<span data-ttu-id="e0fb7-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-133">Boolean</span></span>|<span data-ttu-id="e0fb7-134">如果不应排除 MS Office Outlook 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="e0fb7-135">powerPoint</span></span>|<span data-ttu-id="e0fb7-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-136">Boolean</span></span>|<span data-ttu-id="e0fb7-137">如果不应排除 MS Office PowerPoint，则值为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-138">发布者</span><span class="sxs-lookup"><span data-stu-id="e0fb7-138">publisher</span></span>|<span data-ttu-id="e0fb7-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-139">Boolean</span></span>|<span data-ttu-id="e0fb7-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="e0fb7-141">sharePointDesigner</span></span>|<span data-ttu-id="e0fb7-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-142">Boolean</span></span>|<span data-ttu-id="e0fb7-143">如果不应排除 MS Office SharePointDesigner 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-144">协作</span><span class="sxs-lookup"><span data-stu-id="e0fb7-144">teams</span></span>|<span data-ttu-id="e0fb7-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-145">Boolean</span></span>|<span data-ttu-id="e0fb7-146">如果不应排除 MS Office 团队，则值为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-147">visio</span><span class="sxs-lookup"><span data-stu-id="e0fb7-147">visio</span></span>|<span data-ttu-id="e0fb7-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-148">Boolean</span></span>|<span data-ttu-id="e0fb7-149">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="e0fb7-150">word</span><span class="sxs-lookup"><span data-stu-id="e0fb7-150">word</span></span>|<span data-ttu-id="e0fb7-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0fb7-151">Boolean</span></span>|<span data-ttu-id="e0fb7-152">如果不应排除 MS Office Word 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0fb7-153">关系</span><span class="sxs-lookup"><span data-stu-id="e0fb7-153">Relationships</span></span>
<span data-ttu-id="e0fb7-154">无</span><span class="sxs-lookup"><span data-stu-id="e0fb7-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0fb7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0fb7-155">JSON Representation</span></span>
<span data-ttu-id="e0fb7-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0fb7-156">Here is a JSON representation of the resource.</span></span>
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



