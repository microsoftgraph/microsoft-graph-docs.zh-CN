---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 506b2ac619d13c3c07fd815ea389b9d06f1109ae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980899"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="e16a5-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e16a5-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="e16a5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e16a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e16a5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e16a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e16a5-106">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e16a5-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e16a5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e16a5-107">Prerequisites</span></span>
<span data-ttu-id="e16a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e16a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e16a5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e16a5-110">Permission type</span></span>|<span data-ttu-id="e16a5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e16a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e16a5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e16a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e16a5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e16a5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e16a5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e16a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e16a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e16a5-115">Not supported.</span></span>|
|<span data-ttu-id="e16a5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e16a5-116">Application</span></span>|<span data-ttu-id="e16a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e16a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e16a5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e16a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e16a5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e16a5-119">Request headers</span></span>
|<span data-ttu-id="e16a5-120">标头</span><span class="sxs-lookup"><span data-stu-id="e16a5-120">Header</span></span>|<span data-ttu-id="e16a5-121">值</span><span class="sxs-lookup"><span data-stu-id="e16a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e16a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e16a5-122">Authorization</span></span>|<span data-ttu-id="e16a5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e16a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e16a5-124">接受</span><span class="sxs-lookup"><span data-stu-id="e16a5-124">Accept</span></span>|<span data-ttu-id="e16a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e16a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e16a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e16a5-126">Request body</span></span>
<span data-ttu-id="e16a5-127">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e16a5-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e16a5-128">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e16a5-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="e16a5-129">属性</span><span class="sxs-lookup"><span data-stu-id="e16a5-129">Property</span></span>|<span data-ttu-id="e16a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="e16a5-130">Type</span></span>|<span data-ttu-id="e16a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="e16a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e16a5-132">id</span><span class="sxs-lookup"><span data-stu-id="e16a5-132">id</span></span>|<span data-ttu-id="e16a5-133">String</span><span class="sxs-lookup"><span data-stu-id="e16a5-133">String</span></span>|<span data-ttu-id="e16a5-134">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="e16a5-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="e16a5-135">target</span><span class="sxs-lookup"><span data-stu-id="e16a5-135">target</span></span>|[<span data-ttu-id="e16a5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e16a5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e16a5-137">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="e16a5-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="e16a5-138">响应</span><span class="sxs-lookup"><span data-stu-id="e16a5-138">Response</span></span>
<span data-ttu-id="e16a5-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e16a5-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e16a5-140">示例</span><span class="sxs-lookup"><span data-stu-id="e16a5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e16a5-141">请求</span><span class="sxs-lookup"><span data-stu-id="e16a5-141">Request</span></span>
<span data-ttu-id="e16a5-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e16a5-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e16a5-143">响应</span><span class="sxs-lookup"><span data-stu-id="e16a5-143">Response</span></span>
<span data-ttu-id="e16a5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e16a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





