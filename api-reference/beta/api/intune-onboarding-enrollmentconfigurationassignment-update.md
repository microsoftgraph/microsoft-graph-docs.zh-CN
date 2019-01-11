---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f4aba8c5e1cd6a392661e84d60cf11496ec39f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868101"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="eb354-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eb354-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="eb354-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb354-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb354-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb354-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb354-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb354-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb354-107">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb354-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb354-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb354-108">Prerequisites</span></span>
<span data-ttu-id="eb354-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eb354-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb354-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb354-111">Permission type</span></span>|<span data-ttu-id="eb354-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb354-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb354-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb354-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb354-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb354-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb354-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb354-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb354-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb354-116">Not supported.</span></span>|
|<span data-ttu-id="eb354-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb354-117">Application</span></span>|<span data-ttu-id="eb354-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb354-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb354-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb354-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eb354-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb354-120">Request headers</span></span>
|<span data-ttu-id="eb354-121">标头</span><span class="sxs-lookup"><span data-stu-id="eb354-121">Header</span></span>|<span data-ttu-id="eb354-122">值</span><span class="sxs-lookup"><span data-stu-id="eb354-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb354-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb354-123">Authorization</span></span>|<span data-ttu-id="eb354-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb354-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb354-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb354-125">Accept</span></span>|<span data-ttu-id="eb354-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb354-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb354-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb354-127">Request body</span></span>
<span data-ttu-id="eb354-128">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb354-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="eb354-129">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb354-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="eb354-130">属性</span><span class="sxs-lookup"><span data-stu-id="eb354-130">Property</span></span>|<span data-ttu-id="eb354-131">类型</span><span class="sxs-lookup"><span data-stu-id="eb354-131">Type</span></span>|<span data-ttu-id="eb354-132">说明</span><span class="sxs-lookup"><span data-stu-id="eb354-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb354-133">id</span><span class="sxs-lookup"><span data-stu-id="eb354-133">id</span></span>|<span data-ttu-id="eb354-134">字符串</span><span class="sxs-lookup"><span data-stu-id="eb354-134">String</span></span>|<span data-ttu-id="eb354-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eb354-135">Not yet documented</span></span>|
|<span data-ttu-id="eb354-136">target</span><span class="sxs-lookup"><span data-stu-id="eb354-136">target</span></span>|[<span data-ttu-id="eb354-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eb354-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eb354-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eb354-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eb354-139">响应</span><span class="sxs-lookup"><span data-stu-id="eb354-139">Response</span></span>
<span data-ttu-id="eb354-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb354-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb354-141">示例</span><span class="sxs-lookup"><span data-stu-id="eb354-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb354-142">请求</span><span class="sxs-lookup"><span data-stu-id="eb354-142">Request</span></span>
<span data-ttu-id="eb354-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb354-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="eb354-144">响应</span><span class="sxs-lookup"><span data-stu-id="eb354-144">Response</span></span>
<span data-ttu-id="eb354-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb354-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





