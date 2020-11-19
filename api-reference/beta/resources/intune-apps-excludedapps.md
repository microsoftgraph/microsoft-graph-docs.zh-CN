---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4a481d52b06c59d9d79df439b41152600af989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274283"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c2385-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2385-103">excludedApps resource type</span></span>

<span data-ttu-id="c2385-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2385-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2385-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2385-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2385-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2385-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2385-107">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="c2385-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="c2385-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2385-108">Properties</span></span>
|<span data-ttu-id="c2385-109">属性</span><span class="sxs-lookup"><span data-stu-id="c2385-109">Property</span></span>|<span data-ttu-id="c2385-110">类型</span><span class="sxs-lookup"><span data-stu-id="c2385-110">Type</span></span>|<span data-ttu-id="c2385-111">说明</span><span class="sxs-lookup"><span data-stu-id="c2385-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2385-112">访问</span><span class="sxs-lookup"><span data-stu-id="c2385-112">access</span></span>|<span data-ttu-id="c2385-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-113">Boolean</span></span>|<span data-ttu-id="c2385-114">如果应排除 MS Office Access，则该值为。</span><span class="sxs-lookup"><span data-stu-id="c2385-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-115">必应</span><span class="sxs-lookup"><span data-stu-id="c2385-115">bing</span></span>|<span data-ttu-id="c2385-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-116">Boolean</span></span>|<span data-ttu-id="c2385-117">如果应排除 Microsoft 搜索为默认值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-117">The value for if Microsoft Search as default should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-118">excel</span><span class="sxs-lookup"><span data-stu-id="c2385-118">excel</span></span>|<span data-ttu-id="c2385-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-119">Boolean</span></span>|<span data-ttu-id="c2385-120">如果不应排除 MS Office Excel 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-120">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-121">为止</span><span class="sxs-lookup"><span data-stu-id="c2385-121">groove</span></span>|<span data-ttu-id="c2385-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-122">Boolean</span></span>|<span data-ttu-id="c2385-123">如果要排除 MS Office OneDrive for Business-Groove 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="c2385-123">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-124">infoPath</span><span class="sxs-lookup"><span data-stu-id="c2385-124">infoPath</span></span>|<span data-ttu-id="c2385-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-125">Boolean</span></span>|<span data-ttu-id="c2385-126">如果不应排除 MS Office InfoPath，则值为。</span><span class="sxs-lookup"><span data-stu-id="c2385-126">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-127">lync</span><span class="sxs-lookup"><span data-stu-id="c2385-127">lync</span></span>|<span data-ttu-id="c2385-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-128">Boolean</span></span>|<span data-ttu-id="c2385-129">如果要排除 MS Office Skype for Business-Lync 的值，应将其排除。</span><span class="sxs-lookup"><span data-stu-id="c2385-129">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-130">For</span><span class="sxs-lookup"><span data-stu-id="c2385-130">oneDrive</span></span>|<span data-ttu-id="c2385-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-131">Boolean</span></span>|<span data-ttu-id="c2385-132">如果不应排除 MS Office OneDrive，则值为。</span><span class="sxs-lookup"><span data-stu-id="c2385-132">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-133">oneNote</span><span class="sxs-lookup"><span data-stu-id="c2385-133">oneNote</span></span>|<span data-ttu-id="c2385-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-134">Boolean</span></span>|<span data-ttu-id="c2385-135">如果不应排除 MS Office OneNote 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-135">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-136">outlook</span><span class="sxs-lookup"><span data-stu-id="c2385-136">outlook</span></span>|<span data-ttu-id="c2385-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-137">Boolean</span></span>|<span data-ttu-id="c2385-138">如果不应排除 MS Office Outlook 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-138">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-139">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c2385-139">powerPoint</span></span>|<span data-ttu-id="c2385-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-140">Boolean</span></span>|<span data-ttu-id="c2385-141">如果不应排除 MS Office PowerPoint，则值为。</span><span class="sxs-lookup"><span data-stu-id="c2385-141">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-142">发布者</span><span class="sxs-lookup"><span data-stu-id="c2385-142">publisher</span></span>|<span data-ttu-id="c2385-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-143">Boolean</span></span>|<span data-ttu-id="c2385-144">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="c2385-144">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-145">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="c2385-145">sharePointDesigner</span></span>|<span data-ttu-id="c2385-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-146">Boolean</span></span>|<span data-ttu-id="c2385-147">如果不应排除 MS Office SharePointDesigner 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-147">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-148">协作</span><span class="sxs-lookup"><span data-stu-id="c2385-148">teams</span></span>|<span data-ttu-id="c2385-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-149">Boolean</span></span>|<span data-ttu-id="c2385-150">如果不应排除 MS Office 团队，则值为。</span><span class="sxs-lookup"><span data-stu-id="c2385-150">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-151">visio</span><span class="sxs-lookup"><span data-stu-id="c2385-151">visio</span></span>|<span data-ttu-id="c2385-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-152">Boolean</span></span>|<span data-ttu-id="c2385-153">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="c2385-153">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c2385-154">word</span><span class="sxs-lookup"><span data-stu-id="c2385-154">word</span></span>|<span data-ttu-id="c2385-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2385-155">Boolean</span></span>|<span data-ttu-id="c2385-156">如果不应排除 MS Office Word 的值，则为。</span><span class="sxs-lookup"><span data-stu-id="c2385-156">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2385-157">关系</span><span class="sxs-lookup"><span data-stu-id="c2385-157">Relationships</span></span>
<span data-ttu-id="c2385-158">无</span><span class="sxs-lookup"><span data-stu-id="c2385-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2385-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2385-159">JSON Representation</span></span>
<span data-ttu-id="c2385-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2385-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "bing": true,
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




