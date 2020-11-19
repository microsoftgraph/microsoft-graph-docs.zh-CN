---
title: 创建 groupPolicyConfigurationAssignment
description: 创建新的 groupPolicyConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d135faf9b8cac07c159e22eee6fdbd5cd9e46b15
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212200"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="c16db-103">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c16db-103">Create groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="c16db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c16db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c16db-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c16db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c16db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c16db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c16db-107">创建新的 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c16db-107">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c16db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c16db-108">Prerequisites</span></span>
<span data-ttu-id="c16db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c16db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c16db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c16db-111">Permission type</span></span>|<span data-ttu-id="c16db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c16db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c16db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c16db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c16db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c16db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c16db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c16db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c16db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c16db-116">Not supported.</span></span>|
|<span data-ttu-id="c16db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c16db-117">Application</span></span>|<span data-ttu-id="c16db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c16db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c16db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c16db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c16db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c16db-120">Request headers</span></span>
|<span data-ttu-id="c16db-121">标头</span><span class="sxs-lookup"><span data-stu-id="c16db-121">Header</span></span>|<span data-ttu-id="c16db-122">值</span><span class="sxs-lookup"><span data-stu-id="c16db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c16db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c16db-123">Authorization</span></span>|<span data-ttu-id="c16db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c16db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c16db-125">接受</span><span class="sxs-lookup"><span data-stu-id="c16db-125">Accept</span></span>|<span data-ttu-id="c16db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c16db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c16db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c16db-127">Request body</span></span>
<span data-ttu-id="c16db-128">在请求正文中，提供 groupPolicyConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c16db-128">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="c16db-129">下表显示创建 groupPolicyConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c16db-129">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="c16db-130">属性</span><span class="sxs-lookup"><span data-stu-id="c16db-130">Property</span></span>|<span data-ttu-id="c16db-131">类型</span><span class="sxs-lookup"><span data-stu-id="c16db-131">Type</span></span>|<span data-ttu-id="c16db-132">说明</span><span class="sxs-lookup"><span data-stu-id="c16db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c16db-133">id</span><span class="sxs-lookup"><span data-stu-id="c16db-133">id</span></span>|<span data-ttu-id="c16db-134">String</span><span class="sxs-lookup"><span data-stu-id="c16db-134">String</span></span>|<span data-ttu-id="c16db-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c16db-135">Key of the entity.</span></span>|
|<span data-ttu-id="c16db-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c16db-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c16db-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c16db-137">DateTimeOffset</span></span>|<span data-ttu-id="c16db-138">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c16db-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c16db-139">target</span><span class="sxs-lookup"><span data-stu-id="c16db-139">target</span></span>|[<span data-ttu-id="c16db-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c16db-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c16db-141">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="c16db-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c16db-142">响应</span><span class="sxs-lookup"><span data-stu-id="c16db-142">Response</span></span>
<span data-ttu-id="c16db-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c16db-143">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c16db-144">示例</span><span class="sxs-lookup"><span data-stu-id="c16db-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c16db-145">请求</span><span class="sxs-lookup"><span data-stu-id="c16db-145">Request</span></span>
<span data-ttu-id="c16db-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c16db-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="c16db-147">响应</span><span class="sxs-lookup"><span data-stu-id="c16db-147">Response</span></span>
<span data-ttu-id="c16db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c16db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




