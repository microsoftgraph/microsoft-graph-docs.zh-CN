---
title: 创建 deviceManagementConfigurationPolicyAssignment
description: 创建新的 deviceManagementConfigurationPolicyAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdacc5f360340e6e07de25183ed53ddce181b15e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301589"
---
# <a name="create-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="06c25-103">创建 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="06c25-103">Create deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="06c25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06c25-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06c25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06c25-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06c25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c25-107">创建新的 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06c25-107">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06c25-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="06c25-108">Prerequisites</span></span>
<span data-ttu-id="06c25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06c25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06c25-111">Permission type</span></span>|<span data-ttu-id="06c25-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06c25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06c25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06c25-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c25-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06c25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06c25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06c25-116">Not supported.</span></span>|
|<span data-ttu-id="06c25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06c25-117">Application</span></span>|<span data-ttu-id="06c25-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c25-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06c25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="06c25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06c25-120">Request headers</span></span>
|<span data-ttu-id="06c25-121">标头</span><span class="sxs-lookup"><span data-stu-id="06c25-121">Header</span></span>|<span data-ttu-id="06c25-122">值</span><span class="sxs-lookup"><span data-stu-id="06c25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c25-123">Authorization</span></span>|<span data-ttu-id="06c25-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06c25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c25-125">接受</span><span class="sxs-lookup"><span data-stu-id="06c25-125">Accept</span></span>|<span data-ttu-id="06c25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06c25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="06c25-127">Request body</span></span>
<span data-ttu-id="06c25-128">在请求正文中，提供 deviceManagementConfigurationPolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06c25-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyAssignment object.</span></span>

<span data-ttu-id="06c25-129">下表显示创建 deviceManagementConfigurationPolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06c25-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyAssignment.</span></span>

|<span data-ttu-id="06c25-130">属性</span><span class="sxs-lookup"><span data-stu-id="06c25-130">Property</span></span>|<span data-ttu-id="06c25-131">类型</span><span class="sxs-lookup"><span data-stu-id="06c25-131">Type</span></span>|<span data-ttu-id="06c25-132">说明</span><span class="sxs-lookup"><span data-stu-id="06c25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c25-133">id</span><span class="sxs-lookup"><span data-stu-id="06c25-133">id</span></span>|<span data-ttu-id="06c25-134">字符串</span><span class="sxs-lookup"><span data-stu-id="06c25-134">String</span></span>|<span data-ttu-id="06c25-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="06c25-135">The key of the assignment.</span></span>|
|<span data-ttu-id="06c25-136">target</span><span class="sxs-lookup"><span data-stu-id="06c25-136">target</span></span>|[<span data-ttu-id="06c25-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="06c25-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="06c25-138">DeviceManagementConfigurationPolicy 的分配目标。</span><span class="sxs-lookup"><span data-stu-id="06c25-138">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|



## <a name="response"></a><span data-ttu-id="06c25-139">响应</span><span class="sxs-lookup"><span data-stu-id="06c25-139">Response</span></span>
<span data-ttu-id="06c25-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06c25-140">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c25-141">示例</span><span class="sxs-lookup"><span data-stu-id="06c25-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="06c25-142">请求</span><span class="sxs-lookup"><span data-stu-id="06c25-142">Request</span></span>
<span data-ttu-id="06c25-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06c25-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="06c25-144">响应</span><span class="sxs-lookup"><span data-stu-id="06c25-144">Response</span></span>
<span data-ttu-id="06c25-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06c25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "1f069921-9921-1f06-2199-061f2199061f",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




