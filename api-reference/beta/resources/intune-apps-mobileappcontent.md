---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 394eadb5f24f900bda4435804f8da4831ba08ec3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708982"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="98d4b-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="98d4b-104">mobileAppContent resource type</span></span>

<span data-ttu-id="98d4b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d4b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98d4b-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98d4b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98d4b-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98d4b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98d4b-108">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="98d4b-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="98d4b-109">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="98d4b-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="98d4b-110">Methods</span><span class="sxs-lookup"><span data-stu-id="98d4b-110">Methods</span></span>
|<span data-ttu-id="98d4b-111">方法</span><span class="sxs-lookup"><span data-stu-id="98d4b-111">Method</span></span>|<span data-ttu-id="98d4b-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="98d4b-112">Return Type</span></span>|<span data-ttu-id="98d4b-113">说明</span><span class="sxs-lookup"><span data-stu-id="98d4b-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98d4b-114">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="98d4b-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="98d4b-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98d4b-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="98d4b-116">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98d4b-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="98d4b-117">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="98d4b-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="98d4b-119">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98d4b-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="98d4b-120">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="98d4b-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="98d4b-122">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98d4b-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="98d4b-123">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="98d4b-124">无</span><span class="sxs-lookup"><span data-stu-id="98d4b-124">None</span></span>|<span data-ttu-id="98d4b-125">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="98d4b-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="98d4b-126">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="98d4b-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="98d4b-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="98d4b-128">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="98d4b-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98d4b-129">属性</span><span class="sxs-lookup"><span data-stu-id="98d4b-129">Properties</span></span>
|<span data-ttu-id="98d4b-130">属性</span><span class="sxs-lookup"><span data-stu-id="98d4b-130">Property</span></span>|<span data-ttu-id="98d4b-131">类型</span><span class="sxs-lookup"><span data-stu-id="98d4b-131">Type</span></span>|<span data-ttu-id="98d4b-132">说明</span><span class="sxs-lookup"><span data-stu-id="98d4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98d4b-133">id</span><span class="sxs-lookup"><span data-stu-id="98d4b-133">id</span></span>|<span data-ttu-id="98d4b-134">String</span><span class="sxs-lookup"><span data-stu-id="98d4b-134">String</span></span>|<span data-ttu-id="98d4b-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="98d4b-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98d4b-136">关系</span><span class="sxs-lookup"><span data-stu-id="98d4b-136">Relationships</span></span>
|<span data-ttu-id="98d4b-137">关系</span><span class="sxs-lookup"><span data-stu-id="98d4b-137">Relationship</span></span>|<span data-ttu-id="98d4b-138">类型</span><span class="sxs-lookup"><span data-stu-id="98d4b-138">Type</span></span>|<span data-ttu-id="98d4b-139">说明</span><span class="sxs-lookup"><span data-stu-id="98d4b-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98d4b-140">files</span><span class="sxs-lookup"><span data-stu-id="98d4b-140">files</span></span>|<span data-ttu-id="98d4b-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98d4b-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="98d4b-142">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="98d4b-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="98d4b-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="98d4b-143">containedApps</span></span>|<span data-ttu-id="98d4b-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98d4b-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="98d4b-145">充当包的 MobileLobApp 中包含的应用程序的集合。</span><span class="sxs-lookup"><span data-stu-id="98d4b-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98d4b-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98d4b-146">JSON Representation</span></span>
<span data-ttu-id="98d4b-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d4b-147">Here is a JSON representation of the resource.</span></span>
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





