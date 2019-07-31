---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 159b7e38db24a103989e22209baf9a6424b2c1b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967474"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="3029d-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="3029d-104">deviceCategory resource type</span></span>

> <span data-ttu-id="3029d-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3029d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3029d-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3029d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3029d-107">设备类别提供了一种组织设备的方法。</span><span class="sxs-lookup"><span data-stu-id="3029d-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="3029d-108">使用设备类别, 公司管理员可以定义对其公司有意义的独特类别。</span><span class="sxs-lookup"><span data-stu-id="3029d-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="3029d-109">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="3029d-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="3029d-110">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="3029d-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="3029d-111">方法</span><span class="sxs-lookup"><span data-stu-id="3029d-111">Methods</span></span>
|<span data-ttu-id="3029d-112">方法</span><span class="sxs-lookup"><span data-stu-id="3029d-112">Method</span></span>|<span data-ttu-id="3029d-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="3029d-113">Return Type</span></span>|<span data-ttu-id="3029d-114">说明</span><span class="sxs-lookup"><span data-stu-id="3029d-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3029d-115">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="3029d-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="3029d-116">[deviceCategory](../resources/intune-shared-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3029d-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="3029d-117">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3029d-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="3029d-118">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="3029d-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="3029d-120">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3029d-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="3029d-121">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="3029d-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="3029d-123">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3029d-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="3029d-124">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="3029d-125">无</span><span class="sxs-lookup"><span data-stu-id="3029d-125">None</span></span>|<span data-ttu-id="3029d-126">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="3029d-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="3029d-127">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="3029d-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3029d-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="3029d-129">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3029d-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3029d-130">属性</span><span class="sxs-lookup"><span data-stu-id="3029d-130">Properties</span></span>
|<span data-ttu-id="3029d-131">属性</span><span class="sxs-lookup"><span data-stu-id="3029d-131">Property</span></span>|<span data-ttu-id="3029d-132">类型</span><span class="sxs-lookup"><span data-stu-id="3029d-132">Type</span></span>|<span data-ttu-id="3029d-133">说明</span><span class="sxs-lookup"><span data-stu-id="3029d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3029d-134">id</span><span class="sxs-lookup"><span data-stu-id="3029d-134">id</span></span>|<span data-ttu-id="3029d-135">字符串</span><span class="sxs-lookup"><span data-stu-id="3029d-135">String</span></span>|<span data-ttu-id="3029d-136">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3029d-136">Unique identifier for the device category.</span></span> <span data-ttu-id="3029d-137">只读。</span><span class="sxs-lookup"><span data-stu-id="3029d-137">Read-only.</span></span>|
|<span data-ttu-id="3029d-138">**载入**</span><span class="sxs-lookup"><span data-stu-id="3029d-138">**Onboarding**</span></span>|
|<span data-ttu-id="3029d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3029d-139">displayName</span></span>|<span data-ttu-id="3029d-140">String</span><span class="sxs-lookup"><span data-stu-id="3029d-140">String</span></span>|<span data-ttu-id="3029d-141">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3029d-141">Display name for the device category.</span></span>|
|<span data-ttu-id="3029d-142">说明</span><span class="sxs-lookup"><span data-stu-id="3029d-142">description</span></span>|<span data-ttu-id="3029d-143">String</span><span class="sxs-lookup"><span data-stu-id="3029d-143">String</span></span>|<span data-ttu-id="3029d-144">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="3029d-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3029d-145">关系</span><span class="sxs-lookup"><span data-stu-id="3029d-145">Relationships</span></span>
<span data-ttu-id="3029d-146">无</span><span class="sxs-lookup"><span data-stu-id="3029d-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3029d-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3029d-147">JSON Representation</span></span>
<span data-ttu-id="3029d-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3029d-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



