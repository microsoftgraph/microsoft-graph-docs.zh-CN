---
title: 更新 groupPolicyConfigurationAssignment
description: 更新 groupPolicyConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eaed9dd4d91ddd6bb10a21cce140f8e7984672f8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791964"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="7afa6-103">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7afa6-103">Update groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="7afa6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7afa6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7afa6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7afa6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7afa6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7afa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7afa6-107">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7afa6-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7afa6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7afa6-108">Prerequisites</span></span>
<span data-ttu-id="7afa6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7afa6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7afa6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7afa6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7afa6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7afa6-111">Permission type</span></span>|<span data-ttu-id="7afa6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7afa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7afa6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7afa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7afa6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7afa6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7afa6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7afa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7afa6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7afa6-116">Not supported.</span></span>|
|<span data-ttu-id="7afa6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7afa6-117">Application</span></span>|<span data-ttu-id="7afa6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7afa6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7afa6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7afa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7afa6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7afa6-120">Request headers</span></span>
|<span data-ttu-id="7afa6-121">标头</span><span class="sxs-lookup"><span data-stu-id="7afa6-121">Header</span></span>|<span data-ttu-id="7afa6-122">值</span><span class="sxs-lookup"><span data-stu-id="7afa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7afa6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7afa6-123">Authorization</span></span>|<span data-ttu-id="7afa6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7afa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7afa6-125">接受</span><span class="sxs-lookup"><span data-stu-id="7afa6-125">Accept</span></span>|<span data-ttu-id="7afa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7afa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7afa6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7afa6-127">Request body</span></span>
<span data-ttu-id="7afa6-128">在请求正文中，提供[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7afa6-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7afa6-129">下表显示创建[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7afa6-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="7afa6-130">属性</span><span class="sxs-lookup"><span data-stu-id="7afa6-130">Property</span></span>|<span data-ttu-id="7afa6-131">类型</span><span class="sxs-lookup"><span data-stu-id="7afa6-131">Type</span></span>|<span data-ttu-id="7afa6-132">说明</span><span class="sxs-lookup"><span data-stu-id="7afa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7afa6-133">id</span><span class="sxs-lookup"><span data-stu-id="7afa6-133">id</span></span>|<span data-ttu-id="7afa6-134">String</span><span class="sxs-lookup"><span data-stu-id="7afa6-134">String</span></span>|<span data-ttu-id="7afa6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7afa6-135">Key of the entity.</span></span>|
|<span data-ttu-id="7afa6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7afa6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7afa6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7afa6-137">DateTimeOffset</span></span>|<span data-ttu-id="7afa6-138">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7afa6-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="7afa6-139">target</span><span class="sxs-lookup"><span data-stu-id="7afa6-139">target</span></span>|[<span data-ttu-id="7afa6-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7afa6-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7afa6-141">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="7afa6-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="7afa6-142">响应</span><span class="sxs-lookup"><span data-stu-id="7afa6-142">Response</span></span>
<span data-ttu-id="7afa6-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7afa6-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7afa6-144">示例</span><span class="sxs-lookup"><span data-stu-id="7afa6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7afa6-145">请求</span><span class="sxs-lookup"><span data-stu-id="7afa6-145">Request</span></span>
<span data-ttu-id="7afa6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7afa6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="7afa6-147">响应</span><span class="sxs-lookup"><span data-stu-id="7afa6-147">Response</span></span>
<span data-ttu-id="7afa6-148">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7afa6-148">Here is an example of the response.</span></span> <span data-ttu-id="7afa6-149">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7afa6-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7afa6-150">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7afa6-150">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



