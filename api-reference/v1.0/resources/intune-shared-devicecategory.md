---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732363"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="0bd9b-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bd9b-104">deviceCategory resource type</span></span>

<span data-ttu-id="0bd9b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bd9b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bd9b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd9b-107">设备类别提供了整理设备的方法。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-107">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="0bd9b-108">公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-108">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="0bd9b-109">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-109">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="0bd9b-110">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="0bd9b-111">Methods</span><span class="sxs-lookup"><span data-stu-id="0bd9b-111">Methods</span></span>
|<span data-ttu-id="0bd9b-112">方法</span><span class="sxs-lookup"><span data-stu-id="0bd9b-112">Method</span></span>|<span data-ttu-id="0bd9b-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0bd9b-113">Return Type</span></span>|<span data-ttu-id="0bd9b-114">Description</span><span class="sxs-lookup"><span data-stu-id="0bd9b-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd9b-115">[列出 deviceCategories](../api/intune-shared-devicecategory-list.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0bd9b-115">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="0bd9b-116">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-116">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="0bd9b-117">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0bd9b-117">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="0bd9b-118">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-118">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="0bd9b-119">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0bd9b-119">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="0bd9b-120">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-120">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="0bd9b-121">[删除 deviceCategory](../api/intune-shared-devicecategory-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-121">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="0bd9b-122">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0bd9b-122">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="0bd9b-123">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-123">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0bd9b-124">属性</span><span class="sxs-lookup"><span data-stu-id="0bd9b-124">Properties</span></span>
|<span data-ttu-id="0bd9b-125">属性</span><span class="sxs-lookup"><span data-stu-id="0bd9b-125">Property</span></span>|<span data-ttu-id="0bd9b-126">类型</span><span class="sxs-lookup"><span data-stu-id="0bd9b-126">Type</span></span>|<span data-ttu-id="0bd9b-127">说明</span><span class="sxs-lookup"><span data-stu-id="0bd9b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd9b-128">id</span><span class="sxs-lookup"><span data-stu-id="0bd9b-128">id</span></span>|<span data-ttu-id="0bd9b-129">String</span><span class="sxs-lookup"><span data-stu-id="0bd9b-129">String</span></span>|<span data-ttu-id="0bd9b-130">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-130">Unique identifier for the device category.</span></span> <span data-ttu-id="0bd9b-131">只读。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-131">Read-only.</span></span>|
|<span data-ttu-id="0bd9b-132">**载入**</span><span class="sxs-lookup"><span data-stu-id="0bd9b-132">**Onboarding**</span></span>|
|<span data-ttu-id="0bd9b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0bd9b-133">displayName</span></span>|<span data-ttu-id="0bd9b-134">String</span><span class="sxs-lookup"><span data-stu-id="0bd9b-134">String</span></span>|<span data-ttu-id="0bd9b-135">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-135">Display name for the device category.</span></span>|
|<span data-ttu-id="0bd9b-136">说明</span><span class="sxs-lookup"><span data-stu-id="0bd9b-136">description</span></span>|<span data-ttu-id="0bd9b-137">String</span><span class="sxs-lookup"><span data-stu-id="0bd9b-137">String</span></span>|<span data-ttu-id="0bd9b-138">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-138">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bd9b-139">关系</span><span class="sxs-lookup"><span data-stu-id="0bd9b-139">Relationships</span></span>
<span data-ttu-id="0bd9b-140">无</span><span class="sxs-lookup"><span data-stu-id="0bd9b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bd9b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bd9b-141">JSON Representation</span></span>
<span data-ttu-id="0bd9b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bd9b-142">Here is a JSON representation of the resource.</span></span>
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









