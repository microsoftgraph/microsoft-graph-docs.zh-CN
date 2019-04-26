---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4e4b7255f82fe9b0fa0b517e66aeb00e05ee16b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552252"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="254bf-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="254bf-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="254bf-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="254bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="254bf-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="254bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="254bf-107">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="254bf-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="254bf-108">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="254bf-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="254bf-109">方法</span><span class="sxs-lookup"><span data-stu-id="254bf-109">Methods</span></span>
|<span data-ttu-id="254bf-110">方法</span><span class="sxs-lookup"><span data-stu-id="254bf-110">Method</span></span>|<span data-ttu-id="254bf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="254bf-111">Return Type</span></span>|<span data-ttu-id="254bf-112">说明</span><span class="sxs-lookup"><span data-stu-id="254bf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="254bf-113">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="254bf-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="254bf-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="254bf-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="254bf-115">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254bf-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="254bf-116">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="254bf-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="254bf-118">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254bf-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="254bf-119">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="254bf-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="254bf-121">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="254bf-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="254bf-122">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="254bf-123">无</span><span class="sxs-lookup"><span data-stu-id="254bf-123">None</span></span>|<span data-ttu-id="254bf-124">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="254bf-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="254bf-125">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="254bf-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="254bf-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="254bf-127">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="254bf-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="254bf-128">属性</span><span class="sxs-lookup"><span data-stu-id="254bf-128">Properties</span></span>
|<span data-ttu-id="254bf-129">属性</span><span class="sxs-lookup"><span data-stu-id="254bf-129">Property</span></span>|<span data-ttu-id="254bf-130">类型</span><span class="sxs-lookup"><span data-stu-id="254bf-130">Type</span></span>|<span data-ttu-id="254bf-131">说明</span><span class="sxs-lookup"><span data-stu-id="254bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254bf-132">id</span><span class="sxs-lookup"><span data-stu-id="254bf-132">id</span></span>|<span data-ttu-id="254bf-133">String</span><span class="sxs-lookup"><span data-stu-id="254bf-133">String</span></span>|<span data-ttu-id="254bf-134">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="254bf-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="254bf-135">关系</span><span class="sxs-lookup"><span data-stu-id="254bf-135">Relationships</span></span>
|<span data-ttu-id="254bf-136">关系</span><span class="sxs-lookup"><span data-stu-id="254bf-136">Relationship</span></span>|<span data-ttu-id="254bf-137">类型</span><span class="sxs-lookup"><span data-stu-id="254bf-137">Type</span></span>|<span data-ttu-id="254bf-138">说明</span><span class="sxs-lookup"><span data-stu-id="254bf-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254bf-139">files</span><span class="sxs-lookup"><span data-stu-id="254bf-139">files</span></span>|<span data-ttu-id="254bf-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="254bf-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="254bf-141">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="254bf-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="254bf-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="254bf-142">containedApps</span></span>|<span data-ttu-id="254bf-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="254bf-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="254bf-144">充当包的 MobileLobApp 中包含的应用程序的集合。</span><span class="sxs-lookup"><span data-stu-id="254bf-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="254bf-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="254bf-145">JSON Representation</span></span>
<span data-ttu-id="254bf-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="254bf-146">Here is a JSON representation of the resource.</span></span>
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





