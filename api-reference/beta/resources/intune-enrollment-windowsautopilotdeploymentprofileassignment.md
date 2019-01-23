---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec24363dbf245ce261cdbd534ef00f501af1d8ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406008"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="de184-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="de184-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="de184-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="de184-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="de184-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de184-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de184-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de184-107">Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。</span><span class="sxs-lookup"><span data-stu-id="de184-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="de184-108">方法</span><span class="sxs-lookup"><span data-stu-id="de184-108">Methods</span></span>
|<span data-ttu-id="de184-109">方法</span><span class="sxs-lookup"><span data-stu-id="de184-109">Method</span></span>|<span data-ttu-id="de184-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="de184-110">Return Type</span></span>|<span data-ttu-id="de184-111">说明</span><span class="sxs-lookup"><span data-stu-id="de184-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de184-112">列表 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="de184-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="de184-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="de184-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="de184-114">列出属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="de184-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="de184-115">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="de184-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="de184-117">读取属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="de184-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="de184-118">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="de184-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="de184-120">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de184-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="de184-121">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="de184-122">无</span><span class="sxs-lookup"><span data-stu-id="de184-122">None</span></span>|<span data-ttu-id="de184-123">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="de184-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="de184-124">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="de184-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de184-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="de184-126">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de184-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de184-127">属性</span><span class="sxs-lookup"><span data-stu-id="de184-127">Properties</span></span>
|<span data-ttu-id="de184-128">属性</span><span class="sxs-lookup"><span data-stu-id="de184-128">Property</span></span>|<span data-ttu-id="de184-129">类型</span><span class="sxs-lookup"><span data-stu-id="de184-129">Type</span></span>|<span data-ttu-id="de184-130">说明</span><span class="sxs-lookup"><span data-stu-id="de184-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de184-131">id</span><span class="sxs-lookup"><span data-stu-id="de184-131">id</span></span>|<span data-ttu-id="de184-132">String</span><span class="sxs-lookup"><span data-stu-id="de184-132">String</span></span>|<span data-ttu-id="de184-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="de184-133">The key of the assignment.</span></span>|
|<span data-ttu-id="de184-134">target</span><span class="sxs-lookup"><span data-stu-id="de184-134">target</span></span>|[<span data-ttu-id="de184-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de184-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de184-136">工作分配针对的 Windows 自动执行某些操作部署配置文件。</span><span class="sxs-lookup"><span data-stu-id="de184-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de184-137">关系</span><span class="sxs-lookup"><span data-stu-id="de184-137">Relationships</span></span>
<span data-ttu-id="de184-138">无</span><span class="sxs-lookup"><span data-stu-id="de184-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de184-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de184-139">JSON Representation</span></span>
<span data-ttu-id="de184-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de184-140">Here is a JSON representation of the resource.</span></span>
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




