---
title: 创建 enrollmentConfigurationAssignment
description: 创建新的 enrollmentConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51e139fbf3c903bb591647566ab74177f397add7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145444"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="42b0e-103">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="42b0e-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="42b0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42b0e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42b0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42b0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42b0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42b0e-107">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42b0e-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42b0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="42b0e-108">Prerequisites</span></span>
<span data-ttu-id="42b0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42b0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42b0e-111">Permission type</span></span>|<span data-ttu-id="42b0e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42b0e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42b0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42b0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42b0e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b0e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42b0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42b0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42b0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42b0e-116">Not supported.</span></span>|
|<span data-ttu-id="42b0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42b0e-117">Application</span></span>|<span data-ttu-id="42b0e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b0e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42b0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42b0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="42b0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42b0e-120">Request headers</span></span>
|<span data-ttu-id="42b0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="42b0e-121">Header</span></span>|<span data-ttu-id="42b0e-122">值</span><span class="sxs-lookup"><span data-stu-id="42b0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42b0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42b0e-123">Authorization</span></span>|<span data-ttu-id="42b0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42b0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42b0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="42b0e-125">Accept</span></span>|<span data-ttu-id="42b0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42b0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42b0e-127">Request body</span></span>
<span data-ttu-id="42b0e-128">在请求正文中，提供 enrollmentConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42b0e-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="42b0e-129">下表显示创建 enrollmentConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42b0e-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="42b0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="42b0e-130">Property</span></span>|<span data-ttu-id="42b0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="42b0e-131">Type</span></span>|<span data-ttu-id="42b0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="42b0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42b0e-133">id</span><span class="sxs-lookup"><span data-stu-id="42b0e-133">id</span></span>|<span data-ttu-id="42b0e-134">String</span><span class="sxs-lookup"><span data-stu-id="42b0e-134">String</span></span>|<span data-ttu-id="42b0e-135">注册配置分配密钥</span><span class="sxs-lookup"><span data-stu-id="42b0e-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="42b0e-136">target</span><span class="sxs-lookup"><span data-stu-id="42b0e-136">target</span></span>|[<span data-ttu-id="42b0e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42b0e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="42b0e-138">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="42b0e-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="42b0e-139">source</span><span class="sxs-lookup"><span data-stu-id="42b0e-139">source</span></span>|[<span data-ttu-id="42b0e-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="42b0e-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="42b0e-141">用于部署到组、直接或 policySet 的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="42b0e-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="42b0e-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="42b0e-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="42b0e-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="42b0e-143">sourceId</span></span>|<span data-ttu-id="42b0e-144">String</span><span class="sxs-lookup"><span data-stu-id="42b0e-144">String</span></span>|<span data-ttu-id="42b0e-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="42b0e-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="42b0e-146">响应</span><span class="sxs-lookup"><span data-stu-id="42b0e-146">Response</span></span>
<span data-ttu-id="42b0e-147">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42b0e-147">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b0e-148">示例</span><span class="sxs-lookup"><span data-stu-id="42b0e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="42b0e-149">请求</span><span class="sxs-lookup"><span data-stu-id="42b0e-149">Request</span></span>
<span data-ttu-id="42b0e-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42b0e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="42b0e-151">响应</span><span class="sxs-lookup"><span data-stu-id="42b0e-151">Response</span></span>
<span data-ttu-id="42b0e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42b0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




