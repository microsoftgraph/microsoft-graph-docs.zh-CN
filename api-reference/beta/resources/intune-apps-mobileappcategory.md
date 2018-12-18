---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
author: tfitzmac
ms.openlocfilehash: f40e9a24269d276c89d770acb0d772a7bdf94c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340759"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="6f0b0-103">mobileAppCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f0b0-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="6f0b0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f0b0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f0b0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f0b0-107">包含单个 Intune 应用类别的属性。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-107">Contains properties for a single Intune app category.</span></span>
## <a name="methods"></a><span data-ttu-id="6f0b0-108">方法</span><span class="sxs-lookup"><span data-stu-id="6f0b0-108">Methods</span></span>
|<span data-ttu-id="6f0b0-109">方法</span><span class="sxs-lookup"><span data-stu-id="6f0b0-109">Method</span></span>|<span data-ttu-id="6f0b0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f0b0-110">Return Type</span></span>|<span data-ttu-id="6f0b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f0b0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f0b0-112">列出 mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="6f0b0-112">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="6f0b0-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f0b0-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="6f0b0-114">列出 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-114">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="6f0b0-115">获取 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-115">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="6f0b0-116">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-116">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="6f0b0-117">读取 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-117">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="6f0b0-118">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-118">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="6f0b0-119">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-119">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="6f0b0-120">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-120">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="6f0b0-121">删除 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-121">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="6f0b0-122">无</span><span class="sxs-lookup"><span data-stu-id="6f0b0-122">None</span></span>|<span data-ttu-id="6f0b0-123">删除 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-123">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="6f0b0-124">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-124">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="6f0b0-125">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="6f0b0-125">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="6f0b0-126">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-126">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f0b0-127">属性</span><span class="sxs-lookup"><span data-stu-id="6f0b0-127">Properties</span></span>
|<span data-ttu-id="6f0b0-128">属性</span><span class="sxs-lookup"><span data-stu-id="6f0b0-128">Property</span></span>|<span data-ttu-id="6f0b0-129">类型</span><span class="sxs-lookup"><span data-stu-id="6f0b0-129">Type</span></span>|<span data-ttu-id="6f0b0-130">说明</span><span class="sxs-lookup"><span data-stu-id="6f0b0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f0b0-131">id</span><span class="sxs-lookup"><span data-stu-id="6f0b0-131">id</span></span>|<span data-ttu-id="6f0b0-132">String</span><span class="sxs-lookup"><span data-stu-id="6f0b0-132">String</span></span>|<span data-ttu-id="6f0b0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-133">The key of the entity.</span></span>|
|<span data-ttu-id="6f0b0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6f0b0-134">displayName</span></span>|<span data-ttu-id="6f0b0-135">String</span><span class="sxs-lookup"><span data-stu-id="6f0b0-135">String</span></span>|<span data-ttu-id="6f0b0-136">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-136">The name of the app category.</span></span>|
|<span data-ttu-id="6f0b0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f0b0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f0b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f0b0-138">DateTimeOffset</span></span>|<span data-ttu-id="6f0b0-139">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-139">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f0b0-140">关系</span><span class="sxs-lookup"><span data-stu-id="6f0b0-140">Relationships</span></span>
<span data-ttu-id="6f0b0-141">无</span><span class="sxs-lookup"><span data-stu-id="6f0b0-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f0b0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f0b0-142">JSON Representation</span></span>
<span data-ttu-id="6f0b0-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f0b0-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```





