---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395676"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="921eb-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="921eb-103">excludedApps resource type</span></span>

> <span data-ttu-id="921eb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="921eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="921eb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="921eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="921eb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="921eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921eb-107">包含用于排除 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="921eb-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="921eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="921eb-108">Properties</span></span>
|<span data-ttu-id="921eb-109">属性</span><span class="sxs-lookup"><span data-stu-id="921eb-109">Property</span></span>|<span data-ttu-id="921eb-110">类型</span><span class="sxs-lookup"><span data-stu-id="921eb-110">Type</span></span>|<span data-ttu-id="921eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="921eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921eb-112">访问</span><span class="sxs-lookup"><span data-stu-id="921eb-112">access</span></span>|<span data-ttu-id="921eb-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-113">Boolean</span></span>|<span data-ttu-id="921eb-114">值为 if 或不应排除 MS Office Access。</span><span class="sxs-lookup"><span data-stu-id="921eb-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-115">excel</span><span class="sxs-lookup"><span data-stu-id="921eb-115">excel</span></span>|<span data-ttu-id="921eb-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-116">Boolean</span></span>|<span data-ttu-id="921eb-117">值为 if 或不应排除 MS Office Excel。</span><span class="sxs-lookup"><span data-stu-id="921eb-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-118">groove</span><span class="sxs-lookup"><span data-stu-id="921eb-118">groove</span></span>|<span data-ttu-id="921eb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-119">Boolean</span></span>|<span data-ttu-id="921eb-120">如果值或不应排除 MS Office OneDrive for Business 的 Groove。</span><span class="sxs-lookup"><span data-stu-id="921eb-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="921eb-121">infoPath</span></span>|<span data-ttu-id="921eb-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-122">Boolean</span></span>|<span data-ttu-id="921eb-123">值为 if 或不应排除 MS Office InfoPath。</span><span class="sxs-lookup"><span data-stu-id="921eb-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-124">lync</span><span class="sxs-lookup"><span data-stu-id="921eb-124">lync</span></span>|<span data-ttu-id="921eb-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-125">Boolean</span></span>|<span data-ttu-id="921eb-126">如果值或不应排除 MS Office Skype for Business-Lync。</span><span class="sxs-lookup"><span data-stu-id="921eb-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="921eb-127">oneDrive</span></span>|<span data-ttu-id="921eb-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-128">Boolean</span></span>|<span data-ttu-id="921eb-129">值为 if 或不应排除 MS Office OneDrive。</span><span class="sxs-lookup"><span data-stu-id="921eb-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="921eb-130">oneNote</span></span>|<span data-ttu-id="921eb-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-131">Boolean</span></span>|<span data-ttu-id="921eb-132">值为 if 或不应排除 MS Office OneNote。</span><span class="sxs-lookup"><span data-stu-id="921eb-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-133">outlook</span><span class="sxs-lookup"><span data-stu-id="921eb-133">outlook</span></span>|<span data-ttu-id="921eb-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-134">Boolean</span></span>|<span data-ttu-id="921eb-135">值为 if 或不应排除 MS Office Outlook。</span><span class="sxs-lookup"><span data-stu-id="921eb-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="921eb-136">powerPoint</span></span>|<span data-ttu-id="921eb-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-137">Boolean</span></span>|<span data-ttu-id="921eb-138">值为 if 或不应排除 MS Office PowerPoint。</span><span class="sxs-lookup"><span data-stu-id="921eb-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-139">publisher</span><span class="sxs-lookup"><span data-stu-id="921eb-139">publisher</span></span>|<span data-ttu-id="921eb-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-140">Boolean</span></span>|<span data-ttu-id="921eb-141">值为 if 或不应排除 MS Office Publisher。</span><span class="sxs-lookup"><span data-stu-id="921eb-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="921eb-142">sharePointDesigner</span></span>|<span data-ttu-id="921eb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-143">Boolean</span></span>|<span data-ttu-id="921eb-144">值为 if 或不应排除 MS Office SharePointDesigner。</span><span class="sxs-lookup"><span data-stu-id="921eb-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-145">visio</span><span class="sxs-lookup"><span data-stu-id="921eb-145">visio</span></span>|<span data-ttu-id="921eb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-146">Boolean</span></span>|<span data-ttu-id="921eb-147">值为 if 或不应排除 MS Office Visio。</span><span class="sxs-lookup"><span data-stu-id="921eb-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="921eb-148">word</span><span class="sxs-lookup"><span data-stu-id="921eb-148">word</span></span>|<span data-ttu-id="921eb-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="921eb-149">Boolean</span></span>|<span data-ttu-id="921eb-150">值为 if 或不应排除 MS Office Word。</span><span class="sxs-lookup"><span data-stu-id="921eb-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="921eb-151">关系</span><span class="sxs-lookup"><span data-stu-id="921eb-151">Relationships</span></span>
<span data-ttu-id="921eb-152">无</span><span class="sxs-lookup"><span data-stu-id="921eb-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="921eb-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="921eb-153">JSON Representation</span></span>
<span data-ttu-id="921eb-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="921eb-154">Here is a JSON representation of the resource.</span></span>
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




