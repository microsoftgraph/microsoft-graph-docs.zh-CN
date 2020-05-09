---
title: 更新 deviceManagementScriptAssignment
description: 更新 deviceManagementScriptAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5521c3753deafb40279e2ec0e16bd2fa0b30316b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176545"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="625cc-103">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="625cc-103">Update deviceManagementScriptAssignment</span></span>

<span data-ttu-id="625cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="625cc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="625cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="625cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="625cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="625cc-107">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="625cc-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="625cc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="625cc-108">Prerequisites</span></span>
<span data-ttu-id="625cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="625cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="625cc-111">Permission type</span></span>|<span data-ttu-id="625cc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="625cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="625cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="625cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="625cc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625cc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="625cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="625cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="625cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="625cc-116">Not supported.</span></span>|
|<span data-ttu-id="625cc-117">Application</span><span class="sxs-lookup"><span data-stu-id="625cc-117">Application</span></span>|<span data-ttu-id="625cc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625cc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="625cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="625cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="625cc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="625cc-120">Request headers</span></span>
|<span data-ttu-id="625cc-121">标头</span><span class="sxs-lookup"><span data-stu-id="625cc-121">Header</span></span>|<span data-ttu-id="625cc-122">值</span><span class="sxs-lookup"><span data-stu-id="625cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="625cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="625cc-123">Authorization</span></span>|<span data-ttu-id="625cc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="625cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="625cc-125">接受</span><span class="sxs-lookup"><span data-stu-id="625cc-125">Accept</span></span>|<span data-ttu-id="625cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="625cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="625cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="625cc-127">Request body</span></span>
<span data-ttu-id="625cc-128">在请求正文中，提供[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="625cc-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="625cc-129">下表显示创建[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="625cc-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="625cc-130">属性</span><span class="sxs-lookup"><span data-stu-id="625cc-130">Property</span></span>|<span data-ttu-id="625cc-131">类型</span><span class="sxs-lookup"><span data-stu-id="625cc-131">Type</span></span>|<span data-ttu-id="625cc-132">说明</span><span class="sxs-lookup"><span data-stu-id="625cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="625cc-133">id</span><span class="sxs-lookup"><span data-stu-id="625cc-133">id</span></span>|<span data-ttu-id="625cc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="625cc-134">String</span></span>|<span data-ttu-id="625cc-135">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="625cc-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="625cc-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="625cc-136">This property is read-only.</span></span>|
|<span data-ttu-id="625cc-137">target</span><span class="sxs-lookup"><span data-stu-id="625cc-137">target</span></span>|[<span data-ttu-id="625cc-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="625cc-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="625cc-139">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="625cc-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="625cc-140">响应</span><span class="sxs-lookup"><span data-stu-id="625cc-140">Response</span></span>
<span data-ttu-id="625cc-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="625cc-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625cc-142">示例</span><span class="sxs-lookup"><span data-stu-id="625cc-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="625cc-143">请求</span><span class="sxs-lookup"><span data-stu-id="625cc-143">Request</span></span>
<span data-ttu-id="625cc-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="625cc-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 160

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="625cc-145">响应</span><span class="sxs-lookup"><span data-stu-id="625cc-145">Response</span></span>
<span data-ttu-id="625cc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="625cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



