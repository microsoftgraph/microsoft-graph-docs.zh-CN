---
title: 更新 appleEnrollmentProfileAssignment
description: 更新 appleEnrollmentProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f04da100fd863e87fea64f5dc7f0cfac0bdf8cb5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733390"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="95cce-103">更新 appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="95cce-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="95cce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95cce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95cce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95cce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95cce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95cce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95cce-107">更新 [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95cce-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95cce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="95cce-108">Prerequisites</span></span>
<span data-ttu-id="95cce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95cce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="95cce-111">Permission type</span></span>|<span data-ttu-id="95cce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95cce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95cce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95cce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95cce-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95cce-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95cce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95cce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95cce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="95cce-116">Not supported.</span></span>|
|<span data-ttu-id="95cce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="95cce-117">Application</span></span>|<span data-ttu-id="95cce-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95cce-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95cce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95cce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="95cce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="95cce-120">Request headers</span></span>
|<span data-ttu-id="95cce-121">标头</span><span class="sxs-lookup"><span data-stu-id="95cce-121">Header</span></span>|<span data-ttu-id="95cce-122">值</span><span class="sxs-lookup"><span data-stu-id="95cce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95cce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95cce-123">Authorization</span></span>|<span data-ttu-id="95cce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95cce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95cce-125">接受</span><span class="sxs-lookup"><span data-stu-id="95cce-125">Accept</span></span>|<span data-ttu-id="95cce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95cce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95cce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95cce-127">Request body</span></span>
<span data-ttu-id="95cce-128">在请求正文中，提供 [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95cce-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="95cce-129">下表显示创建 [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95cce-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="95cce-130">属性</span><span class="sxs-lookup"><span data-stu-id="95cce-130">Property</span></span>|<span data-ttu-id="95cce-131">类型</span><span class="sxs-lookup"><span data-stu-id="95cce-131">Type</span></span>|<span data-ttu-id="95cce-132">说明</span><span class="sxs-lookup"><span data-stu-id="95cce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95cce-133">id</span><span class="sxs-lookup"><span data-stu-id="95cce-133">id</span></span>|<span data-ttu-id="95cce-134">String</span><span class="sxs-lookup"><span data-stu-id="95cce-134">String</span></span>|<span data-ttu-id="95cce-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="95cce-135">The key of the assignment.</span></span>|
|<span data-ttu-id="95cce-136">target</span><span class="sxs-lookup"><span data-stu-id="95cce-136">target</span></span>|[<span data-ttu-id="95cce-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95cce-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95cce-138">Apple 用户启动的部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="95cce-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="95cce-139">响应</span><span class="sxs-lookup"><span data-stu-id="95cce-139">Response</span></span>
<span data-ttu-id="95cce-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95cce-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95cce-141">示例</span><span class="sxs-lookup"><span data-stu-id="95cce-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="95cce-142">请求</span><span class="sxs-lookup"><span data-stu-id="95cce-142">Request</span></span>
<span data-ttu-id="95cce-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95cce-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="95cce-144">响应</span><span class="sxs-lookup"><span data-stu-id="95cce-144">Response</span></span>
<span data-ttu-id="95cce-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95cce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





