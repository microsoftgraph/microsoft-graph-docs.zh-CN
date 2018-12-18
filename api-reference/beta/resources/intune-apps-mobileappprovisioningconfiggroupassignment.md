---
title: mobileAppProvisioningConfigGroupAssignment 资源类型
description: 包含用于分配给组应用程序设置配置的属性。
author: tfitzmac
ms.openlocfilehash: c38faf3f8de9aea79667664051bba6e45c83c238
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356481"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="12fc1-103">mobileAppProvisioningConfigGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="12fc1-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="12fc1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12fc1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12fc1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12fc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12fc1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12fc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12fc1-107">包含用于分配给组应用程序设置配置的属性。</span><span class="sxs-lookup"><span data-stu-id="12fc1-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="12fc1-108">方法</span><span class="sxs-lookup"><span data-stu-id="12fc1-108">Methods</span></span>
|<span data-ttu-id="12fc1-109">方法</span><span class="sxs-lookup"><span data-stu-id="12fc1-109">Method</span></span>|<span data-ttu-id="12fc1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="12fc1-110">Return Type</span></span>|<span data-ttu-id="12fc1-111">说明</span><span class="sxs-lookup"><span data-stu-id="12fc1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12fc1-112">列表 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="12fc1-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="12fc1-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="12fc1-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="12fc1-114">列出属性和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="12fc1-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="12fc1-115">获取 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="12fc1-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="12fc1-117">读取属性和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="12fc1-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="12fc1-118">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="12fc1-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="12fc1-120">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12fc1-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="12fc1-121">删除 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="12fc1-122">无</span><span class="sxs-lookup"><span data-stu-id="12fc1-122">None</span></span>|<span data-ttu-id="12fc1-123">删除[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="12fc1-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="12fc1-124">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="12fc1-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="12fc1-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="12fc1-126">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12fc1-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12fc1-127">属性</span><span class="sxs-lookup"><span data-stu-id="12fc1-127">Properties</span></span>
|<span data-ttu-id="12fc1-128">属性</span><span class="sxs-lookup"><span data-stu-id="12fc1-128">Property</span></span>|<span data-ttu-id="12fc1-129">类型</span><span class="sxs-lookup"><span data-stu-id="12fc1-129">Type</span></span>|<span data-ttu-id="12fc1-130">说明</span><span class="sxs-lookup"><span data-stu-id="12fc1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12fc1-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="12fc1-131">targetGroupId</span></span>|<span data-ttu-id="12fc1-132">字符串</span><span class="sxs-lookup"><span data-stu-id="12fc1-132">String</span></span>|<span data-ttu-id="12fc1-133">AAD 组顺序为目标应用程序设置配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="12fc1-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="12fc1-134">id</span><span class="sxs-lookup"><span data-stu-id="12fc1-134">id</span></span>|<span data-ttu-id="12fc1-135">String</span><span class="sxs-lookup"><span data-stu-id="12fc1-135">String</span></span>|<span data-ttu-id="12fc1-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12fc1-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12fc1-137">关系</span><span class="sxs-lookup"><span data-stu-id="12fc1-137">Relationships</span></span>
<span data-ttu-id="12fc1-138">无</span><span class="sxs-lookup"><span data-stu-id="12fc1-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12fc1-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12fc1-139">JSON Representation</span></span>
<span data-ttu-id="12fc1-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12fc1-140">Here is a JSON representation of the resource.</span></span>
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





