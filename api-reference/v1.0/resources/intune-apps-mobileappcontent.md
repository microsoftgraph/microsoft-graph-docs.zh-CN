---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261297"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="e2551-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2551-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="e2551-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2551-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2551-106">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="e2551-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="e2551-107">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="e2551-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="e2551-108">方法</span><span class="sxs-lookup"><span data-stu-id="e2551-108">Methods</span></span>
|<span data-ttu-id="e2551-109">方法</span><span class="sxs-lookup"><span data-stu-id="e2551-109">Method</span></span>|<span data-ttu-id="e2551-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2551-110">Return Type</span></span>|<span data-ttu-id="e2551-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2551-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2551-112">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="e2551-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="e2551-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2551-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e2551-114">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2551-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="e2551-115">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="e2551-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="e2551-117">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2551-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e2551-118">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="e2551-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="e2551-120">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2551-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e2551-121">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="e2551-122">无</span><span class="sxs-lookup"><span data-stu-id="e2551-122">None</span></span>|<span data-ttu-id="e2551-123">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="e2551-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="e2551-124">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="e2551-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e2551-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="e2551-126">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2551-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2551-127">属性</span><span class="sxs-lookup"><span data-stu-id="e2551-127">Properties</span></span>
|<span data-ttu-id="e2551-128">属性</span><span class="sxs-lookup"><span data-stu-id="e2551-128">Property</span></span>|<span data-ttu-id="e2551-129">类型</span><span class="sxs-lookup"><span data-stu-id="e2551-129">Type</span></span>|<span data-ttu-id="e2551-130">说明</span><span class="sxs-lookup"><span data-stu-id="e2551-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2551-131">id</span><span class="sxs-lookup"><span data-stu-id="e2551-131">id</span></span>|<span data-ttu-id="e2551-132">String</span><span class="sxs-lookup"><span data-stu-id="e2551-132">String</span></span>|<span data-ttu-id="e2551-133">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="e2551-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2551-134">关系</span><span class="sxs-lookup"><span data-stu-id="e2551-134">Relationships</span></span>
|<span data-ttu-id="e2551-135">关系</span><span class="sxs-lookup"><span data-stu-id="e2551-135">Relationship</span></span>|<span data-ttu-id="e2551-136">类型</span><span class="sxs-lookup"><span data-stu-id="e2551-136">Type</span></span>|<span data-ttu-id="e2551-137">说明</span><span class="sxs-lookup"><span data-stu-id="e2551-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2551-138">files</span><span class="sxs-lookup"><span data-stu-id="e2551-138">files</span></span>|<span data-ttu-id="e2551-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2551-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="e2551-140">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="e2551-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2551-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2551-141">JSON Representation</span></span>
<span data-ttu-id="e2551-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2551-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



