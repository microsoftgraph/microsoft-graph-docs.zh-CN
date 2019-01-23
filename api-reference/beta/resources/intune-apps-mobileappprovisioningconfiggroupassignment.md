---
title: mobileAppProvisioningConfigGroupAssignment 资源类型
description: 包含用于分配给组应用程序设置配置的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ad07112031ce8ebe46d48c2c5fa51f0744a2bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421926"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="00501-103">mobileAppProvisioningConfigGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="00501-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="00501-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="00501-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00501-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00501-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00501-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00501-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00501-107">包含用于分配给组应用程序设置配置的属性。</span><span class="sxs-lookup"><span data-stu-id="00501-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="00501-108">方法</span><span class="sxs-lookup"><span data-stu-id="00501-108">Methods</span></span>
|<span data-ttu-id="00501-109">方法</span><span class="sxs-lookup"><span data-stu-id="00501-109">Method</span></span>|<span data-ttu-id="00501-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="00501-110">Return Type</span></span>|<span data-ttu-id="00501-111">说明</span><span class="sxs-lookup"><span data-stu-id="00501-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00501-112">列表 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="00501-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="00501-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="00501-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="00501-114">列出属性和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="00501-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="00501-115">获取 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="00501-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="00501-117">读取属性和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="00501-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="00501-118">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="00501-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="00501-120">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="00501-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="00501-121">删除 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="00501-122">无</span><span class="sxs-lookup"><span data-stu-id="00501-122">None</span></span>|<span data-ttu-id="00501-123">删除[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="00501-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="00501-124">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="00501-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="00501-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="00501-126">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00501-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00501-127">属性</span><span class="sxs-lookup"><span data-stu-id="00501-127">Properties</span></span>
|<span data-ttu-id="00501-128">属性</span><span class="sxs-lookup"><span data-stu-id="00501-128">Property</span></span>|<span data-ttu-id="00501-129">类型</span><span class="sxs-lookup"><span data-stu-id="00501-129">Type</span></span>|<span data-ttu-id="00501-130">说明</span><span class="sxs-lookup"><span data-stu-id="00501-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00501-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="00501-131">targetGroupId</span></span>|<span data-ttu-id="00501-132">String</span><span class="sxs-lookup"><span data-stu-id="00501-132">String</span></span>|<span data-ttu-id="00501-133">AAD 组顺序为目标应用程序设置配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="00501-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="00501-134">id</span><span class="sxs-lookup"><span data-stu-id="00501-134">id</span></span>|<span data-ttu-id="00501-135">String</span><span class="sxs-lookup"><span data-stu-id="00501-135">String</span></span>|<span data-ttu-id="00501-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="00501-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00501-137">关系</span><span class="sxs-lookup"><span data-stu-id="00501-137">Relationships</span></span>
<span data-ttu-id="00501-138">无</span><span class="sxs-lookup"><span data-stu-id="00501-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00501-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00501-139">JSON Representation</span></span>
<span data-ttu-id="00501-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00501-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```




