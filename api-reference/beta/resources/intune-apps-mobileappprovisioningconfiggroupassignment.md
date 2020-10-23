---
title: mobileAppProvisioningConfigGroupAssignment 资源类型
description: 包含用于向组分配应用程序设置配置的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ceb7d2ec77f980ae9788aba930eb29b6db158338
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721495"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="47842-103">mobileAppProvisioningConfigGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="47842-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

<span data-ttu-id="47842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47842-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47842-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47842-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47842-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47842-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47842-107">包含用于向组分配应用程序设置配置的属性。</span><span class="sxs-lookup"><span data-stu-id="47842-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="47842-108">Methods</span><span class="sxs-lookup"><span data-stu-id="47842-108">Methods</span></span>
|<span data-ttu-id="47842-109">方法</span><span class="sxs-lookup"><span data-stu-id="47842-109">Method</span></span>|<span data-ttu-id="47842-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="47842-110">Return Type</span></span>|<span data-ttu-id="47842-111">说明</span><span class="sxs-lookup"><span data-stu-id="47842-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47842-112">列出 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="47842-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="47842-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47842-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="47842-114">列出 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47842-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="47842-115">获取 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="47842-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="47842-117">读取 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47842-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="47842-118">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="47842-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="47842-120">创建新的 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47842-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="47842-121">删除 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="47842-122">无</span><span class="sxs-lookup"><span data-stu-id="47842-122">None</span></span>|<span data-ttu-id="47842-123">删除 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="47842-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="47842-124">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="47842-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="47842-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="47842-126">更新 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47842-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47842-127">属性</span><span class="sxs-lookup"><span data-stu-id="47842-127">Properties</span></span>
|<span data-ttu-id="47842-128">属性</span><span class="sxs-lookup"><span data-stu-id="47842-128">Property</span></span>|<span data-ttu-id="47842-129">类型</span><span class="sxs-lookup"><span data-stu-id="47842-129">Type</span></span>|<span data-ttu-id="47842-130">说明</span><span class="sxs-lookup"><span data-stu-id="47842-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47842-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="47842-131">targetGroupId</span></span>|<span data-ttu-id="47842-132">String</span><span class="sxs-lookup"><span data-stu-id="47842-132">String</span></span>|<span data-ttu-id="47842-133">要在其中定向应用程序设置配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="47842-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="47842-134">id</span><span class="sxs-lookup"><span data-stu-id="47842-134">id</span></span>|<span data-ttu-id="47842-135">String</span><span class="sxs-lookup"><span data-stu-id="47842-135">String</span></span>|<span data-ttu-id="47842-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47842-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47842-137">关系</span><span class="sxs-lookup"><span data-stu-id="47842-137">Relationships</span></span>
<span data-ttu-id="47842-138">无</span><span class="sxs-lookup"><span data-stu-id="47842-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47842-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47842-139">JSON Representation</span></span>
<span data-ttu-id="47842-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47842-140">Here is a JSON representation of the resource.</span></span>
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





