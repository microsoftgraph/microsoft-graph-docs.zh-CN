---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
ms.openlocfilehash: 8cc5bd6e3c7aa5f08236d2662821a9a5d03707d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360345"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="c9a1a-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9a1a-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="c9a1a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a1a-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9a1a-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9a1a-108">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="c9a1a-109">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="c9a1a-110">方法</span><span class="sxs-lookup"><span data-stu-id="c9a1a-110">Methods</span></span>
|<span data-ttu-id="c9a1a-111">方法</span><span class="sxs-lookup"><span data-stu-id="c9a1a-111">Method</span></span>|<span data-ttu-id="c9a1a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9a1a-112">Return Type</span></span>|<span data-ttu-id="c9a1a-113">说明</span><span class="sxs-lookup"><span data-stu-id="c9a1a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9a1a-114">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="c9a1a-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="c9a1a-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9a1a-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="c9a1a-116">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="c9a1a-117">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="c9a1a-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c9a1a-119">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c9a1a-120">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="c9a1a-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c9a1a-122">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c9a1a-123">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="c9a1a-124">无</span><span class="sxs-lookup"><span data-stu-id="c9a1a-124">None</span></span>|<span data-ttu-id="c9a1a-125">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="c9a1a-126">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="c9a1a-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c9a1a-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c9a1a-128">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9a1a-129">属性</span><span class="sxs-lookup"><span data-stu-id="c9a1a-129">Properties</span></span>
|<span data-ttu-id="c9a1a-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9a1a-130">Property</span></span>|<span data-ttu-id="c9a1a-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9a1a-131">Type</span></span>|<span data-ttu-id="c9a1a-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9a1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9a1a-133">id</span><span class="sxs-lookup"><span data-stu-id="c9a1a-133">id</span></span>|<span data-ttu-id="c9a1a-134">String</span><span class="sxs-lookup"><span data-stu-id="c9a1a-134">String</span></span>|<span data-ttu-id="c9a1a-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9a1a-136">关系</span><span class="sxs-lookup"><span data-stu-id="c9a1a-136">Relationships</span></span>
|<span data-ttu-id="c9a1a-137">关系</span><span class="sxs-lookup"><span data-stu-id="c9a1a-137">Relationship</span></span>|<span data-ttu-id="c9a1a-138">类型</span><span class="sxs-lookup"><span data-stu-id="c9a1a-138">Type</span></span>|<span data-ttu-id="c9a1a-139">说明</span><span class="sxs-lookup"><span data-stu-id="c9a1a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9a1a-140">files</span><span class="sxs-lookup"><span data-stu-id="c9a1a-140">files</span></span>|<span data-ttu-id="c9a1a-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9a1a-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="c9a1a-142">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="c9a1a-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="c9a1a-143">containedApps</span></span>|<span data-ttu-id="c9a1a-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9a1a-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="c9a1a-145">包含充当包 MobileLobApp 中的应用程序的集合。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9a1a-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9a1a-146">JSON Representation</span></span>
<span data-ttu-id="c9a1a-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9a1a-147">Here is a JSON representation of the resource.</span></span>
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





