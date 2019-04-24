---
title: 创建 deviceManagementScriptAssignment
description: 创建新的 deviceManagementScriptAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be608d325a47bc68dcc03188e068020d205d7c1b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465872"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="ec957-103">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ec957-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="ec957-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec957-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec957-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec957-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec957-106">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec957-106">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec957-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec957-107">Prerequisites</span></span>
<span data-ttu-id="ec957-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec957-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec957-110">Permission type</span></span>|<span data-ttu-id="ec957-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec957-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec957-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec957-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec957-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec957-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ec957-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec957-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec957-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec957-115">Not supported.</span></span>|
|<span data-ttu-id="ec957-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec957-116">Application</span></span>|<span data-ttu-id="ec957-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec957-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec957-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec957-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ec957-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec957-119">Request headers</span></span>
|<span data-ttu-id="ec957-120">标头</span><span class="sxs-lookup"><span data-stu-id="ec957-120">Header</span></span>|<span data-ttu-id="ec957-121">值</span><span class="sxs-lookup"><span data-stu-id="ec957-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec957-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec957-122">Authorization</span></span>|<span data-ttu-id="ec957-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec957-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec957-124">接受</span><span class="sxs-lookup"><span data-stu-id="ec957-124">Accept</span></span>|<span data-ttu-id="ec957-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec957-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec957-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec957-126">Request body</span></span>
<span data-ttu-id="ec957-127">在请求正文中, 提供 deviceManagementScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec957-127">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="ec957-128">下表显示创建 deviceManagementScriptAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec957-128">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="ec957-129">属性</span><span class="sxs-lookup"><span data-stu-id="ec957-129">Property</span></span>|<span data-ttu-id="ec957-130">类型</span><span class="sxs-lookup"><span data-stu-id="ec957-130">Type</span></span>|<span data-ttu-id="ec957-131">说明</span><span class="sxs-lookup"><span data-stu-id="ec957-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec957-132">id</span><span class="sxs-lookup"><span data-stu-id="ec957-132">id</span></span>|<span data-ttu-id="ec957-133">String</span><span class="sxs-lookup"><span data-stu-id="ec957-133">String</span></span>|<span data-ttu-id="ec957-134">device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec957-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="ec957-135">target</span><span class="sxs-lookup"><span data-stu-id="ec957-135">target</span></span>|[<span data-ttu-id="ec957-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ec957-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ec957-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="ec957-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="ec957-138">响应</span><span class="sxs-lookup"><span data-stu-id="ec957-138">Response</span></span>
<span data-ttu-id="ec957-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec957-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec957-140">示例</span><span class="sxs-lookup"><span data-stu-id="ec957-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec957-141">请求</span><span class="sxs-lookup"><span data-stu-id="ec957-141">Request</span></span>
<span data-ttu-id="ec957-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec957-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ec957-143">响应</span><span class="sxs-lookup"><span data-stu-id="ec957-143">Response</span></span>
<span data-ttu-id="ec957-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec957-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





