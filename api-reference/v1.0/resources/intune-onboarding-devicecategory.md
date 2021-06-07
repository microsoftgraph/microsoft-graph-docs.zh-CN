---
title: deviceCategory 资源类型
description: 设备类别提供了整理设备的方法。 公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5def5ee6c6a97e91c9255a9808db7fc6b2fa07fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751836"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="0922e-106">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="0922e-106">deviceCategory resource type</span></span>

<span data-ttu-id="0922e-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0922e-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0922e-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0922e-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0922e-109">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="0922e-109">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="0922e-110">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="0922e-110">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="0922e-111">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="0922e-111">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="0922e-112">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="0922e-112">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="0922e-113">方法</span><span class="sxs-lookup"><span data-stu-id="0922e-113">Methods</span></span>
|<span data-ttu-id="0922e-114">方法</span><span class="sxs-lookup"><span data-stu-id="0922e-114">Method</span></span>|<span data-ttu-id="0922e-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="0922e-115">Return Type</span></span>|<span data-ttu-id="0922e-116">说明</span><span class="sxs-lookup"><span data-stu-id="0922e-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0922e-117">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="0922e-117">List deviceCategories</span></span>](../api/intune-onboarding-devicecategory-list.md)|<span data-ttu-id="0922e-118">[deviceCategory](../resources/intune-onboarding-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0922e-118">[deviceCategory](../resources/intune-onboarding-devicecategory.md) collection</span></span>|<span data-ttu-id="0922e-119">列出 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0922e-119">List properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="0922e-120">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-120">Get deviceCategory</span></span>](../api/intune-onboarding-devicecategory-get.md)|[<span data-ttu-id="0922e-121">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-121">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="0922e-122">读取 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0922e-122">Read properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="0922e-123">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-123">Create deviceCategory</span></span>](../api/intune-onboarding-devicecategory-create.md)|[<span data-ttu-id="0922e-124">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-124">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="0922e-125">创建新的 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0922e-125">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="0922e-126">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-126">Delete deviceCategory</span></span>](../api/intune-onboarding-devicecategory-delete.md)|<span data-ttu-id="0922e-127">无</span><span class="sxs-lookup"><span data-stu-id="0922e-127">None</span></span>|<span data-ttu-id="0922e-128">删除 [deviceCategory](../resources/intune-onboarding-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="0922e-128">Deletes a [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span></span>|
|[<span data-ttu-id="0922e-129">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-129">Update deviceCategory</span></span>](../api/intune-onboarding-devicecategory-update.md)|[<span data-ttu-id="0922e-130">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0922e-130">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="0922e-131">更新 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0922e-131">Update the properties of a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0922e-132">属性</span><span class="sxs-lookup"><span data-stu-id="0922e-132">Properties</span></span>
|<span data-ttu-id="0922e-133">属性</span><span class="sxs-lookup"><span data-stu-id="0922e-133">Property</span></span>|<span data-ttu-id="0922e-134">类型</span><span class="sxs-lookup"><span data-stu-id="0922e-134">Type</span></span>|<span data-ttu-id="0922e-135">说明</span><span class="sxs-lookup"><span data-stu-id="0922e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0922e-136">id</span><span class="sxs-lookup"><span data-stu-id="0922e-136">id</span></span>|<span data-ttu-id="0922e-137">String</span><span class="sxs-lookup"><span data-stu-id="0922e-137">String</span></span>|<span data-ttu-id="0922e-138">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0922e-138">Unique identifier for the device category.</span></span> <span data-ttu-id="0922e-139">只读。</span><span class="sxs-lookup"><span data-stu-id="0922e-139">Read-only.</span></span>|
|<span data-ttu-id="0922e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0922e-140">displayName</span></span>|<span data-ttu-id="0922e-141">String</span><span class="sxs-lookup"><span data-stu-id="0922e-141">String</span></span>|<span data-ttu-id="0922e-142">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0922e-142">Display name for the device category.</span></span>|
|<span data-ttu-id="0922e-143">description</span><span class="sxs-lookup"><span data-stu-id="0922e-143">description</span></span>|<span data-ttu-id="0922e-144">String</span><span class="sxs-lookup"><span data-stu-id="0922e-144">String</span></span>|<span data-ttu-id="0922e-145">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="0922e-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0922e-146">关系</span><span class="sxs-lookup"><span data-stu-id="0922e-146">Relationships</span></span>
<span data-ttu-id="0922e-147">无</span><span class="sxs-lookup"><span data-stu-id="0922e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0922e-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0922e-148">JSON Representation</span></span>
<span data-ttu-id="0922e-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0922e-149">Here is a JSON representation of the resource.</span></span>
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




