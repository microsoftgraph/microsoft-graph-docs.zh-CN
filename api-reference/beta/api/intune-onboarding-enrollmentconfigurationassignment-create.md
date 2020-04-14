---
title: 创建 enrollmentConfigurationAssignment
description: 创建新的 enrollmentConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 318fc6d46fdc2598292e96f89e07fa14819ef5f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441391"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="911de-103">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="911de-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="911de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="911de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="911de-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="911de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="911de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="911de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="911de-107">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="911de-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="911de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="911de-108">Prerequisites</span></span>
<span data-ttu-id="911de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="911de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="911de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="911de-111">Permission type</span></span>|<span data-ttu-id="911de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="911de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="911de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="911de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="911de-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911de-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="911de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="911de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="911de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="911de-116">Not supported.</span></span>|
|<span data-ttu-id="911de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="911de-117">Application</span></span>|<span data-ttu-id="911de-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911de-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="911de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="911de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="911de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="911de-120">Request headers</span></span>
|<span data-ttu-id="911de-121">标头</span><span class="sxs-lookup"><span data-stu-id="911de-121">Header</span></span>|<span data-ttu-id="911de-122">值</span><span class="sxs-lookup"><span data-stu-id="911de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="911de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="911de-123">Authorization</span></span>|<span data-ttu-id="911de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="911de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="911de-125">接受</span><span class="sxs-lookup"><span data-stu-id="911de-125">Accept</span></span>|<span data-ttu-id="911de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="911de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="911de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="911de-127">Request body</span></span>
<span data-ttu-id="911de-128">在请求正文中，提供 enrollmentConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="911de-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="911de-129">下表显示创建 enrollmentConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="911de-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="911de-130">属性</span><span class="sxs-lookup"><span data-stu-id="911de-130">Property</span></span>|<span data-ttu-id="911de-131">类型</span><span class="sxs-lookup"><span data-stu-id="911de-131">Type</span></span>|<span data-ttu-id="911de-132">说明</span><span class="sxs-lookup"><span data-stu-id="911de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="911de-133">id</span><span class="sxs-lookup"><span data-stu-id="911de-133">id</span></span>|<span data-ttu-id="911de-134">String</span><span class="sxs-lookup"><span data-stu-id="911de-134">String</span></span>|<span data-ttu-id="911de-135">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="911de-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="911de-136">target</span><span class="sxs-lookup"><span data-stu-id="911de-136">target</span></span>|[<span data-ttu-id="911de-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="911de-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="911de-138">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="911de-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="911de-139">source</span><span class="sxs-lookup"><span data-stu-id="911de-139">source</span></span>|[<span data-ttu-id="911de-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="911de-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="911de-141">用于部署到组、direct 或 policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="911de-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="911de-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="911de-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="911de-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="911de-143">sourceId</span></span>|<span data-ttu-id="911de-144">String</span><span class="sxs-lookup"><span data-stu-id="911de-144">String</span></span>|<span data-ttu-id="911de-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="911de-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="911de-146">响应</span><span class="sxs-lookup"><span data-stu-id="911de-146">Response</span></span>
<span data-ttu-id="911de-147">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="911de-147">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="911de-148">示例</span><span class="sxs-lookup"><span data-stu-id="911de-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="911de-149">请求</span><span class="sxs-lookup"><span data-stu-id="911de-149">Request</span></span>
<span data-ttu-id="911de-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="911de-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="911de-151">响应</span><span class="sxs-lookup"><span data-stu-id="911de-151">Response</span></span>
<span data-ttu-id="911de-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="911de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



