---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: 将 Windows Autopilot 部署配置文件分配给 AAD 组。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d148be78cdef4208cc06a1d5e3f4b698dc5850ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999050"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="25712-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="25712-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="25712-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25712-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25712-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25712-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25712-106">将 Windows Autopilot 部署配置文件分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="25712-106">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="25712-107">方法</span><span class="sxs-lookup"><span data-stu-id="25712-107">Methods</span></span>
|<span data-ttu-id="25712-108">方法</span><span class="sxs-lookup"><span data-stu-id="25712-108">Method</span></span>|<span data-ttu-id="25712-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="25712-109">Return Type</span></span>|<span data-ttu-id="25712-110">说明</span><span class="sxs-lookup"><span data-stu-id="25712-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25712-111">列出 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="25712-111">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="25712-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="25712-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="25712-113">列出[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25712-113">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="25712-114">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-114">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="25712-115">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-115">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="25712-116">读取[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25712-116">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="25712-117">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-117">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="25712-118">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-118">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="25712-119">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25712-119">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="25712-120">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-120">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="25712-121">无</span><span class="sxs-lookup"><span data-stu-id="25712-121">None</span></span>|<span data-ttu-id="25712-122">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="25712-122">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="25712-123">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-123">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="25712-124">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="25712-124">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="25712-125">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="25712-125">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25712-126">属性</span><span class="sxs-lookup"><span data-stu-id="25712-126">Properties</span></span>
|<span data-ttu-id="25712-127">属性</span><span class="sxs-lookup"><span data-stu-id="25712-127">Property</span></span>|<span data-ttu-id="25712-128">类型</span><span class="sxs-lookup"><span data-stu-id="25712-128">Type</span></span>|<span data-ttu-id="25712-129">说明</span><span class="sxs-lookup"><span data-stu-id="25712-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25712-130">id</span><span class="sxs-lookup"><span data-stu-id="25712-130">id</span></span>|<span data-ttu-id="25712-131">String</span><span class="sxs-lookup"><span data-stu-id="25712-131">String</span></span>|<span data-ttu-id="25712-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="25712-132">The key of the assignment.</span></span>|
|<span data-ttu-id="25712-133">target</span><span class="sxs-lookup"><span data-stu-id="25712-133">target</span></span>|[<span data-ttu-id="25712-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="25712-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="25712-135">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="25712-135">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25712-136">关系</span><span class="sxs-lookup"><span data-stu-id="25712-136">Relationships</span></span>
<span data-ttu-id="25712-137">无</span><span class="sxs-lookup"><span data-stu-id="25712-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25712-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25712-138">JSON Representation</span></span>
<span data-ttu-id="25712-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25712-139">Here is a JSON representation of the resource.</span></span>
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
  }
}
```





