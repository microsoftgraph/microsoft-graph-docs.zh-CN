---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7470f6cf0193474bfaff4f7444ed3df1d9453a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418860"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="b64bd-104">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="b64bd-104">deviceCategory resource type</span></span>

> <span data-ttu-id="b64bd-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b64bd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b64bd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b64bd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b64bd-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b64bd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b64bd-108">设备类别提供了一种方式来组织您的设备。</span><span class="sxs-lookup"><span data-stu-id="b64bd-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="b64bd-109">使用设备类别，公司管理员可以定义对其公司有意义的唯一类别。</span><span class="sxs-lookup"><span data-stu-id="b64bd-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="b64bd-110">然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。</span><span class="sxs-lookup"><span data-stu-id="b64bd-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="b64bd-111">可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。</span><span class="sxs-lookup"><span data-stu-id="b64bd-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="b64bd-112">方法</span><span class="sxs-lookup"><span data-stu-id="b64bd-112">Methods</span></span>
|<span data-ttu-id="b64bd-113">方法</span><span class="sxs-lookup"><span data-stu-id="b64bd-113">Method</span></span>|<span data-ttu-id="b64bd-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="b64bd-114">Return Type</span></span>|<span data-ttu-id="b64bd-115">说明</span><span class="sxs-lookup"><span data-stu-id="b64bd-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b64bd-116">List deviceCategories</span><span class="sxs-lookup"><span data-stu-id="b64bd-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="b64bd-117">[deviceCategory](../resources/intune-shared-devicecategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b64bd-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="b64bd-118">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b64bd-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="b64bd-119">Get deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="b64bd-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b64bd-121">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b64bd-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b64bd-122">Create deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="b64bd-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b64bd-124">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b64bd-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b64bd-125">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="b64bd-126">无</span><span class="sxs-lookup"><span data-stu-id="b64bd-126">None</span></span>|<span data-ttu-id="b64bd-127">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="b64bd-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="b64bd-128">Update deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="b64bd-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b64bd-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b64bd-130">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b64bd-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b64bd-131">属性</span><span class="sxs-lookup"><span data-stu-id="b64bd-131">Properties</span></span>
|<span data-ttu-id="b64bd-132">属性</span><span class="sxs-lookup"><span data-stu-id="b64bd-132">Property</span></span>|<span data-ttu-id="b64bd-133">类型</span><span class="sxs-lookup"><span data-stu-id="b64bd-133">Type</span></span>|<span data-ttu-id="b64bd-134">说明</span><span class="sxs-lookup"><span data-stu-id="b64bd-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b64bd-135">id</span><span class="sxs-lookup"><span data-stu-id="b64bd-135">id</span></span>|<span data-ttu-id="b64bd-136">String</span><span class="sxs-lookup"><span data-stu-id="b64bd-136">String</span></span>|<span data-ttu-id="b64bd-137">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b64bd-137">Unique identifier for the device category.</span></span> <span data-ttu-id="b64bd-138">只读。</span><span class="sxs-lookup"><span data-stu-id="b64bd-138">Read-only.</span></span>|
|<span data-ttu-id="b64bd-139">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="b64bd-139">**Onboarding**</span></span>|
|<span data-ttu-id="b64bd-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b64bd-140">displayName</span></span>|<span data-ttu-id="b64bd-141">String</span><span class="sxs-lookup"><span data-stu-id="b64bd-141">String</span></span>|<span data-ttu-id="b64bd-142">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b64bd-142">Display name for the device category.</span></span>|
|<span data-ttu-id="b64bd-143">description</span><span class="sxs-lookup"><span data-stu-id="b64bd-143">description</span></span>|<span data-ttu-id="b64bd-144">String</span><span class="sxs-lookup"><span data-stu-id="b64bd-144">String</span></span>|<span data-ttu-id="b64bd-145">设备类别的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="b64bd-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b64bd-146">关系</span><span class="sxs-lookup"><span data-stu-id="b64bd-146">Relationships</span></span>
<span data-ttu-id="b64bd-147">无</span><span class="sxs-lookup"><span data-stu-id="b64bd-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b64bd-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b64bd-148">JSON Representation</span></span>
<span data-ttu-id="b64bd-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b64bd-149">Here is a JSON representation of the resource.</span></span>
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



