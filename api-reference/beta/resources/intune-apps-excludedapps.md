---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ba3e53a26ff71dde2d5a95fde811e42ba2ccb99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154024"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="16fd9-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="16fd9-103">excludedApps resource type</span></span>

> <span data-ttu-id="16fd9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16fd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16fd9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16fd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16fd9-106">包含已排除的 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="16fd9-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="16fd9-107">属性</span><span class="sxs-lookup"><span data-stu-id="16fd9-107">Properties</span></span>
|<span data-ttu-id="16fd9-108">属性</span><span class="sxs-lookup"><span data-stu-id="16fd9-108">Property</span></span>|<span data-ttu-id="16fd9-109">类型</span><span class="sxs-lookup"><span data-stu-id="16fd9-109">Type</span></span>|<span data-ttu-id="16fd9-110">说明</span><span class="sxs-lookup"><span data-stu-id="16fd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16fd9-111">访问</span><span class="sxs-lookup"><span data-stu-id="16fd9-111">access</span></span>|<span data-ttu-id="16fd9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-112">Boolean</span></span>|<span data-ttu-id="16fd9-113">如果应排除 MS Office Access, 则该值为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-114">excel</span><span class="sxs-lookup"><span data-stu-id="16fd9-114">excel</span></span>|<span data-ttu-id="16fd9-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-115">Boolean</span></span>|<span data-ttu-id="16fd9-116">如果不应排除 MS Office Excel 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-117">为止</span><span class="sxs-lookup"><span data-stu-id="16fd9-117">groove</span></span>|<span data-ttu-id="16fd9-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-118">Boolean</span></span>|<span data-ttu-id="16fd9-119">如果要排除 MS Office OneDrive for business-Groove 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="16fd9-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="16fd9-120">infoPath</span></span>|<span data-ttu-id="16fd9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-121">Boolean</span></span>|<span data-ttu-id="16fd9-122">如果不应排除 MS Office InfoPath, 则值为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-123">lync</span><span class="sxs-lookup"><span data-stu-id="16fd9-123">lync</span></span>|<span data-ttu-id="16fd9-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-124">Boolean</span></span>|<span data-ttu-id="16fd9-125">如果要排除 MS Office Skype for business-Lync 的值, 应将其排除。</span><span class="sxs-lookup"><span data-stu-id="16fd9-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-126">for</span><span class="sxs-lookup"><span data-stu-id="16fd9-126">oneDrive</span></span>|<span data-ttu-id="16fd9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-127">Boolean</span></span>|<span data-ttu-id="16fd9-128">如果不应排除 MS Office OneDrive, 则值为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-129">oneNote</span><span class="sxs-lookup"><span data-stu-id="16fd9-129">oneNote</span></span>|<span data-ttu-id="16fd9-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-130">Boolean</span></span>|<span data-ttu-id="16fd9-131">如果不应排除 MS Office OneNote 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-132">outlook</span><span class="sxs-lookup"><span data-stu-id="16fd9-132">outlook</span></span>|<span data-ttu-id="16fd9-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-133">Boolean</span></span>|<span data-ttu-id="16fd9-134">如果不应排除 MS Office Outlook 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="16fd9-135">powerPoint</span></span>|<span data-ttu-id="16fd9-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-136">Boolean</span></span>|<span data-ttu-id="16fd9-137">如果不应排除 MS Office PowerPoint, 则值为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-138">publisher</span><span class="sxs-lookup"><span data-stu-id="16fd9-138">publisher</span></span>|<span data-ttu-id="16fd9-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-139">Boolean</span></span>|<span data-ttu-id="16fd9-140">应排除 MS Office 发布服务器的值。</span><span class="sxs-lookup"><span data-stu-id="16fd9-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-141">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="16fd9-141">sharePointDesigner</span></span>|<span data-ttu-id="16fd9-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-142">Boolean</span></span>|<span data-ttu-id="16fd9-143">如果不应排除 MS Office SharePointDesigner 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-144">visio</span><span class="sxs-lookup"><span data-stu-id="16fd9-144">visio</span></span>|<span data-ttu-id="16fd9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-145">Boolean</span></span>|<span data-ttu-id="16fd9-146">应排除 MS Office Visio 的值。</span><span class="sxs-lookup"><span data-stu-id="16fd9-146">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="16fd9-147">word</span><span class="sxs-lookup"><span data-stu-id="16fd9-147">word</span></span>|<span data-ttu-id="16fd9-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fd9-148">Boolean</span></span>|<span data-ttu-id="16fd9-149">如果不应排除 MS Office Word 的值, 则为。</span><span class="sxs-lookup"><span data-stu-id="16fd9-149">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16fd9-150">关系</span><span class="sxs-lookup"><span data-stu-id="16fd9-150">Relationships</span></span>
<span data-ttu-id="16fd9-151">无</span><span class="sxs-lookup"><span data-stu-id="16fd9-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16fd9-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16fd9-152">JSON Representation</span></span>
<span data-ttu-id="16fd9-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16fd9-153">Here is a JSON representation of the resource.</span></span>
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
  "visio": true,
  "word": true
}
```




