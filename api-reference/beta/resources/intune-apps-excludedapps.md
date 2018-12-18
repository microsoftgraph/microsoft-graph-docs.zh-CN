---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344623"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="7ac3d-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ac3d-103">excludedApps resource type</span></span>

> <span data-ttu-id="7ac3d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac3d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ac3d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ac3d-107">包含用于排除 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="7ac3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ac3d-108">Properties</span></span>
|<span data-ttu-id="7ac3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ac3d-109">Property</span></span>|<span data-ttu-id="7ac3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ac3d-110">Type</span></span>|<span data-ttu-id="7ac3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ac3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac3d-112">访问</span><span class="sxs-lookup"><span data-stu-id="7ac3d-112">access</span></span>|<span data-ttu-id="7ac3d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-113">Boolean</span></span>|<span data-ttu-id="7ac3d-114">值为 if 或不应排除 MS Office Access。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-115">excel</span><span class="sxs-lookup"><span data-stu-id="7ac3d-115">excel</span></span>|<span data-ttu-id="7ac3d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-116">Boolean</span></span>|<span data-ttu-id="7ac3d-117">值为 if 或不应排除 MS Office Excel。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-118">groove</span><span class="sxs-lookup"><span data-stu-id="7ac3d-118">groove</span></span>|<span data-ttu-id="7ac3d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-119">Boolean</span></span>|<span data-ttu-id="7ac3d-120">如果值或不应排除 MS Office OneDrive for Business 的 Groove。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="7ac3d-121">infoPath</span></span>|<span data-ttu-id="7ac3d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-122">Boolean</span></span>|<span data-ttu-id="7ac3d-123">值为 if 或不应排除 MS Office InfoPath。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-124">lync</span><span class="sxs-lookup"><span data-stu-id="7ac3d-124">lync</span></span>|<span data-ttu-id="7ac3d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-125">Boolean</span></span>|<span data-ttu-id="7ac3d-126">如果值或不应排除 MS Office Skype for Business-Lync。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="7ac3d-127">oneDrive</span></span>|<span data-ttu-id="7ac3d-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-128">Boolean</span></span>|<span data-ttu-id="7ac3d-129">值为 if 或不应排除 MS Office OneDrive。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="7ac3d-130">oneNote</span></span>|<span data-ttu-id="7ac3d-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-131">Boolean</span></span>|<span data-ttu-id="7ac3d-132">值为 if 或不应排除 MS Office OneNote。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-133">outlook</span><span class="sxs-lookup"><span data-stu-id="7ac3d-133">outlook</span></span>|<span data-ttu-id="7ac3d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-134">Boolean</span></span>|<span data-ttu-id="7ac3d-135">值为 if 或不应排除 MS Office Outlook。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="7ac3d-136">powerPoint</span></span>|<span data-ttu-id="7ac3d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-137">Boolean</span></span>|<span data-ttu-id="7ac3d-138">值为 if 或不应排除 MS Office PowerPoint。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-139">publisher</span><span class="sxs-lookup"><span data-stu-id="7ac3d-139">publisher</span></span>|<span data-ttu-id="7ac3d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-140">Boolean</span></span>|<span data-ttu-id="7ac3d-141">值为 if 或不应排除 MS Office Publisher。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="7ac3d-142">sharePointDesigner</span></span>|<span data-ttu-id="7ac3d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-143">Boolean</span></span>|<span data-ttu-id="7ac3d-144">值为 if 或不应排除 MS Office SharePointDesigner。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-145">visio</span><span class="sxs-lookup"><span data-stu-id="7ac3d-145">visio</span></span>|<span data-ttu-id="7ac3d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-146">Boolean</span></span>|<span data-ttu-id="7ac3d-147">值为 if 或不应排除 MS Office Visio。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="7ac3d-148">word</span><span class="sxs-lookup"><span data-stu-id="7ac3d-148">word</span></span>|<span data-ttu-id="7ac3d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac3d-149">Boolean</span></span>|<span data-ttu-id="7ac3d-150">值为 if 或不应排除 MS Office Word。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac3d-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="7ac3d-151">Relationships</span></span>
<span data-ttu-id="7ac3d-152">无</span><span class="sxs-lookup"><span data-stu-id="7ac3d-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ac3d-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ac3d-153">JSON Representation</span></span>
<span data-ttu-id="7ac3d-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ac3d-154">Here is a JSON representation of the resource.</span></span>
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





