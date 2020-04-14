---
title: 更新 appleEnrollmentProfileAssignment
description: 更新 appleEnrollmentProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 434b2d5ee2f3d751fa5662605cf94c6e180cad48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321132"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="f9726-103">更新 appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="f9726-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="f9726-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9726-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9726-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9726-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9726-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9726-107">更新[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9726-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9726-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9726-108">Prerequisites</span></span>
<span data-ttu-id="f9726-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9726-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9726-111">Permission type</span></span>|<span data-ttu-id="f9726-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9726-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9726-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9726-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9726-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9726-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9726-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9726-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9726-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9726-116">Not supported.</span></span>|
|<span data-ttu-id="f9726-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9726-117">Application</span></span>|<span data-ttu-id="f9726-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9726-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9726-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9726-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f9726-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9726-120">Request headers</span></span>
|<span data-ttu-id="f9726-121">标头</span><span class="sxs-lookup"><span data-stu-id="f9726-121">Header</span></span>|<span data-ttu-id="f9726-122">值</span><span class="sxs-lookup"><span data-stu-id="f9726-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9726-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9726-123">Authorization</span></span>|<span data-ttu-id="f9726-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9726-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9726-125">接受</span><span class="sxs-lookup"><span data-stu-id="f9726-125">Accept</span></span>|<span data-ttu-id="f9726-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9726-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9726-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9726-127">Request body</span></span>
<span data-ttu-id="f9726-128">在请求正文中，提供[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9726-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="f9726-129">下表显示创建[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9726-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="f9726-130">属性</span><span class="sxs-lookup"><span data-stu-id="f9726-130">Property</span></span>|<span data-ttu-id="f9726-131">类型</span><span class="sxs-lookup"><span data-stu-id="f9726-131">Type</span></span>|<span data-ttu-id="f9726-132">说明</span><span class="sxs-lookup"><span data-stu-id="f9726-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9726-133">id</span><span class="sxs-lookup"><span data-stu-id="f9726-133">id</span></span>|<span data-ttu-id="f9726-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f9726-134">String</span></span>|<span data-ttu-id="f9726-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="f9726-135">The key of the assignment.</span></span>|
|<span data-ttu-id="f9726-136">target</span><span class="sxs-lookup"><span data-stu-id="f9726-136">target</span></span>|[<span data-ttu-id="f9726-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9726-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9726-138">Apple 用户启动的部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="f9726-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="f9726-139">响应</span><span class="sxs-lookup"><span data-stu-id="f9726-139">Response</span></span>
<span data-ttu-id="f9726-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f9726-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9726-141">示例</span><span class="sxs-lookup"><span data-stu-id="f9726-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9726-142">请求</span><span class="sxs-lookup"><span data-stu-id="f9726-142">Request</span></span>
<span data-ttu-id="f9726-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9726-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="f9726-144">响应</span><span class="sxs-lookup"><span data-stu-id="f9726-144">Response</span></span>
<span data-ttu-id="f9726-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9726-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



