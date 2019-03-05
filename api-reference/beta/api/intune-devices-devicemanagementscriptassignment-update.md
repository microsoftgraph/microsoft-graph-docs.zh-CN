---
title: 更新 deviceManagementScriptAssignment
description: 更新 deviceManagementScriptAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35085405f8b28066f3774e9f27fe1471e2cc1654
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153422"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="2779c-103">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="2779c-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="2779c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2779c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2779c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2779c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2779c-106">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2779c-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2779c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2779c-107">Prerequisites</span></span>
<span data-ttu-id="2779c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2779c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2779c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2779c-110">Permission type</span></span>|<span data-ttu-id="2779c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2779c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2779c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2779c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2779c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2779c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2779c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2779c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2779c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2779c-115">Not supported.</span></span>|
|<span data-ttu-id="2779c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2779c-116">Application</span></span>|<span data-ttu-id="2779c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2779c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2779c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2779c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2779c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2779c-119">Request headers</span></span>
|<span data-ttu-id="2779c-120">标头</span><span class="sxs-lookup"><span data-stu-id="2779c-120">Header</span></span>|<span data-ttu-id="2779c-121">值</span><span class="sxs-lookup"><span data-stu-id="2779c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2779c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2779c-122">Authorization</span></span>|<span data-ttu-id="2779c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2779c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2779c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2779c-124">Accept</span></span>|<span data-ttu-id="2779c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2779c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2779c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2779c-126">Request body</span></span>
<span data-ttu-id="2779c-127">在请求正文中, 提供[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2779c-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="2779c-128">下表显示创建[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2779c-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="2779c-129">属性</span><span class="sxs-lookup"><span data-stu-id="2779c-129">Property</span></span>|<span data-ttu-id="2779c-130">类型</span><span class="sxs-lookup"><span data-stu-id="2779c-130">Type</span></span>|<span data-ttu-id="2779c-131">说明</span><span class="sxs-lookup"><span data-stu-id="2779c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2779c-132">id</span><span class="sxs-lookup"><span data-stu-id="2779c-132">id</span></span>|<span data-ttu-id="2779c-133">String</span><span class="sxs-lookup"><span data-stu-id="2779c-133">String</span></span>|<span data-ttu-id="2779c-134">device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="2779c-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="2779c-135">target</span><span class="sxs-lookup"><span data-stu-id="2779c-135">target</span></span>|[<span data-ttu-id="2779c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2779c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2779c-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="2779c-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="2779c-138">响应</span><span class="sxs-lookup"><span data-stu-id="2779c-138">Response</span></span>
<span data-ttu-id="2779c-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2779c-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2779c-140">示例</span><span class="sxs-lookup"><span data-stu-id="2779c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2779c-141">请求</span><span class="sxs-lookup"><span data-stu-id="2779c-141">Request</span></span>
<span data-ttu-id="2779c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2779c-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2779c-143">响应</span><span class="sxs-lookup"><span data-stu-id="2779c-143">Response</span></span>
<span data-ttu-id="2779c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2779c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




