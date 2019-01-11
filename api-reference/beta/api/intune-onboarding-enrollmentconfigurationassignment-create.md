---
title: 创建 enrollmentConfigurationAssignment
description: 创建新的 enrollmentConfigurationAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5541b89a01ea0384506803f605ee33abc6fe32aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873827"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="672c4-103">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="672c4-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="672c4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="672c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="672c4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="672c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="672c4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="672c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="672c4-107">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="672c4-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="672c4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="672c4-108">Prerequisites</span></span>
<span data-ttu-id="672c4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="672c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="672c4-111">Permission type</span></span>|<span data-ttu-id="672c4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="672c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="672c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="672c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="672c4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672c4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="672c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="672c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="672c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="672c4-116">Not supported.</span></span>|
|<span data-ttu-id="672c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="672c4-117">Application</span></span>|<span data-ttu-id="672c4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="672c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="672c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="672c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="672c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="672c4-120">Request headers</span></span>
|<span data-ttu-id="672c4-121">标头</span><span class="sxs-lookup"><span data-stu-id="672c4-121">Header</span></span>|<span data-ttu-id="672c4-122">值</span><span class="sxs-lookup"><span data-stu-id="672c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="672c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="672c4-123">Authorization</span></span>|<span data-ttu-id="672c4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="672c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="672c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="672c4-125">Accept</span></span>|<span data-ttu-id="672c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="672c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="672c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="672c4-127">Request body</span></span>
<span data-ttu-id="672c4-128">在请求正文中，提供 enrollmentConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="672c4-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="672c4-129">下表显示创建 enrollmentConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="672c4-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="672c4-130">属性</span><span class="sxs-lookup"><span data-stu-id="672c4-130">Property</span></span>|<span data-ttu-id="672c4-131">类型</span><span class="sxs-lookup"><span data-stu-id="672c4-131">Type</span></span>|<span data-ttu-id="672c4-132">说明</span><span class="sxs-lookup"><span data-stu-id="672c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="672c4-133">id</span><span class="sxs-lookup"><span data-stu-id="672c4-133">id</span></span>|<span data-ttu-id="672c4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="672c4-134">String</span></span>|<span data-ttu-id="672c4-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="672c4-135">Not yet documented</span></span>|
|<span data-ttu-id="672c4-136">target</span><span class="sxs-lookup"><span data-stu-id="672c4-136">target</span></span>|[<span data-ttu-id="672c4-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="672c4-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="672c4-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="672c4-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="672c4-139">响应</span><span class="sxs-lookup"><span data-stu-id="672c4-139">Response</span></span>
<span data-ttu-id="672c4-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="672c4-140">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="672c4-141">示例</span><span class="sxs-lookup"><span data-stu-id="672c4-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="672c4-142">请求</span><span class="sxs-lookup"><span data-stu-id="672c4-142">Request</span></span>
<span data-ttu-id="672c4-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="672c4-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="672c4-144">响应</span><span class="sxs-lookup"><span data-stu-id="672c4-144">Response</span></span>
<span data-ttu-id="672c4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="672c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





