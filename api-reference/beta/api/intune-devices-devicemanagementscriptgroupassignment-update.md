---
title: 更新 deviceManagementScriptGroupAssignment
description: 更新 deviceManagementScriptGroupAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ec8b9e31d7e80bbc7f2733832aa5f75213a04fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150400"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="b9de8-103">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b9de8-103">Update deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="b9de8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9de8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9de8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9de8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9de8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9de8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9de8-107">更新 [deviceManagementScriptGroupAssignment 对象](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b9de8-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9de8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9de8-108">Prerequisites</span></span>
<span data-ttu-id="b9de8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9de8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9de8-111">Permission type</span></span>|<span data-ttu-id="b9de8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9de8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9de8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9de8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9de8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9de8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b9de8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9de8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9de8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9de8-116">Not supported.</span></span>|
|<span data-ttu-id="b9de8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9de8-117">Application</span></span>|<span data-ttu-id="b9de8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9de8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9de8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9de8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9de8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9de8-120">Request headers</span></span>
|<span data-ttu-id="b9de8-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9de8-121">Header</span></span>|<span data-ttu-id="b9de8-122">值</span><span class="sxs-lookup"><span data-stu-id="b9de8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9de8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9de8-123">Authorization</span></span>|<span data-ttu-id="b9de8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9de8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9de8-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9de8-125">Accept</span></span>|<span data-ttu-id="b9de8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9de8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9de8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9de8-127">Request body</span></span>
<span data-ttu-id="b9de8-128">在请求正文中，提供 [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9de8-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="b9de8-129">下表显示创建 [deviceManagementScriptGroupAssignment 时所需的属性](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b9de8-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="b9de8-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9de8-130">Property</span></span>|<span data-ttu-id="b9de8-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9de8-131">Type</span></span>|<span data-ttu-id="b9de8-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9de8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9de8-133">id</span><span class="sxs-lookup"><span data-stu-id="b9de8-133">id</span></span>|<span data-ttu-id="b9de8-134">String</span><span class="sxs-lookup"><span data-stu-id="b9de8-134">String</span></span>|<span data-ttu-id="b9de8-135">设备管理脚本组分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9de8-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="b9de8-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b9de8-136">This property is read-only.</span></span>|
|<span data-ttu-id="b9de8-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b9de8-137">targetGroupId</span></span>|<span data-ttu-id="b9de8-138">String</span><span class="sxs-lookup"><span data-stu-id="b9de8-138">String</span></span>|<span data-ttu-id="b9de8-139">我们将脚本定向到的 Azure Active Directory 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="b9de8-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="b9de8-140">响应</span><span class="sxs-lookup"><span data-stu-id="b9de8-140">Response</span></span>
<span data-ttu-id="b9de8-141">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9de8-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9de8-142">示例</span><span class="sxs-lookup"><span data-stu-id="b9de8-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9de8-143">请求</span><span class="sxs-lookup"><span data-stu-id="b9de8-143">Request</span></span>
<span data-ttu-id="b9de8-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9de8-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="b9de8-145">响应</span><span class="sxs-lookup"><span data-stu-id="b9de8-145">Response</span></span>
<span data-ttu-id="b9de8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9de8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




