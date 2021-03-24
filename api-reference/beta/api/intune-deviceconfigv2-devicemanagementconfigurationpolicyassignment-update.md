---
title: 更新 deviceManagementConfigurationPolicyAssignment
description: 更新 deviceManagementConfigurationPolicyAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ee9a8db3a360d3576068fb5229ca3448cb3da68
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147054"
---
# <a name="update-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="45d1f-103">更新 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="45d1f-103">Update deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="45d1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45d1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d1f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45d1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d1f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45d1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d1f-107">更新 [deviceManagementConfigurationPolicyAssignment 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="45d1f-107">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45d1f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="45d1f-108">Prerequisites</span></span>
<span data-ttu-id="45d1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d1f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="45d1f-111">Permission type</span></span>|<span data-ttu-id="45d1f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45d1f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d1f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45d1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45d1f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45d1f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45d1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45d1f-116">Not supported.</span></span>|
|<span data-ttu-id="45d1f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="45d1f-117">Application</span></span>|<span data-ttu-id="45d1f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d1f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45d1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="45d1f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="45d1f-120">Request headers</span></span>
|<span data-ttu-id="45d1f-121">标头</span><span class="sxs-lookup"><span data-stu-id="45d1f-121">Header</span></span>|<span data-ttu-id="45d1f-122">值</span><span class="sxs-lookup"><span data-stu-id="45d1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d1f-123">Authorization</span></span>|<span data-ttu-id="45d1f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45d1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d1f-125">接受</span><span class="sxs-lookup"><span data-stu-id="45d1f-125">Accept</span></span>|<span data-ttu-id="45d1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d1f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45d1f-127">Request body</span></span>
<span data-ttu-id="45d1f-128">在请求正文中，提供 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45d1f-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

<span data-ttu-id="45d1f-129">下表显示创建 [deviceManagementConfigurationPolicyAssignment 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="45d1f-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>

|<span data-ttu-id="45d1f-130">属性</span><span class="sxs-lookup"><span data-stu-id="45d1f-130">Property</span></span>|<span data-ttu-id="45d1f-131">类型</span><span class="sxs-lookup"><span data-stu-id="45d1f-131">Type</span></span>|<span data-ttu-id="45d1f-132">说明</span><span class="sxs-lookup"><span data-stu-id="45d1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d1f-133">id</span><span class="sxs-lookup"><span data-stu-id="45d1f-133">id</span></span>|<span data-ttu-id="45d1f-134">String</span><span class="sxs-lookup"><span data-stu-id="45d1f-134">String</span></span>|<span data-ttu-id="45d1f-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="45d1f-135">The key of the assignment.</span></span>|
|<span data-ttu-id="45d1f-136">target</span><span class="sxs-lookup"><span data-stu-id="45d1f-136">target</span></span>|[<span data-ttu-id="45d1f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="45d1f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="45d1f-138">DeviceManagementConfigurationPolicy 的分配目标。</span><span class="sxs-lookup"><span data-stu-id="45d1f-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="45d1f-139">响应</span><span class="sxs-lookup"><span data-stu-id="45d1f-139">Response</span></span>
<span data-ttu-id="45d1f-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45d1f-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d1f-141">示例</span><span class="sxs-lookup"><span data-stu-id="45d1f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="45d1f-142">请求</span><span class="sxs-lookup"><span data-stu-id="45d1f-142">Request</span></span>
<span data-ttu-id="45d1f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45d1f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="45d1f-144">响应</span><span class="sxs-lookup"><span data-stu-id="45d1f-144">Response</span></span>
<span data-ttu-id="45d1f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45d1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




