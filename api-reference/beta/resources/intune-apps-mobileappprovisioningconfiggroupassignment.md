---
title: mobileAppProvisioningConfigGroupAssignment 资源类型
description: 包含用于向组分配应用程序设置配置的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6af0d2547e5e63ed887e31983046944630f8cdf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772207"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="353fe-103">mobileAppProvisioningConfigGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="353fe-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="353fe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="353fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="353fe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="353fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="353fe-106">包含用于向组分配应用程序设置配置的属性。</span><span class="sxs-lookup"><span data-stu-id="353fe-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="353fe-107">方法</span><span class="sxs-lookup"><span data-stu-id="353fe-107">Methods</span></span>
|<span data-ttu-id="353fe-108">方法</span><span class="sxs-lookup"><span data-stu-id="353fe-108">Method</span></span>|<span data-ttu-id="353fe-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="353fe-109">Return Type</span></span>|<span data-ttu-id="353fe-110">说明</span><span class="sxs-lookup"><span data-stu-id="353fe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="353fe-111">列出 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="353fe-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="353fe-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="353fe-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="353fe-113">列出[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="353fe-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="353fe-114">获取 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="353fe-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="353fe-116">读取[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="353fe-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="353fe-117">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="353fe-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="353fe-119">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="353fe-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="353fe-120">删除 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="353fe-121">无</span><span class="sxs-lookup"><span data-stu-id="353fe-121">None</span></span>|<span data-ttu-id="353fe-122">删除[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="353fe-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="353fe-123">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="353fe-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="353fe-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="353fe-125">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="353fe-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="353fe-126">属性</span><span class="sxs-lookup"><span data-stu-id="353fe-126">Properties</span></span>
|<span data-ttu-id="353fe-127">属性</span><span class="sxs-lookup"><span data-stu-id="353fe-127">Property</span></span>|<span data-ttu-id="353fe-128">类型</span><span class="sxs-lookup"><span data-stu-id="353fe-128">Type</span></span>|<span data-ttu-id="353fe-129">说明</span><span class="sxs-lookup"><span data-stu-id="353fe-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="353fe-130">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="353fe-130">targetGroupId</span></span>|<span data-ttu-id="353fe-131">String</span><span class="sxs-lookup"><span data-stu-id="353fe-131">String</span></span>|<span data-ttu-id="353fe-132">要在其中定向应用程序设置配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="353fe-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="353fe-133">id</span><span class="sxs-lookup"><span data-stu-id="353fe-133">id</span></span>|<span data-ttu-id="353fe-134">String</span><span class="sxs-lookup"><span data-stu-id="353fe-134">String</span></span>|<span data-ttu-id="353fe-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="353fe-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="353fe-136">关系</span><span class="sxs-lookup"><span data-stu-id="353fe-136">Relationships</span></span>
<span data-ttu-id="353fe-137">无</span><span class="sxs-lookup"><span data-stu-id="353fe-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="353fe-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="353fe-138">JSON Representation</span></span>
<span data-ttu-id="353fe-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="353fe-139">Here is a JSON representation of the resource.</span></span>
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





