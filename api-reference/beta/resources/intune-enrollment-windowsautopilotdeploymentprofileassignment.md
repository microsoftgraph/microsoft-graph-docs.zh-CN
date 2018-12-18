---
title: windowsAutopilotDeploymentProfileAssignment 资源类型
description: Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。
author: tfitzmac
ms.openlocfilehash: b9141d9a3126d25dd6de5e342ebb463304e1ae02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337119"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="f660b-103">windowsAutopilotDeploymentProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f660b-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="f660b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f660b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f660b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f660b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f660b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f660b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f660b-107">Windows 自动执行某些操作部署配置文件到 AAD 组工作分配。</span><span class="sxs-lookup"><span data-stu-id="f660b-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>
## <a name="methods"></a><span data-ttu-id="f660b-108">方法</span><span class="sxs-lookup"><span data-stu-id="f660b-108">Methods</span></span>
|<span data-ttu-id="f660b-109">方法</span><span class="sxs-lookup"><span data-stu-id="f660b-109">Method</span></span>|<span data-ttu-id="f660b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f660b-110">Return Type</span></span>|<span data-ttu-id="f660b-111">说明</span><span class="sxs-lookup"><span data-stu-id="f660b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f660b-112">列表 windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="f660b-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="f660b-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f660b-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="f660b-114">列出属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f660b-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="f660b-115">获取 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="f660b-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="f660b-117">读取属性和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f660b-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="f660b-118">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="f660b-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="f660b-120">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f660b-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="f660b-121">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="f660b-122">无</span><span class="sxs-lookup"><span data-stu-id="f660b-122">None</span></span>|<span data-ttu-id="f660b-123">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f660b-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="f660b-124">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="f660b-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f660b-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="f660b-126">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f660b-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f660b-127">属性</span><span class="sxs-lookup"><span data-stu-id="f660b-127">Properties</span></span>
|<span data-ttu-id="f660b-128">属性</span><span class="sxs-lookup"><span data-stu-id="f660b-128">Property</span></span>|<span data-ttu-id="f660b-129">类型</span><span class="sxs-lookup"><span data-stu-id="f660b-129">Type</span></span>|<span data-ttu-id="f660b-130">说明</span><span class="sxs-lookup"><span data-stu-id="f660b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f660b-131">id</span><span class="sxs-lookup"><span data-stu-id="f660b-131">id</span></span>|<span data-ttu-id="f660b-132">String</span><span class="sxs-lookup"><span data-stu-id="f660b-132">String</span></span>|<span data-ttu-id="f660b-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="f660b-133">The key of the assignment.</span></span>|
|<span data-ttu-id="f660b-134">target</span><span class="sxs-lookup"><span data-stu-id="f660b-134">target</span></span>|[<span data-ttu-id="f660b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f660b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f660b-136">工作分配针对的 Windows 自动执行某些操作部署配置文件。</span><span class="sxs-lookup"><span data-stu-id="f660b-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f660b-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="f660b-137">Relationships</span></span>
<span data-ttu-id="f660b-138">无</span><span class="sxs-lookup"><span data-stu-id="f660b-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f660b-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f660b-139">JSON Representation</span></span>
<span data-ttu-id="f660b-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f660b-140">Here is a JSON representation of the resource.</span></span>
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





