---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: c05856fbdcd3f5930ac5c40b10c53c7dedbc97ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339562"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="07c96-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07c96-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="07c96-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="07c96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07c96-105">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07c96-105">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07c96-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="07c96-106">Prerequisites</span></span>
<span data-ttu-id="07c96-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="07c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="07c96-109">Permission type</span></span>|<span data-ttu-id="07c96-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="07c96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07c96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07c96-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c96-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07c96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07c96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="07c96-114">Not supported.</span></span>|
|<span data-ttu-id="07c96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="07c96-115">Application</span></span>|<span data-ttu-id="07c96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07c96-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07c96-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="07c96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="07c96-118">Request headers</span></span>
|<span data-ttu-id="07c96-119">标头</span><span class="sxs-lookup"><span data-stu-id="07c96-119">Header</span></span>|<span data-ttu-id="07c96-120">值</span><span class="sxs-lookup"><span data-stu-id="07c96-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c96-121">授权</span><span class="sxs-lookup"><span data-stu-id="07c96-121">Authorization</span></span>|<span data-ttu-id="07c96-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07c96-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c96-123">Accept</span><span class="sxs-lookup"><span data-stu-id="07c96-123">Accept</span></span>|<span data-ttu-id="07c96-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07c96-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c96-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="07c96-125">Request body</span></span>
<span data-ttu-id="07c96-126">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07c96-126">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="07c96-127">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07c96-127">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="07c96-128">属性</span><span class="sxs-lookup"><span data-stu-id="07c96-128">Property</span></span>|<span data-ttu-id="07c96-129">类型</span><span class="sxs-lookup"><span data-stu-id="07c96-129">Type</span></span>|<span data-ttu-id="07c96-130">说明</span><span class="sxs-lookup"><span data-stu-id="07c96-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c96-131">id</span><span class="sxs-lookup"><span data-stu-id="07c96-131">id</span></span>|<span data-ttu-id="07c96-132">字符串</span><span class="sxs-lookup"><span data-stu-id="07c96-132">String</span></span>|<span data-ttu-id="07c96-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="07c96-133">Not yet documented</span></span>|
|<span data-ttu-id="07c96-134">target</span><span class="sxs-lookup"><span data-stu-id="07c96-134">target</span></span>|[<span data-ttu-id="07c96-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="07c96-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="07c96-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="07c96-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="07c96-137">响应</span><span class="sxs-lookup"><span data-stu-id="07c96-137">Response</span></span>
<span data-ttu-id="07c96-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07c96-138">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c96-139">示例</span><span class="sxs-lookup"><span data-stu-id="07c96-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="07c96-140">请求</span><span class="sxs-lookup"><span data-stu-id="07c96-140">Request</span></span>
<span data-ttu-id="07c96-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07c96-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="07c96-142">响应</span><span class="sxs-lookup"><span data-stu-id="07c96-142">Response</span></span>
<span data-ttu-id="07c96-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07c96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



