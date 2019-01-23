---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ceeb6cd4e989f4e020c885dde119c39d9659539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418181"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="9907c-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="9907c-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="9907c-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9907c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9907c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9907c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9907c-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9907c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9907c-108">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="9907c-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="9907c-109">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="9907c-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="9907c-110">方法</span><span class="sxs-lookup"><span data-stu-id="9907c-110">Methods</span></span>
|<span data-ttu-id="9907c-111">方法</span><span class="sxs-lookup"><span data-stu-id="9907c-111">Method</span></span>|<span data-ttu-id="9907c-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="9907c-112">Return Type</span></span>|<span data-ttu-id="9907c-113">说明</span><span class="sxs-lookup"><span data-stu-id="9907c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9907c-114">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="9907c-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="9907c-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9907c-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="9907c-116">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9907c-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="9907c-117">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="9907c-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="9907c-119">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9907c-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="9907c-120">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="9907c-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="9907c-122">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9907c-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="9907c-123">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="9907c-124">无</span><span class="sxs-lookup"><span data-stu-id="9907c-124">None</span></span>|<span data-ttu-id="9907c-125">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="9907c-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="9907c-126">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="9907c-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="9907c-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="9907c-128">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9907c-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9907c-129">属性</span><span class="sxs-lookup"><span data-stu-id="9907c-129">Properties</span></span>
|<span data-ttu-id="9907c-130">属性</span><span class="sxs-lookup"><span data-stu-id="9907c-130">Property</span></span>|<span data-ttu-id="9907c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9907c-131">Type</span></span>|<span data-ttu-id="9907c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9907c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9907c-133">id</span><span class="sxs-lookup"><span data-stu-id="9907c-133">id</span></span>|<span data-ttu-id="9907c-134">String</span><span class="sxs-lookup"><span data-stu-id="9907c-134">String</span></span>|<span data-ttu-id="9907c-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="9907c-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9907c-136">关系</span><span class="sxs-lookup"><span data-stu-id="9907c-136">Relationships</span></span>
|<span data-ttu-id="9907c-137">关系</span><span class="sxs-lookup"><span data-stu-id="9907c-137">Relationship</span></span>|<span data-ttu-id="9907c-138">类型</span><span class="sxs-lookup"><span data-stu-id="9907c-138">Type</span></span>|<span data-ttu-id="9907c-139">说明</span><span class="sxs-lookup"><span data-stu-id="9907c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9907c-140">files</span><span class="sxs-lookup"><span data-stu-id="9907c-140">files</span></span>|<span data-ttu-id="9907c-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9907c-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="9907c-142">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="9907c-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="9907c-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="9907c-143">containedApps</span></span>|<span data-ttu-id="9907c-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="9907c-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="9907c-145">包含充当包 MobileLobApp 中的应用程序的集合。</span><span class="sxs-lookup"><span data-stu-id="9907c-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9907c-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9907c-146">JSON Representation</span></span>
<span data-ttu-id="9907c-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9907c-147">Here is a JSON representation of the resource.</span></span>
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




