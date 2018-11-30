---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043898"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="08da3-103">excludedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="08da3-103">excludedApps resource type</span></span>

> <span data-ttu-id="08da3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08da3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08da3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08da3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08da3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08da3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08da3-107">包含用于排除 Office365 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="08da3-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="08da3-108">属性</span><span class="sxs-lookup"><span data-stu-id="08da3-108">Properties</span></span>
|<span data-ttu-id="08da3-109">属性</span><span class="sxs-lookup"><span data-stu-id="08da3-109">Property</span></span>|<span data-ttu-id="08da3-110">类型</span><span class="sxs-lookup"><span data-stu-id="08da3-110">Type</span></span>|<span data-ttu-id="08da3-111">说明</span><span class="sxs-lookup"><span data-stu-id="08da3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08da3-112">访问</span><span class="sxs-lookup"><span data-stu-id="08da3-112">access</span></span>|<span data-ttu-id="08da3-113">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-113">Boolean</span></span>|<span data-ttu-id="08da3-114">值为 if 或不应排除 MS Office Access。</span><span class="sxs-lookup"><span data-stu-id="08da3-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-115">excel</span><span class="sxs-lookup"><span data-stu-id="08da3-115">excel</span></span>|<span data-ttu-id="08da3-116">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-116">Boolean</span></span>|<span data-ttu-id="08da3-117">值为 if 或不应排除 MS Office Excel。</span><span class="sxs-lookup"><span data-stu-id="08da3-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-118">groove</span><span class="sxs-lookup"><span data-stu-id="08da3-118">groove</span></span>|<span data-ttu-id="08da3-119">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-119">Boolean</span></span>|<span data-ttu-id="08da3-120">如果值或不应排除 MS Office OneDrive for Business 的 Groove。</span><span class="sxs-lookup"><span data-stu-id="08da3-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="08da3-121">infoPath</span></span>|<span data-ttu-id="08da3-122">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-122">Boolean</span></span>|<span data-ttu-id="08da3-123">值为 if 或不应排除 MS Office InfoPath。</span><span class="sxs-lookup"><span data-stu-id="08da3-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-124">lync</span><span class="sxs-lookup"><span data-stu-id="08da3-124">lync</span></span>|<span data-ttu-id="08da3-125">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-125">Boolean</span></span>|<span data-ttu-id="08da3-126">如果值或不应排除 MS Office Skype for Business-Lync。</span><span class="sxs-lookup"><span data-stu-id="08da3-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="08da3-127">oneDrive</span></span>|<span data-ttu-id="08da3-128">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-128">Boolean</span></span>|<span data-ttu-id="08da3-129">值为 if 或不应排除 MS Office OneDrive。</span><span class="sxs-lookup"><span data-stu-id="08da3-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="08da3-130">oneNote</span></span>|<span data-ttu-id="08da3-131">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-131">Boolean</span></span>|<span data-ttu-id="08da3-132">值为 if 或不应排除 MS Office OneNote。</span><span class="sxs-lookup"><span data-stu-id="08da3-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-133">outlook</span><span class="sxs-lookup"><span data-stu-id="08da3-133">outlook</span></span>|<span data-ttu-id="08da3-134">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-134">Boolean</span></span>|<span data-ttu-id="08da3-135">值为 if 或不应排除 MS Office Outlook。</span><span class="sxs-lookup"><span data-stu-id="08da3-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="08da3-136">powerPoint</span></span>|<span data-ttu-id="08da3-137">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-137">Boolean</span></span>|<span data-ttu-id="08da3-138">值为 if 或不应排除 MS Office PowerPoint。</span><span class="sxs-lookup"><span data-stu-id="08da3-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-139">publisher</span><span class="sxs-lookup"><span data-stu-id="08da3-139">publisher</span></span>|<span data-ttu-id="08da3-140">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-140">Boolean</span></span>|<span data-ttu-id="08da3-141">值为 if 或不应排除 MS Office Publisher。</span><span class="sxs-lookup"><span data-stu-id="08da3-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="08da3-142">sharePointDesigner</span></span>|<span data-ttu-id="08da3-143">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-143">Boolean</span></span>|<span data-ttu-id="08da3-144">值为 if 或不应排除 MS Office SharePointDesigner。</span><span class="sxs-lookup"><span data-stu-id="08da3-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-145">visio</span><span class="sxs-lookup"><span data-stu-id="08da3-145">visio</span></span>|<span data-ttu-id="08da3-146">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-146">Boolean</span></span>|<span data-ttu-id="08da3-147">值为 if 或不应排除 MS Office Visio。</span><span class="sxs-lookup"><span data-stu-id="08da3-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="08da3-148">word</span><span class="sxs-lookup"><span data-stu-id="08da3-148">word</span></span>|<span data-ttu-id="08da3-149">布尔</span><span class="sxs-lookup"><span data-stu-id="08da3-149">Boolean</span></span>|<span data-ttu-id="08da3-150">值为 if 或不应排除 MS Office Word。</span><span class="sxs-lookup"><span data-stu-id="08da3-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08da3-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="08da3-151">Relationships</span></span>
<span data-ttu-id="08da3-152">无</span><span class="sxs-lookup"><span data-stu-id="08da3-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08da3-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08da3-153">JSON Representation</span></span>
<span data-ttu-id="08da3-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08da3-154">Here is a JSON representation of the resource.</span></span>
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





