---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: 将 Windows Autopilot 部署配置文件分配给 AAD 组。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b11c464e3a1e69b7580f2458277abe77d593af75
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783394"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="a7c1b-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7c1b-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="a7c1b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7c1b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c1b-106">将 Windows Autopilot 部署配置文件分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-106">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="a7c1b-107">方法</span><span class="sxs-lookup"><span data-stu-id="a7c1b-107">Methods</span></span>
|<span data-ttu-id="a7c1b-108">方法</span><span class="sxs-lookup"><span data-stu-id="a7c1b-108">Method</span></span>|<span data-ttu-id="a7c1b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7c1b-109">Return Type</span></span>|<span data-ttu-id="a7c1b-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7c1b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7c1b-111">列出 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="a7c1b-111">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="a7c1b-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a7c1b-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="a7c1b-113">列出[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-113">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="a7c1b-114">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-114">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="a7c1b-115">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-115">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="a7c1b-116">读取[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-116">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="a7c1b-117">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-117">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="a7c1b-118">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-118">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="a7c1b-119">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-119">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="a7c1b-120">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-120">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="a7c1b-121">None</span><span class="sxs-lookup"><span data-stu-id="a7c1b-121">None</span></span>|<span data-ttu-id="a7c1b-122">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-122">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="a7c1b-123">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-123">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="a7c1b-124">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="a7c1b-124">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="a7c1b-125">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-125">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7c1b-126">属性</span><span class="sxs-lookup"><span data-stu-id="a7c1b-126">Properties</span></span>
|<span data-ttu-id="a7c1b-127">属性</span><span class="sxs-lookup"><span data-stu-id="a7c1b-127">Property</span></span>|<span data-ttu-id="a7c1b-128">类型</span><span class="sxs-lookup"><span data-stu-id="a7c1b-128">Type</span></span>|<span data-ttu-id="a7c1b-129">说明</span><span class="sxs-lookup"><span data-stu-id="a7c1b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c1b-130">id</span><span class="sxs-lookup"><span data-stu-id="a7c1b-130">id</span></span>|<span data-ttu-id="a7c1b-131">String</span><span class="sxs-lookup"><span data-stu-id="a7c1b-131">String</span></span>|<span data-ttu-id="a7c1b-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-132">The key of the assignment.</span></span>|
|<span data-ttu-id="a7c1b-133">target</span><span class="sxs-lookup"><span data-stu-id="a7c1b-133">target</span></span>|[<span data-ttu-id="a7c1b-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a7c1b-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a7c1b-135">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-135">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="a7c1b-136">source</span><span class="sxs-lookup"><span data-stu-id="a7c1b-136">source</span></span>|[<span data-ttu-id="a7c1b-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a7c1b-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a7c1b-138">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-138">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="a7c1b-139">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a7c1b-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="a7c1b-140">sourceId</span></span>|<span data-ttu-id="a7c1b-141">String</span><span class="sxs-lookup"><span data-stu-id="a7c1b-141">String</span></span>|<span data-ttu-id="a7c1b-142">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="a7c1b-142">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c1b-143">关系</span><span class="sxs-lookup"><span data-stu-id="a7c1b-143">Relationships</span></span>
<span data-ttu-id="a7c1b-144">无</span><span class="sxs-lookup"><span data-stu-id="a7c1b-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7c1b-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7c1b-145">JSON Representation</span></span>
<span data-ttu-id="a7c1b-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7c1b-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



