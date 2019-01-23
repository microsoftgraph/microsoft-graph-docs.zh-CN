---
title: 更新 deviceManagementScriptGroupAssignment
description: 更新 deviceManagementScriptGroupAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bab2f5e2c363d56379e240eb6c26b95e7a0fc8b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409977"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="4a0d3-103">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4a0d3-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="4a0d3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a0d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a0d3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a0d3-107">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a0d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a0d3-108">Prerequisites</span></span>
<span data-ttu-id="4a0d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a0d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a0d3-111">Permission type</span></span>|<span data-ttu-id="4a0d3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a0d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a0d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a0d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a0d3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a0d3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a0d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a0d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a0d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-116">Not supported.</span></span>|
|<span data-ttu-id="4a0d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a0d3-117">Application</span></span>|<span data-ttu-id="4a0d3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a0d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a0d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4a0d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a0d3-120">Request headers</span></span>
|<span data-ttu-id="4a0d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="4a0d3-121">Header</span></span>|<span data-ttu-id="4a0d3-122">值</span><span class="sxs-lookup"><span data-stu-id="4a0d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a0d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a0d3-123">Authorization</span></span>|<span data-ttu-id="4a0d3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a0d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a0d3-125">Accept</span></span>|<span data-ttu-id="4a0d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a0d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a0d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a0d3-127">Request body</span></span>
<span data-ttu-id="4a0d3-128">在请求正文中，提供[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="4a0d3-129">下表显示时创建[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="4a0d3-130">属性</span><span class="sxs-lookup"><span data-stu-id="4a0d3-130">Property</span></span>|<span data-ttu-id="4a0d3-131">类型</span><span class="sxs-lookup"><span data-stu-id="4a0d3-131">Type</span></span>|<span data-ttu-id="4a0d3-132">说明</span><span class="sxs-lookup"><span data-stu-id="4a0d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a0d3-133">id</span><span class="sxs-lookup"><span data-stu-id="4a0d3-133">id</span></span>|<span data-ttu-id="4a0d3-134">String</span><span class="sxs-lookup"><span data-stu-id="4a0d3-134">String</span></span>|<span data-ttu-id="4a0d3-135">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="4a0d3-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4a0d3-136">targetGroupId</span></span>|<span data-ttu-id="4a0d3-137">String</span><span class="sxs-lookup"><span data-stu-id="4a0d3-137">String</span></span>|<span data-ttu-id="4a0d3-138">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="4a0d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="4a0d3-139">Response</span></span>
<span data-ttu-id="4a0d3-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a0d3-141">示例</span><span class="sxs-lookup"><span data-stu-id="4a0d3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a0d3-142">请求</span><span class="sxs-lookup"><span data-stu-id="4a0d3-142">Request</span></span>
<span data-ttu-id="4a0d3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="4a0d3-144">响应</span><span class="sxs-lookup"><span data-stu-id="4a0d3-144">Response</span></span>
<span data-ttu-id="4a0d3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a0d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




