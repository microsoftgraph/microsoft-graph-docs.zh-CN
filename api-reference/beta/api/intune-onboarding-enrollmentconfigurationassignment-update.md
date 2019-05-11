---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca6edf132ba027dc4b0e5c30a7e827a1c9587cc6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900024"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="c1076-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c1076-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="c1076-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1076-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1076-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1076-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1076-106">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1076-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1076-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1076-107">Prerequisites</span></span>
<span data-ttu-id="c1076-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1076-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1076-110">Permission type</span></span>|<span data-ttu-id="c1076-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1076-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1076-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1076-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1076-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1076-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1076-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1076-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1076-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1076-115">Not supported.</span></span>|
|<span data-ttu-id="c1076-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1076-116">Application</span></span>|<span data-ttu-id="c1076-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1076-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1076-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1076-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1076-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1076-119">Request headers</span></span>
|<span data-ttu-id="c1076-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1076-120">Header</span></span>|<span data-ttu-id="c1076-121">值</span><span class="sxs-lookup"><span data-stu-id="c1076-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1076-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1076-122">Authorization</span></span>|<span data-ttu-id="c1076-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1076-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1076-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1076-124">Accept</span></span>|<span data-ttu-id="c1076-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1076-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1076-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1076-126">Request body</span></span>
<span data-ttu-id="c1076-127">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1076-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c1076-128">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1076-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="c1076-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1076-129">Property</span></span>|<span data-ttu-id="c1076-130">类型</span><span class="sxs-lookup"><span data-stu-id="c1076-130">Type</span></span>|<span data-ttu-id="c1076-131">说明</span><span class="sxs-lookup"><span data-stu-id="c1076-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1076-132">id</span><span class="sxs-lookup"><span data-stu-id="c1076-132">id</span></span>|<span data-ttu-id="c1076-133">String</span><span class="sxs-lookup"><span data-stu-id="c1076-133">String</span></span>|<span data-ttu-id="c1076-134">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="c1076-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="c1076-135">target</span><span class="sxs-lookup"><span data-stu-id="c1076-135">target</span></span>|[<span data-ttu-id="c1076-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c1076-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c1076-137">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="c1076-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="c1076-138">响应</span><span class="sxs-lookup"><span data-stu-id="c1076-138">Response</span></span>
<span data-ttu-id="c1076-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1076-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1076-140">示例</span><span class="sxs-lookup"><span data-stu-id="c1076-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1076-141">请求</span><span class="sxs-lookup"><span data-stu-id="c1076-141">Request</span></span>
<span data-ttu-id="c1076-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1076-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c1076-143">响应</span><span class="sxs-lookup"><span data-stu-id="c1076-143">Response</span></span>
<span data-ttu-id="c1076-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1076-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




