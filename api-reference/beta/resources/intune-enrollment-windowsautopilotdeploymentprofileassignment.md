---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: 将 Windows Autopilot 部署配置文件分配给 AAD 组。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb1c9cf2f69182c13121907696547464150ec7e6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460676"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="10a4d-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="10a4d-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

<span data-ttu-id="10a4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10a4d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10a4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10a4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10a4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10a4d-107">将 Windows Autopilot 部署配置文件分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="10a4d-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="10a4d-108">方法</span><span class="sxs-lookup"><span data-stu-id="10a4d-108">Methods</span></span>
|<span data-ttu-id="10a4d-109">方法</span><span class="sxs-lookup"><span data-stu-id="10a4d-109">Method</span></span>|<span data-ttu-id="10a4d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="10a4d-110">Return Type</span></span>|<span data-ttu-id="10a4d-111">说明</span><span class="sxs-lookup"><span data-stu-id="10a4d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10a4d-112">列出 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="10a4d-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="10a4d-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="10a4d-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="10a4d-114">列出[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10a4d-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="10a4d-115">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="10a4d-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="10a4d-117">读取[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10a4d-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="10a4d-118">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="10a4d-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="10a4d-120">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10a4d-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="10a4d-121">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="10a4d-122">无</span><span class="sxs-lookup"><span data-stu-id="10a4d-122">None</span></span>|<span data-ttu-id="10a4d-123">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="10a4d-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="10a4d-124">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="10a4d-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="10a4d-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="10a4d-126">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10a4d-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10a4d-127">属性</span><span class="sxs-lookup"><span data-stu-id="10a4d-127">Properties</span></span>
|<span data-ttu-id="10a4d-128">属性</span><span class="sxs-lookup"><span data-stu-id="10a4d-128">Property</span></span>|<span data-ttu-id="10a4d-129">类型</span><span class="sxs-lookup"><span data-stu-id="10a4d-129">Type</span></span>|<span data-ttu-id="10a4d-130">说明</span><span class="sxs-lookup"><span data-stu-id="10a4d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a4d-131">id</span><span class="sxs-lookup"><span data-stu-id="10a4d-131">id</span></span>|<span data-ttu-id="10a4d-132">String</span><span class="sxs-lookup"><span data-stu-id="10a4d-132">String</span></span>|<span data-ttu-id="10a4d-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="10a4d-133">The key of the assignment.</span></span>|
|<span data-ttu-id="10a4d-134">target</span><span class="sxs-lookup"><span data-stu-id="10a4d-134">target</span></span>|[<span data-ttu-id="10a4d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="10a4d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="10a4d-136">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="10a4d-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="10a4d-137">source</span><span class="sxs-lookup"><span data-stu-id="10a4d-137">source</span></span>|[<span data-ttu-id="10a4d-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="10a4d-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="10a4d-139">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="10a4d-139">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="10a4d-140">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="10a4d-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="10a4d-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="10a4d-141">sourceId</span></span>|<span data-ttu-id="10a4d-142">String</span><span class="sxs-lookup"><span data-stu-id="10a4d-142">String</span></span>|<span data-ttu-id="10a4d-143">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="10a4d-143">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="10a4d-144">关系</span><span class="sxs-lookup"><span data-stu-id="10a4d-144">Relationships</span></span>
<span data-ttu-id="10a4d-145">无</span><span class="sxs-lookup"><span data-stu-id="10a4d-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10a4d-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10a4d-146">JSON Representation</span></span>
<span data-ttu-id="10a4d-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10a4d-147">Here is a JSON representation of the resource.</span></span>
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



