---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
ms.openlocfilehash: 071231d71d6111b5bbac85c6ef89f710b8ada72b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334172"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="77403-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="77403-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="77403-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="77403-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77403-106">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="77403-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="77403-107">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="77403-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="77403-108">方法</span><span class="sxs-lookup"><span data-stu-id="77403-108">Methods</span></span>
|<span data-ttu-id="77403-109">方法</span><span class="sxs-lookup"><span data-stu-id="77403-109">Method</span></span>|<span data-ttu-id="77403-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="77403-110">Return Type</span></span>|<span data-ttu-id="77403-111">说明</span><span class="sxs-lookup"><span data-stu-id="77403-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77403-112">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="77403-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="77403-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77403-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="77403-114">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77403-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="77403-115">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="77403-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="77403-117">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77403-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="77403-118">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="77403-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="77403-120">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77403-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="77403-121">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="77403-122">无</span><span class="sxs-lookup"><span data-stu-id="77403-122">None</span></span>|<span data-ttu-id="77403-123">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="77403-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="77403-124">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="77403-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="77403-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="77403-126">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77403-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77403-127">属性</span><span class="sxs-lookup"><span data-stu-id="77403-127">Properties</span></span>
|<span data-ttu-id="77403-128">属性</span><span class="sxs-lookup"><span data-stu-id="77403-128">Property</span></span>|<span data-ttu-id="77403-129">类型</span><span class="sxs-lookup"><span data-stu-id="77403-129">Type</span></span>|<span data-ttu-id="77403-130">说明</span><span class="sxs-lookup"><span data-stu-id="77403-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77403-131">id</span><span class="sxs-lookup"><span data-stu-id="77403-131">id</span></span>|<span data-ttu-id="77403-132">String</span><span class="sxs-lookup"><span data-stu-id="77403-132">String</span></span>|<span data-ttu-id="77403-133">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="77403-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77403-134">关系</span><span class="sxs-lookup"><span data-stu-id="77403-134">Relationships</span></span>
|<span data-ttu-id="77403-135">关系</span><span class="sxs-lookup"><span data-stu-id="77403-135">Relationship</span></span>|<span data-ttu-id="77403-136">类型</span><span class="sxs-lookup"><span data-stu-id="77403-136">Type</span></span>|<span data-ttu-id="77403-137">说明</span><span class="sxs-lookup"><span data-stu-id="77403-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77403-138">files</span><span class="sxs-lookup"><span data-stu-id="77403-138">files</span></span>|<span data-ttu-id="77403-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77403-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="77403-140">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="77403-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77403-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77403-141">JSON Representation</span></span>
<span data-ttu-id="77403-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77403-142">Here is a JSON representation of the resource.</span></span>
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



