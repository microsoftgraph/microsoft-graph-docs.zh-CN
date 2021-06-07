---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c36a306e0b594ff84bffbc3e80fd393d20051371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759007"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="dc50d-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc50d-104">mobileAppContent resource type</span></span>

<span data-ttu-id="dc50d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc50d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc50d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc50d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc50d-107">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="dc50d-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="dc50d-108">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="dc50d-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="dc50d-109">方法</span><span class="sxs-lookup"><span data-stu-id="dc50d-109">Methods</span></span>
|<span data-ttu-id="dc50d-110">方法</span><span class="sxs-lookup"><span data-stu-id="dc50d-110">Method</span></span>|<span data-ttu-id="dc50d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc50d-111">Return Type</span></span>|<span data-ttu-id="dc50d-112">说明</span><span class="sxs-lookup"><span data-stu-id="dc50d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc50d-113">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="dc50d-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="dc50d-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc50d-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="dc50d-115">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc50d-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="dc50d-116">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="dc50d-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="dc50d-118">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc50d-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="dc50d-119">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="dc50d-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="dc50d-121">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc50d-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="dc50d-122">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="dc50d-123">无</span><span class="sxs-lookup"><span data-stu-id="dc50d-123">None</span></span>|<span data-ttu-id="dc50d-124">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="dc50d-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="dc50d-125">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="dc50d-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="dc50d-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="dc50d-127">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc50d-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc50d-128">属性</span><span class="sxs-lookup"><span data-stu-id="dc50d-128">Properties</span></span>
|<span data-ttu-id="dc50d-129">属性</span><span class="sxs-lookup"><span data-stu-id="dc50d-129">Property</span></span>|<span data-ttu-id="dc50d-130">类型</span><span class="sxs-lookup"><span data-stu-id="dc50d-130">Type</span></span>|<span data-ttu-id="dc50d-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc50d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc50d-132">id</span><span class="sxs-lookup"><span data-stu-id="dc50d-132">id</span></span>|<span data-ttu-id="dc50d-133">String</span><span class="sxs-lookup"><span data-stu-id="dc50d-133">String</span></span>|<span data-ttu-id="dc50d-134">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="dc50d-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc50d-135">关系</span><span class="sxs-lookup"><span data-stu-id="dc50d-135">Relationships</span></span>
|<span data-ttu-id="dc50d-136">关系</span><span class="sxs-lookup"><span data-stu-id="dc50d-136">Relationship</span></span>|<span data-ttu-id="dc50d-137">类型</span><span class="sxs-lookup"><span data-stu-id="dc50d-137">Type</span></span>|<span data-ttu-id="dc50d-138">说明</span><span class="sxs-lookup"><span data-stu-id="dc50d-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc50d-139">files</span><span class="sxs-lookup"><span data-stu-id="dc50d-139">files</span></span>|<span data-ttu-id="dc50d-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc50d-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="dc50d-141">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="dc50d-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc50d-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc50d-142">JSON Representation</span></span>
<span data-ttu-id="dc50d-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc50d-143">Here is a JSON representation of the resource.</span></span>
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




