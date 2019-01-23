---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 59f840bdd3a01ca8f8614f6e14e53d9ba95005dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422262"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="3ff87-103">mobileAppCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ff87-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="3ff87-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3ff87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ff87-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ff87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ff87-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ff87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff87-107">包含单个 Intune 应用类别的属性。</span><span class="sxs-lookup"><span data-stu-id="3ff87-107">Contains properties for a single Intune app category.</span></span>

## <a name="methods"></a><span data-ttu-id="3ff87-108">方法</span><span class="sxs-lookup"><span data-stu-id="3ff87-108">Methods</span></span>
|<span data-ttu-id="3ff87-109">方法</span><span class="sxs-lookup"><span data-stu-id="3ff87-109">Method</span></span>|<span data-ttu-id="3ff87-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ff87-110">Return Type</span></span>|<span data-ttu-id="3ff87-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ff87-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ff87-112">列出 mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="3ff87-112">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="3ff87-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ff87-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="3ff87-114">列出 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ff87-114">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="3ff87-115">获取 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-115">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="3ff87-116">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-116">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="3ff87-117">读取 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ff87-117">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="3ff87-118">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-118">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="3ff87-119">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-119">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="3ff87-120">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ff87-120">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="3ff87-121">删除 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-121">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="3ff87-122">无</span><span class="sxs-lookup"><span data-stu-id="3ff87-122">None</span></span>|<span data-ttu-id="3ff87-123">删除 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="3ff87-123">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="3ff87-124">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-124">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="3ff87-125">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="3ff87-125">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="3ff87-126">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3ff87-126">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ff87-127">属性</span><span class="sxs-lookup"><span data-stu-id="3ff87-127">Properties</span></span>
|<span data-ttu-id="3ff87-128">属性</span><span class="sxs-lookup"><span data-stu-id="3ff87-128">Property</span></span>|<span data-ttu-id="3ff87-129">类型</span><span class="sxs-lookup"><span data-stu-id="3ff87-129">Type</span></span>|<span data-ttu-id="3ff87-130">说明</span><span class="sxs-lookup"><span data-stu-id="3ff87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff87-131">id</span><span class="sxs-lookup"><span data-stu-id="3ff87-131">id</span></span>|<span data-ttu-id="3ff87-132">String</span><span class="sxs-lookup"><span data-stu-id="3ff87-132">String</span></span>|<span data-ttu-id="3ff87-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3ff87-133">The key of the entity.</span></span>|
|<span data-ttu-id="3ff87-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff87-134">displayName</span></span>|<span data-ttu-id="3ff87-135">String</span><span class="sxs-lookup"><span data-stu-id="3ff87-135">String</span></span>|<span data-ttu-id="3ff87-136">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="3ff87-136">The name of the app category.</span></span>|
|<span data-ttu-id="3ff87-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff87-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3ff87-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff87-138">DateTimeOffset</span></span>|<span data-ttu-id="3ff87-139">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3ff87-139">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ff87-140">关系</span><span class="sxs-lookup"><span data-stu-id="3ff87-140">Relationships</span></span>
<span data-ttu-id="3ff87-141">无</span><span class="sxs-lookup"><span data-stu-id="3ff87-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ff87-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ff87-142">JSON Representation</span></span>
<span data-ttu-id="3ff87-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ff87-143">Here is a JSON representation of the resource.</span></span>
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




