---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553048"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="06c34-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="06c34-103">excludedApps resource type</span></span>

> <span data-ttu-id="06c34-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06c34-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c34-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="06c34-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="06c34-107">属性</span><span class="sxs-lookup"><span data-stu-id="06c34-107">Properties</span></span>
|<span data-ttu-id="06c34-108">属性</span><span class="sxs-lookup"><span data-stu-id="06c34-108">Property</span></span>|<span data-ttu-id="06c34-109">类型</span><span class="sxs-lookup"><span data-stu-id="06c34-109">Type</span></span>|<span data-ttu-id="06c34-110">说明</span><span class="sxs-lookup"><span data-stu-id="06c34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c34-111">访问</span><span class="sxs-lookup"><span data-stu-id="06c34-111">access</span></span>|<span data-ttu-id="06c34-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-112">Boolean</span></span>|<span data-ttu-id="06c34-113">如果应排除 MS Office Access, 则该值为。</span><span class="sxs-lookup"><span data-stu-id="06c34-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-114">excel</span><span class="sxs-lookup"><span data-stu-id="06c34-114">excel</span></span>|<span data-ttu-id="06c34-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-115">Boolean</span></span>|<span data-ttu-id="06c34-116">如果不应排除 MS Office Excel 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="06c34-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-117">为止</span><span class="sxs-lookup"><span data-stu-id="06c34-117">groove</span></span>|<span data-ttu-id="06c34-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-118">Boolean</span></span>|<span data-ttu-id="06c34-119">如果要排除 MS Office OneDrive for business-Groove 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="06c34-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="06c34-120">infoPath</span></span>|<span data-ttu-id="06c34-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-121">Boolean</span></span>|<span data-ttu-id="06c34-122">如果不应排除 MS Office InfoPath, 则值为。</span><span class="sxs-lookup"><span data-stu-id="06c34-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-123">lync</span><span class="sxs-lookup"><span data-stu-id="06c34-123">lync</span></span>|<span data-ttu-id="06c34-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-124">Boolean</span></span>|<span data-ttu-id="06c34-125">如果要排除 MS Office Skype for business-Lync 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="06c34-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-126">for</span><span class="sxs-lookup"><span data-stu-id="06c34-126">oneDrive</span></span>|<span data-ttu-id="06c34-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-127">Boolean</span></span>|<span data-ttu-id="06c34-128">如果不应排除 MS Office OneDrive, 则值为。</span><span class="sxs-lookup"><span data-stu-id="06c34-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="06c34-129">oneNote</span></span>|<span data-ttu-id="06c34-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-130">Boolean</span></span>|<span data-ttu-id="06c34-131">如果不应排除 MS Office OneNote 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="06c34-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-132">outlook</span><span class="sxs-lookup"><span data-stu-id="06c34-132">outlook</span></span>|<span data-ttu-id="06c34-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-133">Boolean</span></span>|<span data-ttu-id="06c34-134">如果不应排除 MS Office Outlook 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="06c34-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="06c34-135">powerPoint</span></span>|<span data-ttu-id="06c34-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-136">Boolean</span></span>|<span data-ttu-id="06c34-137">如果不应排除 MS Office PowerPoint, 则值为。</span><span class="sxs-lookup"><span data-stu-id="06c34-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-138">发布者</span><span class="sxs-lookup"><span data-stu-id="06c34-138">publisher</span></span>|<span data-ttu-id="06c34-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-139">Boolean</span></span>|<span data-ttu-id="06c34-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="06c34-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="06c34-141">sharePointDesigner</span></span>|<span data-ttu-id="06c34-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-142">Boolean</span></span>|<span data-ttu-id="06c34-143">如果不应排除 MS Office SharePointDesigner 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="06c34-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-144">协作</span><span class="sxs-lookup"><span data-stu-id="06c34-144">teams</span></span>|<span data-ttu-id="06c34-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-145">Boolean</span></span>|<span data-ttu-id="06c34-146">如果不应排除 MS Office 团队, 则值为。</span><span class="sxs-lookup"><span data-stu-id="06c34-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-147">visio</span><span class="sxs-lookup"><span data-stu-id="06c34-147">visio</span></span>|<span data-ttu-id="06c34-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-148">Boolean</span></span>|<span data-ttu-id="06c34-149">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="06c34-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="06c34-150">word</span><span class="sxs-lookup"><span data-stu-id="06c34-150">word</span></span>|<span data-ttu-id="06c34-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="06c34-151">Boolean</span></span>|<span data-ttu-id="06c34-152">如果不应排除 MS Office Word 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="06c34-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06c34-153">关系</span><span class="sxs-lookup"><span data-stu-id="06c34-153">Relationships</span></span>
<span data-ttu-id="06c34-154">无</span><span class="sxs-lookup"><span data-stu-id="06c34-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06c34-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06c34-155">JSON Representation</span></span>
<span data-ttu-id="06c34-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06c34-156">Here is a JSON representation of the resource.</span></span>
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





