---
title: 更新 enrollmentConfigurationAssignment
description: 更新 enrollmentConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fe867edace02c5b1735783491d9e760cf799dc3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178316"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="c1224-103">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c1224-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="c1224-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1224-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1224-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1224-107">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1224-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1224-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1224-108">Prerequisites</span></span>
<span data-ttu-id="c1224-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1224-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1224-111">Permission type</span></span>|<span data-ttu-id="c1224-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1224-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1224-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1224-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1224-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1224-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1224-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1224-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1224-116">Not supported.</span></span>|
|<span data-ttu-id="c1224-117">Application</span><span class="sxs-lookup"><span data-stu-id="c1224-117">Application</span></span>|<span data-ttu-id="c1224-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1224-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1224-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1224-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1224-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1224-120">Request headers</span></span>
|<span data-ttu-id="c1224-121">标头</span><span class="sxs-lookup"><span data-stu-id="c1224-121">Header</span></span>|<span data-ttu-id="c1224-122">值</span><span class="sxs-lookup"><span data-stu-id="c1224-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1224-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1224-123">Authorization</span></span>|<span data-ttu-id="c1224-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1224-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1224-125">接受</span><span class="sxs-lookup"><span data-stu-id="c1224-125">Accept</span></span>|<span data-ttu-id="c1224-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1224-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1224-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1224-127">Request body</span></span>
<span data-ttu-id="c1224-128">在请求正文中，提供 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1224-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c1224-129">下表显示创建 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1224-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="c1224-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1224-130">Property</span></span>|<span data-ttu-id="c1224-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1224-131">Type</span></span>|<span data-ttu-id="c1224-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1224-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1224-133">id</span><span class="sxs-lookup"><span data-stu-id="c1224-133">id</span></span>|<span data-ttu-id="c1224-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c1224-134">String</span></span>|<span data-ttu-id="c1224-135">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="c1224-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="c1224-136">target</span><span class="sxs-lookup"><span data-stu-id="c1224-136">target</span></span>|[<span data-ttu-id="c1224-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c1224-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c1224-138">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="c1224-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="c1224-139">source</span><span class="sxs-lookup"><span data-stu-id="c1224-139">source</span></span>|[<span data-ttu-id="c1224-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="c1224-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="c1224-141">用于部署到组、direct 或 policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="c1224-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="c1224-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="c1224-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="c1224-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="c1224-143">sourceId</span></span>|<span data-ttu-id="c1224-144">字符串</span><span class="sxs-lookup"><span data-stu-id="c1224-144">String</span></span>|<span data-ttu-id="c1224-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="c1224-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="c1224-146">响应</span><span class="sxs-lookup"><span data-stu-id="c1224-146">Response</span></span>
<span data-ttu-id="c1224-147">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1224-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1224-148">示例</span><span class="sxs-lookup"><span data-stu-id="c1224-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1224-149">请求</span><span class="sxs-lookup"><span data-stu-id="c1224-149">Request</span></span>
<span data-ttu-id="c1224-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1224-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="c1224-151">响应</span><span class="sxs-lookup"><span data-stu-id="c1224-151">Response</span></span>
<span data-ttu-id="c1224-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1224-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



