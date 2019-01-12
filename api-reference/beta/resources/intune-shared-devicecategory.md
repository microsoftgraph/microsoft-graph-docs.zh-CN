---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 885609c4bbbd01a9bf295e7c49a2790ce51b2941
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922212"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="4c7ea-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c7ea-104">deviceCategory resource type</span></span>

> <span data-ttu-id="4c7ea-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c7ea-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c7ea-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c7ea-108">设备类别提供了一种方式来组织您的设备。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="4c7ea-109">使用设备类别，公司管理员可以定义对其公司有意义的唯一类别。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="4c7ea-110">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="4c7ea-111">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="4c7ea-112">方法</span><span class="sxs-lookup"><span data-stu-id="4c7ea-112">Methods</span></span>
|<span data-ttu-id="4c7ea-113">方法</span><span class="sxs-lookup"><span data-stu-id="4c7ea-113">Method</span></span>|<span data-ttu-id="4c7ea-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c7ea-114">Return Type</span></span>|<span data-ttu-id="4c7ea-115">说明</span><span class="sxs-lookup"><span data-stu-id="4c7ea-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c7ea-116">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="4c7ea-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="4c7ea-117">[deviceCategory](../resources/intune-shared-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c7ea-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="4c7ea-118">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="4c7ea-119">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="4c7ea-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="4c7ea-121">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="4c7ea-122">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="4c7ea-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="4c7ea-124">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="4c7ea-125">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="4c7ea-126">无</span><span class="sxs-lookup"><span data-stu-id="4c7ea-126">None</span></span>|<span data-ttu-id="4c7ea-127">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="4c7ea-128">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="4c7ea-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4c7ea-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="4c7ea-130">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c7ea-131">属性</span><span class="sxs-lookup"><span data-stu-id="4c7ea-131">Properties</span></span>
|<span data-ttu-id="4c7ea-132">属性</span><span class="sxs-lookup"><span data-stu-id="4c7ea-132">Property</span></span>|<span data-ttu-id="4c7ea-133">类型</span><span class="sxs-lookup"><span data-stu-id="4c7ea-133">Type</span></span>|<span data-ttu-id="4c7ea-134">说明</span><span class="sxs-lookup"><span data-stu-id="4c7ea-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c7ea-135">id</span><span class="sxs-lookup"><span data-stu-id="4c7ea-135">id</span></span>|<span data-ttu-id="4c7ea-136">String</span><span class="sxs-lookup"><span data-stu-id="4c7ea-136">String</span></span>|<span data-ttu-id="4c7ea-137">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-137">Unique identifier for the device category.</span></span> <span data-ttu-id="4c7ea-138">只读。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-138">Read-only.</span></span>|
|<span data-ttu-id="4c7ea-139">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="4c7ea-139">**Onboarding**</span></span>|
|<span data-ttu-id="4c7ea-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4c7ea-140">displayName</span></span>|<span data-ttu-id="4c7ea-141">String</span><span class="sxs-lookup"><span data-stu-id="4c7ea-141">String</span></span>|<span data-ttu-id="4c7ea-142">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-142">Display name for the device category.</span></span>|
|<span data-ttu-id="4c7ea-143">description</span><span class="sxs-lookup"><span data-stu-id="4c7ea-143">description</span></span>|<span data-ttu-id="4c7ea-144">String</span><span class="sxs-lookup"><span data-stu-id="4c7ea-144">String</span></span>|<span data-ttu-id="4c7ea-145">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c7ea-146">关系</span><span class="sxs-lookup"><span data-stu-id="4c7ea-146">Relationships</span></span>
<span data-ttu-id="4c7ea-147">无</span><span class="sxs-lookup"><span data-stu-id="4c7ea-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c7ea-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c7ea-148">JSON Representation</span></span>
<span data-ttu-id="4c7ea-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-149">Here is a JSON representation of the resource.</span></span>
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



