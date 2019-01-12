---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943947"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="267c6-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="267c6-103">excludedApps resource type</span></span>

> <span data-ttu-id="267c6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="267c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="267c6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="267c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="267c6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="267c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="267c6-107">包含用于排除 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="267c6-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="267c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="267c6-108">Properties</span></span>
|<span data-ttu-id="267c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="267c6-109">Property</span></span>|<span data-ttu-id="267c6-110">类型</span><span class="sxs-lookup"><span data-stu-id="267c6-110">Type</span></span>|<span data-ttu-id="267c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="267c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="267c6-112">访问</span><span class="sxs-lookup"><span data-stu-id="267c6-112">access</span></span>|<span data-ttu-id="267c6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-113">Boolean</span></span>|<span data-ttu-id="267c6-114">值为 if 或不应排除 MS Office Access。</span><span class="sxs-lookup"><span data-stu-id="267c6-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-115">excel</span><span class="sxs-lookup"><span data-stu-id="267c6-115">excel</span></span>|<span data-ttu-id="267c6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-116">Boolean</span></span>|<span data-ttu-id="267c6-117">值为 if 或不应排除 MS Office Excel。</span><span class="sxs-lookup"><span data-stu-id="267c6-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-118">groove</span><span class="sxs-lookup"><span data-stu-id="267c6-118">groove</span></span>|<span data-ttu-id="267c6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-119">Boolean</span></span>|<span data-ttu-id="267c6-120">如果值或不应排除 MS Office OneDrive for Business 的 Groove。</span><span class="sxs-lookup"><span data-stu-id="267c6-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="267c6-121">infoPath</span></span>|<span data-ttu-id="267c6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-122">Boolean</span></span>|<span data-ttu-id="267c6-123">值为 if 或不应排除 MS Office InfoPath。</span><span class="sxs-lookup"><span data-stu-id="267c6-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-124">lync</span><span class="sxs-lookup"><span data-stu-id="267c6-124">lync</span></span>|<span data-ttu-id="267c6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-125">Boolean</span></span>|<span data-ttu-id="267c6-126">如果值或不应排除 MS Office Skype for Business-Lync。</span><span class="sxs-lookup"><span data-stu-id="267c6-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="267c6-127">oneDrive</span></span>|<span data-ttu-id="267c6-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-128">Boolean</span></span>|<span data-ttu-id="267c6-129">值为 if 或不应排除 MS Office OneDrive。</span><span class="sxs-lookup"><span data-stu-id="267c6-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="267c6-130">oneNote</span></span>|<span data-ttu-id="267c6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-131">Boolean</span></span>|<span data-ttu-id="267c6-132">值为 if 或不应排除 MS Office OneNote。</span><span class="sxs-lookup"><span data-stu-id="267c6-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-133">outlook</span><span class="sxs-lookup"><span data-stu-id="267c6-133">outlook</span></span>|<span data-ttu-id="267c6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-134">Boolean</span></span>|<span data-ttu-id="267c6-135">值为 if 或不应排除 MS Office Outlook。</span><span class="sxs-lookup"><span data-stu-id="267c6-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="267c6-136">powerPoint</span></span>|<span data-ttu-id="267c6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-137">Boolean</span></span>|<span data-ttu-id="267c6-138">值为 if 或不应排除 MS Office PowerPoint。</span><span class="sxs-lookup"><span data-stu-id="267c6-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-139">publisher</span><span class="sxs-lookup"><span data-stu-id="267c6-139">publisher</span></span>|<span data-ttu-id="267c6-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-140">Boolean</span></span>|<span data-ttu-id="267c6-141">值为 if 或不应排除 MS Office Publisher。</span><span class="sxs-lookup"><span data-stu-id="267c6-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="267c6-142">sharePointDesigner</span></span>|<span data-ttu-id="267c6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-143">Boolean</span></span>|<span data-ttu-id="267c6-144">值为 if 或不应排除 MS Office SharePointDesigner。</span><span class="sxs-lookup"><span data-stu-id="267c6-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-145">visio</span><span class="sxs-lookup"><span data-stu-id="267c6-145">visio</span></span>|<span data-ttu-id="267c6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-146">Boolean</span></span>|<span data-ttu-id="267c6-147">值为 if 或不应排除 MS Office Visio。</span><span class="sxs-lookup"><span data-stu-id="267c6-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="267c6-148">word</span><span class="sxs-lookup"><span data-stu-id="267c6-148">word</span></span>|<span data-ttu-id="267c6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="267c6-149">Boolean</span></span>|<span data-ttu-id="267c6-150">值为 if 或不应排除 MS Office Word。</span><span class="sxs-lookup"><span data-stu-id="267c6-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="267c6-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="267c6-151">Relationships</span></span>
<span data-ttu-id="267c6-152">无</span><span class="sxs-lookup"><span data-stu-id="267c6-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="267c6-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="267c6-153">JSON Representation</span></span>
<span data-ttu-id="267c6-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="267c6-154">Here is a JSON representation of the resource.</span></span>
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





