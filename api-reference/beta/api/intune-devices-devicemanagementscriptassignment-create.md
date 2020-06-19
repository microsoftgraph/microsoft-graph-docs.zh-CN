---
title: 创建 deviceManagementScriptAssignment
description: 创建新的 deviceManagementScriptAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b43ec4ffeb081eb4865d0fbb7e7f7110bfeefa3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792364"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="bbb40-103">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="bbb40-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="bbb40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbb40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbb40-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bbb40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbb40-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bbb40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb40-107">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bbb40-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbb40-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbb40-108">Prerequisites</span></span>
<span data-ttu-id="bbb40-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bbb40-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bbb40-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb40-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb40-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbb40-111">Permission type</span></span>|<span data-ttu-id="bbb40-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bbb40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbb40-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbb40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbb40-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb40-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bbb40-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbb40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbb40-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbb40-116">Not supported.</span></span>|
|<span data-ttu-id="bbb40-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbb40-117">Application</span></span>|<span data-ttu-id="bbb40-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb40-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbb40-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbb40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bbb40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbb40-120">Request headers</span></span>
|<span data-ttu-id="bbb40-121">标头</span><span class="sxs-lookup"><span data-stu-id="bbb40-121">Header</span></span>|<span data-ttu-id="bbb40-122">值</span><span class="sxs-lookup"><span data-stu-id="bbb40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbb40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbb40-123">Authorization</span></span>|<span data-ttu-id="bbb40-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbb40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbb40-125">接受</span><span class="sxs-lookup"><span data-stu-id="bbb40-125">Accept</span></span>|<span data-ttu-id="bbb40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbb40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbb40-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbb40-127">Request body</span></span>
<span data-ttu-id="bbb40-128">在请求正文中，提供 deviceManagementScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbb40-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="bbb40-129">下表显示创建 deviceManagementScriptAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bbb40-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="bbb40-130">属性</span><span class="sxs-lookup"><span data-stu-id="bbb40-130">Property</span></span>|<span data-ttu-id="bbb40-131">类型</span><span class="sxs-lookup"><span data-stu-id="bbb40-131">Type</span></span>|<span data-ttu-id="bbb40-132">说明</span><span class="sxs-lookup"><span data-stu-id="bbb40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb40-133">id</span><span class="sxs-lookup"><span data-stu-id="bbb40-133">id</span></span>|<span data-ttu-id="bbb40-134">String</span><span class="sxs-lookup"><span data-stu-id="bbb40-134">String</span></span>|<span data-ttu-id="bbb40-135">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="bbb40-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="bbb40-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bbb40-136">This property is read-only.</span></span>|
|<span data-ttu-id="bbb40-137">target</span><span class="sxs-lookup"><span data-stu-id="bbb40-137">target</span></span>|[<span data-ttu-id="bbb40-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bbb40-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bbb40-139">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="bbb40-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="bbb40-140">响应</span><span class="sxs-lookup"><span data-stu-id="bbb40-140">Response</span></span>
<span data-ttu-id="bbb40-141">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bbb40-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb40-142">示例</span><span class="sxs-lookup"><span data-stu-id="bbb40-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbb40-143">请求</span><span class="sxs-lookup"><span data-stu-id="bbb40-143">Request</span></span>
<span data-ttu-id="bbb40-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbb40-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="bbb40-145">响应</span><span class="sxs-lookup"><span data-stu-id="bbb40-145">Response</span></span>
<span data-ttu-id="bbb40-146">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="bbb40-146">Here is an example of the response.</span></span> <span data-ttu-id="bbb40-147">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="bbb40-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bbb40-148">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bbb40-148">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



