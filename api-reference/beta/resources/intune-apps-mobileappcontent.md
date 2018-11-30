---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
ms.openlocfilehash: e57c4c0823636143962ac5fe1c50f4377e731f84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045093"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ff2b2-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff2b2-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="ff2b2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff2b2-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff2b2-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff2b2-108">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ff2b2-109">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="ff2b2-110">方法</span><span class="sxs-lookup"><span data-stu-id="ff2b2-110">Methods</span></span>
|<span data-ttu-id="ff2b2-111">方法</span><span class="sxs-lookup"><span data-stu-id="ff2b2-111">Method</span></span>|<span data-ttu-id="ff2b2-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff2b2-112">Return Type</span></span>|<span data-ttu-id="ff2b2-113">说明</span><span class="sxs-lookup"><span data-stu-id="ff2b2-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff2b2-114">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ff2b2-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="ff2b2-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff2b2-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="ff2b2-116">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ff2b2-117">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="ff2b2-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ff2b2-119">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ff2b2-120">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="ff2b2-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ff2b2-122">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ff2b2-123">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="ff2b2-124">无</span><span class="sxs-lookup"><span data-stu-id="ff2b2-124">None</span></span>|<span data-ttu-id="ff2b2-125">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ff2b2-126">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="ff2b2-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ff2b2-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ff2b2-128">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff2b2-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff2b2-129">Properties</span></span>
|<span data-ttu-id="ff2b2-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff2b2-130">Property</span></span>|<span data-ttu-id="ff2b2-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff2b2-131">Type</span></span>|<span data-ttu-id="ff2b2-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff2b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2b2-133">id</span><span class="sxs-lookup"><span data-stu-id="ff2b2-133">id</span></span>|<span data-ttu-id="ff2b2-134">String</span><span class="sxs-lookup"><span data-stu-id="ff2b2-134">String</span></span>|<span data-ttu-id="ff2b2-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2b2-136">关系</span><span class="sxs-lookup"><span data-stu-id="ff2b2-136">Relationships</span></span>
|<span data-ttu-id="ff2b2-137">关系</span><span class="sxs-lookup"><span data-stu-id="ff2b2-137">Relationship</span></span>|<span data-ttu-id="ff2b2-138">类型</span><span class="sxs-lookup"><span data-stu-id="ff2b2-138">Type</span></span>|<span data-ttu-id="ff2b2-139">说明</span><span class="sxs-lookup"><span data-stu-id="ff2b2-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2b2-140">files</span><span class="sxs-lookup"><span data-stu-id="ff2b2-140">files</span></span>|<span data-ttu-id="ff2b2-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff2b2-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ff2b2-142">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="ff2b2-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="ff2b2-143">containedApps</span></span>|<span data-ttu-id="ff2b2-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff2b2-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="ff2b2-145">包含充当包 MobileLobApp 中的应用程序的集合。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff2b2-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff2b2-146">JSON Representation</span></span>
<span data-ttu-id="ff2b2-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff2b2-147">Here is a JSON representation of the resource.</span></span>
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





