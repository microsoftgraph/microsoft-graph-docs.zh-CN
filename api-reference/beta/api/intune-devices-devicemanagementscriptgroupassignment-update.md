---
title: 更新 deviceManagementScriptGroupAssignment
description: 更新 deviceManagementScriptGroupAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48b5ebfe08487495e44b7f1edb28ba30b0002ad1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944930"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="58a96-103">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="58a96-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="58a96-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58a96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a96-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a96-106">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58a96-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a96-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="58a96-107">Prerequisites</span></span>
<span data-ttu-id="58a96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="58a96-110">Permission type</span></span>|<span data-ttu-id="58a96-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58a96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58a96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58a96-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a96-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58a96-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58a96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a96-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="58a96-115">Not supported.</span></span>|
|<span data-ttu-id="58a96-116">Application</span><span class="sxs-lookup"><span data-stu-id="58a96-116">Application</span></span>|<span data-ttu-id="58a96-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a96-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a96-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58a96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="58a96-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="58a96-119">Request headers</span></span>
|<span data-ttu-id="58a96-120">标头</span><span class="sxs-lookup"><span data-stu-id="58a96-120">Header</span></span>|<span data-ttu-id="58a96-121">值</span><span class="sxs-lookup"><span data-stu-id="58a96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a96-122">授权</span><span class="sxs-lookup"><span data-stu-id="58a96-122">Authorization</span></span>|<span data-ttu-id="58a96-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58a96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a96-124">接受</span><span class="sxs-lookup"><span data-stu-id="58a96-124">Accept</span></span>|<span data-ttu-id="58a96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58a96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a96-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="58a96-126">Request body</span></span>
<span data-ttu-id="58a96-127">在请求正文中，提供[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58a96-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="58a96-128">下表显示创建[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58a96-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="58a96-129">属性</span><span class="sxs-lookup"><span data-stu-id="58a96-129">Property</span></span>|<span data-ttu-id="58a96-130">类型</span><span class="sxs-lookup"><span data-stu-id="58a96-130">Type</span></span>|<span data-ttu-id="58a96-131">说明</span><span class="sxs-lookup"><span data-stu-id="58a96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a96-132">id</span><span class="sxs-lookup"><span data-stu-id="58a96-132">id</span></span>|<span data-ttu-id="58a96-133">字符串</span><span class="sxs-lookup"><span data-stu-id="58a96-133">String</span></span>|<span data-ttu-id="58a96-134">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="58a96-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="58a96-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="58a96-135">This property is read-only.</span></span>|
|<span data-ttu-id="58a96-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="58a96-136">targetGroupId</span></span>|<span data-ttu-id="58a96-137">字符串</span><span class="sxs-lookup"><span data-stu-id="58a96-137">String</span></span>|<span data-ttu-id="58a96-138">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="58a96-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="58a96-139">响应</span><span class="sxs-lookup"><span data-stu-id="58a96-139">Response</span></span>
<span data-ttu-id="58a96-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="58a96-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a96-141">示例</span><span class="sxs-lookup"><span data-stu-id="58a96-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a96-142">请求</span><span class="sxs-lookup"><span data-stu-id="58a96-142">Request</span></span>
<span data-ttu-id="58a96-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58a96-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="58a96-144">响应</span><span class="sxs-lookup"><span data-stu-id="58a96-144">Response</span></span>
<span data-ttu-id="58a96-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58a96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





