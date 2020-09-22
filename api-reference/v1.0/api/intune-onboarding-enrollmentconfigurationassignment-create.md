---
title: 创建 enrollmentConfigurationAssignment
description: 创建新的 enrollmentConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce3400784dc7658e6da5b192b0b9012bf1862347
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063084"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="e8807-103">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e8807-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="e8807-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8807-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8807-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8807-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8807-106">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8807-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8807-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8807-107">Prerequisites</span></span>
<span data-ttu-id="e8807-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8807-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8807-110">Permission type</span></span>|<span data-ttu-id="e8807-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8807-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8807-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8807-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8807-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8807-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8807-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8807-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8807-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8807-115">Not supported.</span></span>|
|<span data-ttu-id="e8807-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8807-116">Application</span></span>|<span data-ttu-id="e8807-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8807-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8807-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8807-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e8807-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8807-119">Request headers</span></span>
|<span data-ttu-id="e8807-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8807-120">Header</span></span>|<span data-ttu-id="e8807-121">值</span><span class="sxs-lookup"><span data-stu-id="e8807-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8807-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8807-122">Authorization</span></span>|<span data-ttu-id="e8807-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8807-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8807-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8807-124">Accept</span></span>|<span data-ttu-id="e8807-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8807-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8807-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8807-126">Request body</span></span>
<span data-ttu-id="e8807-127">在请求正文中，提供 enrollmentConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8807-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="e8807-128">下表显示创建 enrollmentConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8807-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="e8807-129">属性</span><span class="sxs-lookup"><span data-stu-id="e8807-129">Property</span></span>|<span data-ttu-id="e8807-130">类型</span><span class="sxs-lookup"><span data-stu-id="e8807-130">Type</span></span>|<span data-ttu-id="e8807-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8807-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8807-132">id</span><span class="sxs-lookup"><span data-stu-id="e8807-132">id</span></span>|<span data-ttu-id="e8807-133">String</span><span class="sxs-lookup"><span data-stu-id="e8807-133">String</span></span>|<span data-ttu-id="e8807-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8807-134">Not yet documented</span></span>|
|<span data-ttu-id="e8807-135">target</span><span class="sxs-lookup"><span data-stu-id="e8807-135">target</span></span>|[<span data-ttu-id="e8807-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e8807-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e8807-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8807-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8807-138">响应</span><span class="sxs-lookup"><span data-stu-id="e8807-138">Response</span></span>
<span data-ttu-id="e8807-139">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8807-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8807-140">示例</span><span class="sxs-lookup"><span data-stu-id="e8807-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8807-141">请求</span><span class="sxs-lookup"><span data-stu-id="e8807-141">Request</span></span>
<span data-ttu-id="e8807-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8807-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e8807-143">响应</span><span class="sxs-lookup"><span data-stu-id="e8807-143">Response</span></span>
<span data-ttu-id="e8807-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









