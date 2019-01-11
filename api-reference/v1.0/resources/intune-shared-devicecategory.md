---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80f8f1f36198ecfab1021e30cb2f28fa4377852c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810834"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="ed7e6-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed7e6-104">deviceCategory resource type</span></span>

> <span data-ttu-id="ed7e6-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed7e6-106">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="ed7e6-107">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="ed7e6-108">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="ed7e6-109">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="ed7e6-110">方法</span><span class="sxs-lookup"><span data-stu-id="ed7e6-110">Methods</span></span>
|<span data-ttu-id="ed7e6-111">方法</span><span class="sxs-lookup"><span data-stu-id="ed7e6-111">Method</span></span>|<span data-ttu-id="ed7e6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed7e6-112">Return Type</span></span>|<span data-ttu-id="ed7e6-113">说明</span><span class="sxs-lookup"><span data-stu-id="ed7e6-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed7e6-114">[列表 deviceCategories](../api/intune-shared-devicecategory-list.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed7e6-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="ed7e6-115">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="ed7e6-116">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ed7e6-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="ed7e6-117">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="ed7e6-118">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ed7e6-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="ed7e6-119">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="ed7e6-120">[删除 deviceCategory](../api/intune-shared-devicecategory-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="ed7e6-121">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ed7e6-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="ed7e6-122">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed7e6-123">属性</span><span class="sxs-lookup"><span data-stu-id="ed7e6-123">Properties</span></span>
|<span data-ttu-id="ed7e6-124">属性</span><span class="sxs-lookup"><span data-stu-id="ed7e6-124">Property</span></span>|<span data-ttu-id="ed7e6-125">类型</span><span class="sxs-lookup"><span data-stu-id="ed7e6-125">Type</span></span>|<span data-ttu-id="ed7e6-126">说明</span><span class="sxs-lookup"><span data-stu-id="ed7e6-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed7e6-127">id</span><span class="sxs-lookup"><span data-stu-id="ed7e6-127">id</span></span>|<span data-ttu-id="ed7e6-128">String</span><span class="sxs-lookup"><span data-stu-id="ed7e6-128">String</span></span>|<span data-ttu-id="ed7e6-129">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-129">Unique identifier for the device category.</span></span> <span data-ttu-id="ed7e6-130">只读。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-130">Read-only.</span></span>|
|<span data-ttu-id="ed7e6-131">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="ed7e6-131">**Onboarding**</span></span>|
|<span data-ttu-id="ed7e6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ed7e6-132">displayName</span></span>|<span data-ttu-id="ed7e6-133">String</span><span class="sxs-lookup"><span data-stu-id="ed7e6-133">String</span></span>|<span data-ttu-id="ed7e6-134">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-134">Display name for the device category.</span></span>|
|<span data-ttu-id="ed7e6-135">description</span><span class="sxs-lookup"><span data-stu-id="ed7e6-135">description</span></span>|<span data-ttu-id="ed7e6-136">String</span><span class="sxs-lookup"><span data-stu-id="ed7e6-136">String</span></span>|<span data-ttu-id="ed7e6-137">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed7e6-138">关系</span><span class="sxs-lookup"><span data-stu-id="ed7e6-138">Relationships</span></span>
<span data-ttu-id="ed7e6-139">无</span><span class="sxs-lookup"><span data-stu-id="ed7e6-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed7e6-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed7e6-140">JSON Representation</span></span>
<span data-ttu-id="ed7e6-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed7e6-141">Here is a JSON representation of the resource.</span></span>
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



