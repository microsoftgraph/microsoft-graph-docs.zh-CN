---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a6aa5152dd3dd85dc2aadbd4880f638b4e75b1a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967173"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="84436-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="84436-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="84436-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84436-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84436-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84436-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84436-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84436-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84436-107">Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。</span><span class="sxs-lookup"><span data-stu-id="84436-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>
## <a name="methods"></a><span data-ttu-id="84436-108">方法</span><span class="sxs-lookup"><span data-stu-id="84436-108">Methods</span></span>
|<span data-ttu-id="84436-109">方法</span><span class="sxs-lookup"><span data-stu-id="84436-109">Method</span></span>|<span data-ttu-id="84436-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="84436-110">Return Type</span></span>|<span data-ttu-id="84436-111">说明</span><span class="sxs-lookup"><span data-stu-id="84436-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84436-112">列表 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="84436-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="84436-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="84436-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="84436-114">列出属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="84436-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="84436-115">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="84436-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="84436-117">读取属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="84436-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="84436-118">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="84436-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="84436-120">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84436-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="84436-121">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="84436-122">无</span><span class="sxs-lookup"><span data-stu-id="84436-122">None</span></span>|<span data-ttu-id="84436-123">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="84436-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="84436-124">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="84436-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="84436-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="84436-126">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84436-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84436-127">属性</span><span class="sxs-lookup"><span data-stu-id="84436-127">Properties</span></span>
|<span data-ttu-id="84436-128">属性</span><span class="sxs-lookup"><span data-stu-id="84436-128">Property</span></span>|<span data-ttu-id="84436-129">类型</span><span class="sxs-lookup"><span data-stu-id="84436-129">Type</span></span>|<span data-ttu-id="84436-130">说明</span><span class="sxs-lookup"><span data-stu-id="84436-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84436-131">id</span><span class="sxs-lookup"><span data-stu-id="84436-131">id</span></span>|<span data-ttu-id="84436-132">String</span><span class="sxs-lookup"><span data-stu-id="84436-132">String</span></span>|<span data-ttu-id="84436-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="84436-133">The key of the assignment.</span></span>|
|<span data-ttu-id="84436-134">target</span><span class="sxs-lookup"><span data-stu-id="84436-134">target</span></span>|[<span data-ttu-id="84436-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="84436-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="84436-136">工作分配针对的 Windows 自动执行某些操作部署配置文件。</span><span class="sxs-lookup"><span data-stu-id="84436-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84436-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="84436-137">Relationships</span></span>
<span data-ttu-id="84436-138">无</span><span class="sxs-lookup"><span data-stu-id="84436-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84436-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84436-139">JSON Representation</span></span>
<span data-ttu-id="84436-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84436-140">Here is a JSON representation of the resource.</span></span>
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





