---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 928abb0869a401015a6485e240d5ebd2336a7d3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403600"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="6e69f-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6e69f-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="6e69f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6e69f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e69f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e69f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e69f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e69f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e69f-107">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e69f-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e69f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e69f-108">Prerequisites</span></span>
<span data-ttu-id="6e69f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6e69f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e69f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e69f-111">Permission type</span></span>|<span data-ttu-id="6e69f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e69f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e69f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e69f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e69f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e69f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e69f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e69f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e69f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e69f-116">Not supported.</span></span>|
|<span data-ttu-id="6e69f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e69f-117">Application</span></span>|<span data-ttu-id="6e69f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e69f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e69f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e69f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6e69f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e69f-120">Request headers</span></span>
|<span data-ttu-id="6e69f-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e69f-121">Header</span></span>|<span data-ttu-id="6e69f-122">值</span><span class="sxs-lookup"><span data-stu-id="6e69f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e69f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e69f-123">Authorization</span></span>|<span data-ttu-id="6e69f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e69f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e69f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e69f-125">Accept</span></span>|<span data-ttu-id="6e69f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e69f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e69f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e69f-127">Request body</span></span>
<span data-ttu-id="6e69f-128">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e69f-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6e69f-129">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e69f-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="6e69f-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e69f-130">Property</span></span>|<span data-ttu-id="6e69f-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e69f-131">Type</span></span>|<span data-ttu-id="6e69f-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e69f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e69f-133">id</span><span class="sxs-lookup"><span data-stu-id="6e69f-133">id</span></span>|<span data-ttu-id="6e69f-134">String</span><span class="sxs-lookup"><span data-stu-id="6e69f-134">String</span></span>|<span data-ttu-id="6e69f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e69f-135">Not yet documented</span></span>|
|<span data-ttu-id="6e69f-136">target</span><span class="sxs-lookup"><span data-stu-id="6e69f-136">target</span></span>|[<span data-ttu-id="6e69f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6e69f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6e69f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e69f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e69f-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e69f-139">Response</span></span>
<span data-ttu-id="6e69f-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e69f-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e69f-141">示例</span><span class="sxs-lookup"><span data-stu-id="6e69f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e69f-142">请求</span><span class="sxs-lookup"><span data-stu-id="6e69f-142">Request</span></span>
<span data-ttu-id="6e69f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e69f-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e69f-144">响应</span><span class="sxs-lookup"><span data-stu-id="6e69f-144">Response</span></span>
<span data-ttu-id="6e69f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e69f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




