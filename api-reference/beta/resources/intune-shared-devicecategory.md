---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75fb11ef3b734e6d5d0490be1abc3c5399433a70
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525318"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="08069-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="08069-104">deviceCategory resource type</span></span>

> <span data-ttu-id="08069-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08069-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08069-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08069-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08069-107">设备类别提供了一种组织设备的方法。</span><span class="sxs-lookup"><span data-stu-id="08069-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="08069-108">使用设备类别, 公司管理员可以定义对其公司有意义的独特类别。</span><span class="sxs-lookup"><span data-stu-id="08069-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="08069-109">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="08069-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="08069-110">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="08069-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="08069-111">方法</span><span class="sxs-lookup"><span data-stu-id="08069-111">Methods</span></span>
|<span data-ttu-id="08069-112">方法</span><span class="sxs-lookup"><span data-stu-id="08069-112">Method</span></span>|<span data-ttu-id="08069-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="08069-113">Return Type</span></span>|<span data-ttu-id="08069-114">说明</span><span class="sxs-lookup"><span data-stu-id="08069-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08069-115">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="08069-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="08069-116">[deviceCategory](../resources/intune-shared-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08069-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="08069-117">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08069-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="08069-118">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="08069-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="08069-120">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08069-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="08069-121">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="08069-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="08069-123">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08069-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="08069-124">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="08069-125">无</span><span class="sxs-lookup"><span data-stu-id="08069-125">None</span></span>|<span data-ttu-id="08069-126">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="08069-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="08069-127">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="08069-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="08069-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="08069-129">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="08069-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08069-130">属性</span><span class="sxs-lookup"><span data-stu-id="08069-130">Properties</span></span>
|<span data-ttu-id="08069-131">属性</span><span class="sxs-lookup"><span data-stu-id="08069-131">Property</span></span>|<span data-ttu-id="08069-132">类型</span><span class="sxs-lookup"><span data-stu-id="08069-132">Type</span></span>|<span data-ttu-id="08069-133">说明</span><span class="sxs-lookup"><span data-stu-id="08069-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08069-134">id</span><span class="sxs-lookup"><span data-stu-id="08069-134">id</span></span>|<span data-ttu-id="08069-135">字符串</span><span class="sxs-lookup"><span data-stu-id="08069-135">String</span></span>|<span data-ttu-id="08069-136">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08069-136">Unique identifier for the device category.</span></span> <span data-ttu-id="08069-137">只读。</span><span class="sxs-lookup"><span data-stu-id="08069-137">Read-only.</span></span>|
|<span data-ttu-id="08069-138">**载入**</span><span class="sxs-lookup"><span data-stu-id="08069-138">**Onboarding**</span></span>|
|<span data-ttu-id="08069-139">displayName</span><span class="sxs-lookup"><span data-stu-id="08069-139">displayName</span></span>|<span data-ttu-id="08069-140">String</span><span class="sxs-lookup"><span data-stu-id="08069-140">String</span></span>|<span data-ttu-id="08069-141">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="08069-141">Display name for the device category.</span></span>|
|<span data-ttu-id="08069-142">description</span><span class="sxs-lookup"><span data-stu-id="08069-142">description</span></span>|<span data-ttu-id="08069-143">String</span><span class="sxs-lookup"><span data-stu-id="08069-143">String</span></span>|<span data-ttu-id="08069-144">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="08069-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08069-145">关系</span><span class="sxs-lookup"><span data-stu-id="08069-145">Relationships</span></span>
<span data-ttu-id="08069-146">无</span><span class="sxs-lookup"><span data-stu-id="08069-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08069-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08069-147">JSON Representation</span></span>
<span data-ttu-id="08069-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08069-148">Here is a JSON representation of the resource.</span></span>
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



