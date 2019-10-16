---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: 将 Windows Autopilot 部署配置文件分配给 AAD 组。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b988d32ccdbe5a553854a84351bbd216c42f7982
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539139"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="7a872-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a872-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="7a872-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a872-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a872-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a872-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a872-106">将 Windows Autopilot 部署配置文件分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="7a872-106">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="7a872-107">方法</span><span class="sxs-lookup"><span data-stu-id="7a872-107">Methods</span></span>
|<span data-ttu-id="7a872-108">方法</span><span class="sxs-lookup"><span data-stu-id="7a872-108">Method</span></span>|<span data-ttu-id="7a872-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a872-109">Return Type</span></span>|<span data-ttu-id="7a872-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a872-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a872-111">列出 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="7a872-111">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="7a872-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="7a872-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="7a872-113">列出[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a872-113">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="7a872-114">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-114">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="7a872-115">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-115">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="7a872-116">读取[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a872-116">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="7a872-117">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-117">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="7a872-118">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-118">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="7a872-119">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7a872-119">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="7a872-120">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-120">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="7a872-121">无</span><span class="sxs-lookup"><span data-stu-id="7a872-121">None</span></span>|<span data-ttu-id="7a872-122">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7a872-122">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="7a872-123">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-123">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="7a872-124">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7a872-124">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="7a872-125">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7a872-125">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a872-126">属性</span><span class="sxs-lookup"><span data-stu-id="7a872-126">Properties</span></span>
|<span data-ttu-id="7a872-127">属性</span><span class="sxs-lookup"><span data-stu-id="7a872-127">Property</span></span>|<span data-ttu-id="7a872-128">类型</span><span class="sxs-lookup"><span data-stu-id="7a872-128">Type</span></span>|<span data-ttu-id="7a872-129">说明</span><span class="sxs-lookup"><span data-stu-id="7a872-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a872-130">id</span><span class="sxs-lookup"><span data-stu-id="7a872-130">id</span></span>|<span data-ttu-id="7a872-131">字符串</span><span class="sxs-lookup"><span data-stu-id="7a872-131">String</span></span>|<span data-ttu-id="7a872-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="7a872-132">The key of the assignment.</span></span>|
|<span data-ttu-id="7a872-133">target</span><span class="sxs-lookup"><span data-stu-id="7a872-133">target</span></span>|[<span data-ttu-id="7a872-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7a872-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7a872-135">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="7a872-135">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="7a872-136">source</span><span class="sxs-lookup"><span data-stu-id="7a872-136">source</span></span>|[<span data-ttu-id="7a872-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="7a872-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="7a872-138">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="7a872-138">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="7a872-139">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="7a872-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="7a872-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="7a872-140">sourceId</span></span>|<span data-ttu-id="7a872-141">字符串</span><span class="sxs-lookup"><span data-stu-id="7a872-141">String</span></span>|<span data-ttu-id="7a872-142">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="7a872-142">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a872-143">关系</span><span class="sxs-lookup"><span data-stu-id="7a872-143">Relationships</span></span>
<span data-ttu-id="7a872-144">无</span><span class="sxs-lookup"><span data-stu-id="7a872-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a872-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a872-145">JSON Representation</span></span>
<span data-ttu-id="7a872-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a872-146">Here is a JSON representation of the resource.</span></span>
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



