---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3671665c40fb141ddfebe231e3408a94449990eb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866669"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="86a7f-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="86a7f-104">deviceCategory resource type</span></span>

<span data-ttu-id="86a7f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a7f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86a7f-106">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86a7f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a7f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86a7f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a7f-108">设备类别提供了一种组织设备的方法。</span><span class="sxs-lookup"><span data-stu-id="86a7f-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="86a7f-109">使用设备类别，公司管理员可以定义对公司有意义的独特类别。</span><span class="sxs-lookup"><span data-stu-id="86a7f-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span> <span data-ttu-id="86a7f-110">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="86a7f-110">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="86a7f-111">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="86a7f-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="86a7f-112">方法</span><span class="sxs-lookup"><span data-stu-id="86a7f-112">Methods</span></span>
|<span data-ttu-id="86a7f-113">方法</span><span class="sxs-lookup"><span data-stu-id="86a7f-113">Method</span></span>|<span data-ttu-id="86a7f-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="86a7f-114">Return Type</span></span>|<span data-ttu-id="86a7f-115">说明</span><span class="sxs-lookup"><span data-stu-id="86a7f-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86a7f-116">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="86a7f-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="86a7f-117">[deviceCategory](../resources/intune-shared-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86a7f-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="86a7f-118">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86a7f-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="86a7f-119">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="86a7f-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="86a7f-121">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86a7f-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="86a7f-122">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="86a7f-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="86a7f-124">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86a7f-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="86a7f-125">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="86a7f-126">无</span><span class="sxs-lookup"><span data-stu-id="86a7f-126">None</span></span>|<span data-ttu-id="86a7f-127">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="86a7f-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="86a7f-128">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="86a7f-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="86a7f-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="86a7f-130">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86a7f-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86a7f-131">属性</span><span class="sxs-lookup"><span data-stu-id="86a7f-131">Properties</span></span>
|<span data-ttu-id="86a7f-132">属性</span><span class="sxs-lookup"><span data-stu-id="86a7f-132">Property</span></span>|<span data-ttu-id="86a7f-133">类型</span><span class="sxs-lookup"><span data-stu-id="86a7f-133">Type</span></span>|<span data-ttu-id="86a7f-134">说明</span><span class="sxs-lookup"><span data-stu-id="86a7f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a7f-135">id</span><span class="sxs-lookup"><span data-stu-id="86a7f-135">id</span></span>|<span data-ttu-id="86a7f-136">String</span><span class="sxs-lookup"><span data-stu-id="86a7f-136">String</span></span>|<span data-ttu-id="86a7f-137">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="86a7f-137">Unique identifier for the device category.</span></span> <span data-ttu-id="86a7f-138">只读。</span><span class="sxs-lookup"><span data-stu-id="86a7f-138">Read-only.</span></span>|
|<span data-ttu-id="86a7f-139">**载入**</span><span class="sxs-lookup"><span data-stu-id="86a7f-139">**Onboarding**</span></span>|
|<span data-ttu-id="86a7f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="86a7f-140">displayName</span></span>|<span data-ttu-id="86a7f-141">String</span><span class="sxs-lookup"><span data-stu-id="86a7f-141">String</span></span>|<span data-ttu-id="86a7f-142">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="86a7f-142">Display name for the device category.</span></span>|
|<span data-ttu-id="86a7f-143">说明</span><span class="sxs-lookup"><span data-stu-id="86a7f-143">description</span></span>|<span data-ttu-id="86a7f-144">String</span><span class="sxs-lookup"><span data-stu-id="86a7f-144">String</span></span>|<span data-ttu-id="86a7f-145">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="86a7f-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86a7f-146">关系</span><span class="sxs-lookup"><span data-stu-id="86a7f-146">Relationships</span></span>
<span data-ttu-id="86a7f-147">无</span><span class="sxs-lookup"><span data-stu-id="86a7f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86a7f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86a7f-148">JSON Representation</span></span>
<span data-ttu-id="86a7f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86a7f-149">Here is a JSON representation of the resource.</span></span>
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




