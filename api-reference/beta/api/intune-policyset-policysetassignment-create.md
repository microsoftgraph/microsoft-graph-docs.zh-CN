---
title: 创建 policySetAssignment
description: 创建新的 policySetAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0c8a931a50b10f7694312bd618bdc20000299ca
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791712"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="3d4b7-103">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="3d4b7-103">Create policySetAssignment</span></span>

<span data-ttu-id="3d4b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d4b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d4b7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d4b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d4b7-107">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d4b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d4b7-108">Prerequisites</span></span>
<span data-ttu-id="3d4b7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3d4b7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3d4b7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d4b7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d4b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d4b7-111">Permission type</span></span>|<span data-ttu-id="3d4b7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d4b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d4b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d4b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d4b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d4b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d4b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d4b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-116">Not supported.</span></span>|
|<span data-ttu-id="3d4b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d4b7-117">Application</span></span>|<span data-ttu-id="3d4b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d4b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d4b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3d4b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d4b7-120">Request headers</span></span>
|<span data-ttu-id="3d4b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d4b7-121">Header</span></span>|<span data-ttu-id="3d4b7-122">值</span><span class="sxs-lookup"><span data-stu-id="3d4b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d4b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d4b7-123">Authorization</span></span>|<span data-ttu-id="3d4b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d4b7-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d4b7-125">Accept</span></span>|<span data-ttu-id="3d4b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d4b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d4b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d4b7-127">Request body</span></span>
<span data-ttu-id="3d4b7-128">在请求正文中，提供 policySetAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="3d4b7-129">下表显示创建 policySetAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="3d4b7-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d4b7-130">Property</span></span>|<span data-ttu-id="3d4b7-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d4b7-131">Type</span></span>|<span data-ttu-id="3d4b7-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d4b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d4b7-133">id</span><span class="sxs-lookup"><span data-stu-id="3d4b7-133">id</span></span>|<span data-ttu-id="3d4b7-134">String</span><span class="sxs-lookup"><span data-stu-id="3d4b7-134">String</span></span>|<span data-ttu-id="3d4b7-135">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="3d4b7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d4b7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3d4b7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d4b7-137">DateTimeOffset</span></span>|<span data-ttu-id="3d4b7-138">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="3d4b7-139">target</span><span class="sxs-lookup"><span data-stu-id="3d4b7-139">target</span></span>|[<span data-ttu-id="3d4b7-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3d4b7-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3d4b7-141">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="3d4b7-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="3d4b7-142">响应</span><span class="sxs-lookup"><span data-stu-id="3d4b7-142">Response</span></span>
<span data-ttu-id="3d4b7-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d4b7-144">示例</span><span class="sxs-lookup"><span data-stu-id="3d4b7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d4b7-145">请求</span><span class="sxs-lookup"><span data-stu-id="3d4b7-145">Request</span></span>
<span data-ttu-id="3d4b7-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d4b7-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="3d4b7-147">响应</span><span class="sxs-lookup"><span data-stu-id="3d4b7-147">Response</span></span>
<span data-ttu-id="3d4b7-148">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3d4b7-148">Here is an example of the response.</span></span> <span data-ttu-id="3d4b7-149">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3d4b7-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3d4b7-150">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3d4b7-150">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 427

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



