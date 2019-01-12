---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76895e336b633da63d62a467a267f96b3f344132
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918873"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="4fcd3-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fcd3-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="4fcd3-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fcd3-106">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="4fcd3-107">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="4fcd3-108">方法</span><span class="sxs-lookup"><span data-stu-id="4fcd3-108">Methods</span></span>
|<span data-ttu-id="4fcd3-109">方法</span><span class="sxs-lookup"><span data-stu-id="4fcd3-109">Method</span></span>|<span data-ttu-id="4fcd3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4fcd3-110">Return Type</span></span>|<span data-ttu-id="4fcd3-111">说明</span><span class="sxs-lookup"><span data-stu-id="4fcd3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fcd3-112">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="4fcd3-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="4fcd3-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fcd3-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="4fcd3-114">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="4fcd3-115">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="4fcd3-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcd3-117">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4fcd3-118">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="4fcd3-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcd3-120">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4fcd3-121">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="4fcd3-122">无</span><span class="sxs-lookup"><span data-stu-id="4fcd3-122">None</span></span>|<span data-ttu-id="4fcd3-123">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="4fcd3-124">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="4fcd3-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcd3-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcd3-126">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fcd3-127">属性</span><span class="sxs-lookup"><span data-stu-id="4fcd3-127">Properties</span></span>
|<span data-ttu-id="4fcd3-128">属性</span><span class="sxs-lookup"><span data-stu-id="4fcd3-128">Property</span></span>|<span data-ttu-id="4fcd3-129">类型</span><span class="sxs-lookup"><span data-stu-id="4fcd3-129">Type</span></span>|<span data-ttu-id="4fcd3-130">说明</span><span class="sxs-lookup"><span data-stu-id="4fcd3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcd3-131">id</span><span class="sxs-lookup"><span data-stu-id="4fcd3-131">id</span></span>|<span data-ttu-id="4fcd3-132">String</span><span class="sxs-lookup"><span data-stu-id="4fcd3-132">String</span></span>|<span data-ttu-id="4fcd3-133">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fcd3-134">关系</span><span class="sxs-lookup"><span data-stu-id="4fcd3-134">Relationships</span></span>
|<span data-ttu-id="4fcd3-135">关系</span><span class="sxs-lookup"><span data-stu-id="4fcd3-135">Relationship</span></span>|<span data-ttu-id="4fcd3-136">类型</span><span class="sxs-lookup"><span data-stu-id="4fcd3-136">Type</span></span>|<span data-ttu-id="4fcd3-137">说明</span><span class="sxs-lookup"><span data-stu-id="4fcd3-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcd3-138">files</span><span class="sxs-lookup"><span data-stu-id="4fcd3-138">files</span></span>|<span data-ttu-id="4fcd3-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fcd3-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="4fcd3-140">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fcd3-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fcd3-141">JSON Representation</span></span>
<span data-ttu-id="4fcd3-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fcd3-142">Here is a JSON representation of the resource.</span></span>
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



