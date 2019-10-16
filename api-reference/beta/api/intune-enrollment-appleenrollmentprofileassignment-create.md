---
title: 创建 appleEnrollmentProfileAssignment
description: 创建新的 appleEnrollmentProfileAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 042d81fc22a65b3df16d6bdf75fac33c1e1b88b7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526202"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="4dc7d-103">创建 appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4dc7d-103">Create appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="4dc7d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dc7d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc7d-106">创建新的[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-106">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dc7d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4dc7d-107">Prerequisites</span></span>
<span data-ttu-id="4dc7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc7d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dc7d-110">Permission type</span></span>|<span data-ttu-id="4dc7d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4dc7d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dc7d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dc7d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc7d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dc7d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dc7d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-115">Not supported.</span></span>|
|<span data-ttu-id="4dc7d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dc7d-116">Application</span></span>|<span data-ttu-id="4dc7d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc7d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dc7d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dc7d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4dc7d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dc7d-119">Request headers</span></span>
|<span data-ttu-id="4dc7d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4dc7d-120">Header</span></span>|<span data-ttu-id="4dc7d-121">值</span><span class="sxs-lookup"><span data-stu-id="4dc7d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dc7d-122">授权</span><span class="sxs-lookup"><span data-stu-id="4dc7d-122">Authorization</span></span>|<span data-ttu-id="4dc7d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dc7d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4dc7d-124">Accept</span></span>|<span data-ttu-id="4dc7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc7d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dc7d-126">Request body</span></span>
<span data-ttu-id="4dc7d-127">在请求正文中，提供 appleEnrollmentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-127">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="4dc7d-128">下表显示创建 appleEnrollmentProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-128">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="4dc7d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4dc7d-129">Property</span></span>|<span data-ttu-id="4dc7d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4dc7d-130">Type</span></span>|<span data-ttu-id="4dc7d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4dc7d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc7d-132">id</span><span class="sxs-lookup"><span data-stu-id="4dc7d-132">id</span></span>|<span data-ttu-id="4dc7d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4dc7d-133">String</span></span>|<span data-ttu-id="4dc7d-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-134">The key of the assignment.</span></span>|
|<span data-ttu-id="4dc7d-135">target</span><span class="sxs-lookup"><span data-stu-id="4dc7d-135">target</span></span>|[<span data-ttu-id="4dc7d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4dc7d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4dc7d-137">Apple 用户启动的部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-137">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4dc7d-138">响应</span><span class="sxs-lookup"><span data-stu-id="4dc7d-138">Response</span></span>
<span data-ttu-id="4dc7d-139">如果成功，此方法在响应`201 Created`正文中返回响应代码和[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-139">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc7d-140">示例</span><span class="sxs-lookup"><span data-stu-id="4dc7d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dc7d-141">请求</span><span class="sxs-lookup"><span data-stu-id="4dc7d-141">Request</span></span>
<span data-ttu-id="4dc7d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4dc7d-143">响应</span><span class="sxs-lookup"><span data-stu-id="4dc7d-143">Response</span></span>
<span data-ttu-id="4dc7d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dc7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






