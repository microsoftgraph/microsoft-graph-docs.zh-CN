---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d566cd8ba088568e27c9a7e4878eda54cd7f1252
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366089"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="d1448-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1448-103">excludedApps resource type</span></span>

> <span data-ttu-id="d1448-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1448-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1448-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1448-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1448-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="d1448-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="d1448-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1448-107">Properties</span></span>
|<span data-ttu-id="d1448-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1448-108">Property</span></span>|<span data-ttu-id="d1448-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1448-109">Type</span></span>|<span data-ttu-id="d1448-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1448-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1448-111">访问</span><span class="sxs-lookup"><span data-stu-id="d1448-111">access</span></span>|<span data-ttu-id="d1448-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-112">Boolean</span></span>|<span data-ttu-id="d1448-113">如果应排除 MS Office Access, 则该值为。</span><span class="sxs-lookup"><span data-stu-id="d1448-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-114">excel</span><span class="sxs-lookup"><span data-stu-id="d1448-114">excel</span></span>|<span data-ttu-id="d1448-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-115">Boolean</span></span>|<span data-ttu-id="d1448-116">如果不应排除 MS Office Excel 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="d1448-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-117">为止</span><span class="sxs-lookup"><span data-stu-id="d1448-117">groove</span></span>|<span data-ttu-id="d1448-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-118">Boolean</span></span>|<span data-ttu-id="d1448-119">如果要排除 MS Office OneDrive for Business-Groove 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="d1448-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="d1448-120">infoPath</span></span>|<span data-ttu-id="d1448-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-121">Boolean</span></span>|<span data-ttu-id="d1448-122">如果不应排除 MS Office InfoPath, 则值为。</span><span class="sxs-lookup"><span data-stu-id="d1448-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-123">lync</span><span class="sxs-lookup"><span data-stu-id="d1448-123">lync</span></span>|<span data-ttu-id="d1448-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-124">Boolean</span></span>|<span data-ttu-id="d1448-125">如果要排除 MS Office Skype for Business-Lync 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="d1448-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-126">For</span><span class="sxs-lookup"><span data-stu-id="d1448-126">oneDrive</span></span>|<span data-ttu-id="d1448-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-127">Boolean</span></span>|<span data-ttu-id="d1448-128">如果不应排除 MS Office OneDrive, 则值为。</span><span class="sxs-lookup"><span data-stu-id="d1448-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="d1448-129">oneNote</span></span>|<span data-ttu-id="d1448-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-130">Boolean</span></span>|<span data-ttu-id="d1448-131">如果不应排除 MS Office OneNote 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="d1448-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-132">outlook</span><span class="sxs-lookup"><span data-stu-id="d1448-132">outlook</span></span>|<span data-ttu-id="d1448-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-133">Boolean</span></span>|<span data-ttu-id="d1448-134">如果不应排除 MS Office Outlook 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="d1448-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="d1448-135">powerPoint</span></span>|<span data-ttu-id="d1448-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-136">Boolean</span></span>|<span data-ttu-id="d1448-137">如果不应排除 MS Office PowerPoint, 则值为。</span><span class="sxs-lookup"><span data-stu-id="d1448-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-138">发布者</span><span class="sxs-lookup"><span data-stu-id="d1448-138">publisher</span></span>|<span data-ttu-id="d1448-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-139">Boolean</span></span>|<span data-ttu-id="d1448-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="d1448-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="d1448-141">sharePointDesigner</span></span>|<span data-ttu-id="d1448-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-142">Boolean</span></span>|<span data-ttu-id="d1448-143">如果不应排除 MS Office SharePointDesigner 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="d1448-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-144">协作</span><span class="sxs-lookup"><span data-stu-id="d1448-144">teams</span></span>|<span data-ttu-id="d1448-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-145">Boolean</span></span>|<span data-ttu-id="d1448-146">如果不应排除 MS Office 团队, 则值为。</span><span class="sxs-lookup"><span data-stu-id="d1448-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-147">visio</span><span class="sxs-lookup"><span data-stu-id="d1448-147">visio</span></span>|<span data-ttu-id="d1448-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-148">Boolean</span></span>|<span data-ttu-id="d1448-149">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="d1448-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="d1448-150">word</span><span class="sxs-lookup"><span data-stu-id="d1448-150">word</span></span>|<span data-ttu-id="d1448-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1448-151">Boolean</span></span>|<span data-ttu-id="d1448-152">如果不应排除 MS Office Word 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="d1448-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1448-153">关系</span><span class="sxs-lookup"><span data-stu-id="d1448-153">Relationships</span></span>
<span data-ttu-id="d1448-154">无</span><span class="sxs-lookup"><span data-stu-id="d1448-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1448-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1448-155">JSON Representation</span></span>
<span data-ttu-id="d1448-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1448-156">Here is a JSON representation of the resource.</span></span>
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



