---
title: mobileAppProvisioningConfigGroupAssignment 资源类型
description: 包含用于向组分配应用程序设置配置的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bef09ef9a51ed1cdcc3fb534fee962bb93c5bb3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367454"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="4be11-103">mobileAppProvisioningConfigGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4be11-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="4be11-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4be11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4be11-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4be11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4be11-106">包含用于向组分配应用程序设置配置的属性。</span><span class="sxs-lookup"><span data-stu-id="4be11-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="4be11-107">方法</span><span class="sxs-lookup"><span data-stu-id="4be11-107">Methods</span></span>
|<span data-ttu-id="4be11-108">方法</span><span class="sxs-lookup"><span data-stu-id="4be11-108">Method</span></span>|<span data-ttu-id="4be11-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4be11-109">Return Type</span></span>|<span data-ttu-id="4be11-110">说明</span><span class="sxs-lookup"><span data-stu-id="4be11-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4be11-111">列出 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4be11-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="4be11-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="4be11-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="4be11-113">列出[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4be11-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="4be11-114">获取 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="4be11-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="4be11-116">读取[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4be11-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4be11-117">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="4be11-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="4be11-119">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4be11-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4be11-120">删除 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="4be11-121">无</span><span class="sxs-lookup"><span data-stu-id="4be11-121">None</span></span>|<span data-ttu-id="4be11-122">删除[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4be11-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="4be11-123">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="4be11-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4be11-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="4be11-125">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4be11-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4be11-126">属性</span><span class="sxs-lookup"><span data-stu-id="4be11-126">Properties</span></span>
|<span data-ttu-id="4be11-127">属性</span><span class="sxs-lookup"><span data-stu-id="4be11-127">Property</span></span>|<span data-ttu-id="4be11-128">类型</span><span class="sxs-lookup"><span data-stu-id="4be11-128">Type</span></span>|<span data-ttu-id="4be11-129">说明</span><span class="sxs-lookup"><span data-stu-id="4be11-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be11-130">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4be11-130">targetGroupId</span></span>|<span data-ttu-id="4be11-131">String</span><span class="sxs-lookup"><span data-stu-id="4be11-131">String</span></span>|<span data-ttu-id="4be11-132">要在其中定向应用程序设置配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="4be11-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="4be11-133">id</span><span class="sxs-lookup"><span data-stu-id="4be11-133">id</span></span>|<span data-ttu-id="4be11-134">String</span><span class="sxs-lookup"><span data-stu-id="4be11-134">String</span></span>|<span data-ttu-id="4be11-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4be11-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4be11-136">关系</span><span class="sxs-lookup"><span data-stu-id="4be11-136">Relationships</span></span>
<span data-ttu-id="4be11-137">无</span><span class="sxs-lookup"><span data-stu-id="4be11-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4be11-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4be11-138">JSON Representation</span></span>
<span data-ttu-id="4be11-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4be11-139">Here is a JSON representation of the resource.</span></span>
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



