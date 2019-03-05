---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a0bb1e994bcf42ba91a55fdfc75946204d1f9b06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254896"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="48e0a-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="48e0a-104">deviceCategory resource type</span></span>

> <span data-ttu-id="48e0a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48e0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e0a-106">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="48e0a-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="48e0a-107">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="48e0a-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="48e0a-108">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="48e0a-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="48e0a-109">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="48e0a-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="48e0a-110">方法</span><span class="sxs-lookup"><span data-stu-id="48e0a-110">Methods</span></span>
|<span data-ttu-id="48e0a-111">方法</span><span class="sxs-lookup"><span data-stu-id="48e0a-111">Method</span></span>|<span data-ttu-id="48e0a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="48e0a-112">Return Type</span></span>|<span data-ttu-id="48e0a-113">说明</span><span class="sxs-lookup"><span data-stu-id="48e0a-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e0a-114">[列出 deviceCategories](../api/intune-shared-devicecategory-list.md)集合</span><span class="sxs-lookup"><span data-stu-id="48e0a-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="48e0a-115">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48e0a-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="48e0a-116">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="48e0a-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="48e0a-117">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48e0a-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="48e0a-118">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="48e0a-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="48e0a-119">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48e0a-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="48e0a-120">[删除 deviceCategory](../api/intune-shared-devicecategory-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="48e0a-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="48e0a-121">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="48e0a-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="48e0a-122">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48e0a-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="48e0a-123">属性</span><span class="sxs-lookup"><span data-stu-id="48e0a-123">Properties</span></span>
|<span data-ttu-id="48e0a-124">属性</span><span class="sxs-lookup"><span data-stu-id="48e0a-124">Property</span></span>|<span data-ttu-id="48e0a-125">类型</span><span class="sxs-lookup"><span data-stu-id="48e0a-125">Type</span></span>|<span data-ttu-id="48e0a-126">说明</span><span class="sxs-lookup"><span data-stu-id="48e0a-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e0a-127">id</span><span class="sxs-lookup"><span data-stu-id="48e0a-127">id</span></span>|<span data-ttu-id="48e0a-128">String</span><span class="sxs-lookup"><span data-stu-id="48e0a-128">String</span></span>|<span data-ttu-id="48e0a-129">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="48e0a-129">Unique identifier for the device category.</span></span> <span data-ttu-id="48e0a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="48e0a-130">Read-only.</span></span>|
|<span data-ttu-id="48e0a-131">**载入**</span><span class="sxs-lookup"><span data-stu-id="48e0a-131">**Onboarding**</span></span>|
|<span data-ttu-id="48e0a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="48e0a-132">displayName</span></span>|<span data-ttu-id="48e0a-133">String</span><span class="sxs-lookup"><span data-stu-id="48e0a-133">String</span></span>|<span data-ttu-id="48e0a-134">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="48e0a-134">Display name for the device category.</span></span>|
|<span data-ttu-id="48e0a-135">description</span><span class="sxs-lookup"><span data-stu-id="48e0a-135">description</span></span>|<span data-ttu-id="48e0a-136">String</span><span class="sxs-lookup"><span data-stu-id="48e0a-136">String</span></span>|<span data-ttu-id="48e0a-137">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="48e0a-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48e0a-138">关系</span><span class="sxs-lookup"><span data-stu-id="48e0a-138">Relationships</span></span>
<span data-ttu-id="48e0a-139">无</span><span class="sxs-lookup"><span data-stu-id="48e0a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48e0a-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48e0a-140">JSON Representation</span></span>
<span data-ttu-id="48e0a-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48e0a-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



