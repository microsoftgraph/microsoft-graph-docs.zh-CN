---
title: 更新 deviceManagementScriptGroupAssignment
description: 更新 deviceManagementScriptGroupAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b56741024048b3f9442288970275563f1bd9142b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348877"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="46b15-103">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="46b15-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="46b15-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46b15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46b15-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46b15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46b15-106">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="46b15-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46b15-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="46b15-107">Prerequisites</span></span>
<span data-ttu-id="46b15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b15-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46b15-110">Permission type</span></span>|<span data-ttu-id="46b15-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46b15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b15-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46b15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46b15-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46b15-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="46b15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46b15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46b15-115">Not supported.</span></span>|
|<span data-ttu-id="46b15-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46b15-116">Application</span></span>|<span data-ttu-id="46b15-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46b15-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46b15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="46b15-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46b15-119">Request headers</span></span>
|<span data-ttu-id="46b15-120">标头</span><span class="sxs-lookup"><span data-stu-id="46b15-120">Header</span></span>|<span data-ttu-id="46b15-121">值</span><span class="sxs-lookup"><span data-stu-id="46b15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46b15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b15-122">Authorization</span></span>|<span data-ttu-id="46b15-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46b15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46b15-124">接受</span><span class="sxs-lookup"><span data-stu-id="46b15-124">Accept</span></span>|<span data-ttu-id="46b15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46b15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="46b15-126">Request body</span></span>
<span data-ttu-id="46b15-127">在请求正文中, 提供[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46b15-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="46b15-128">下表显示创建[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="46b15-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="46b15-129">属性</span><span class="sxs-lookup"><span data-stu-id="46b15-129">Property</span></span>|<span data-ttu-id="46b15-130">类型</span><span class="sxs-lookup"><span data-stu-id="46b15-130">Type</span></span>|<span data-ttu-id="46b15-131">说明</span><span class="sxs-lookup"><span data-stu-id="46b15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b15-132">id</span><span class="sxs-lookup"><span data-stu-id="46b15-132">id</span></span>|<span data-ttu-id="46b15-133">String</span><span class="sxs-lookup"><span data-stu-id="46b15-133">String</span></span>|<span data-ttu-id="46b15-134">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="46b15-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="46b15-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="46b15-135">targetGroupId</span></span>|<span data-ttu-id="46b15-136">String</span><span class="sxs-lookup"><span data-stu-id="46b15-136">String</span></span>|<span data-ttu-id="46b15-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="46b15-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="46b15-138">响应</span><span class="sxs-lookup"><span data-stu-id="46b15-138">Response</span></span>
<span data-ttu-id="46b15-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="46b15-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b15-140">示例</span><span class="sxs-lookup"><span data-stu-id="46b15-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="46b15-141">请求</span><span class="sxs-lookup"><span data-stu-id="46b15-141">Request</span></span>
<span data-ttu-id="46b15-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46b15-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="46b15-143">响应</span><span class="sxs-lookup"><span data-stu-id="46b15-143">Response</span></span>
<span data-ttu-id="46b15-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46b15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






