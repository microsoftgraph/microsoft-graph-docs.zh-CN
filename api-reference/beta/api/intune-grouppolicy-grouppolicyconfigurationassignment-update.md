---
title: 更新 groupPolicyConfigurationAssignment
description: 更新 groupPolicyConfigurationAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1306abca31be57b71b883b7fdaa5d2e8ab47fec4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780537"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="cd494-103">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="cd494-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="cd494-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd494-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd494-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd494-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd494-106">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd494-106">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd494-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd494-107">Prerequisites</span></span>
<span data-ttu-id="cd494-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd494-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd494-110">Permission type</span></span>|<span data-ttu-id="cd494-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd494-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd494-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd494-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd494-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd494-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd494-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd494-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd494-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd494-115">Not supported.</span></span>|
|<span data-ttu-id="cd494-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd494-116">Application</span></span>|<span data-ttu-id="cd494-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd494-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd494-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd494-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cd494-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd494-119">Request headers</span></span>
|<span data-ttu-id="cd494-120">标头</span><span class="sxs-lookup"><span data-stu-id="cd494-120">Header</span></span>|<span data-ttu-id="cd494-121">值</span><span class="sxs-lookup"><span data-stu-id="cd494-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd494-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd494-122">Authorization</span></span>|<span data-ttu-id="cd494-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd494-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd494-124">接受</span><span class="sxs-lookup"><span data-stu-id="cd494-124">Accept</span></span>|<span data-ttu-id="cd494-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd494-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd494-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd494-126">Request body</span></span>
<span data-ttu-id="cd494-127">在请求正文中, 提供[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd494-127">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="cd494-128">下表显示创建[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd494-128">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="cd494-129">属性</span><span class="sxs-lookup"><span data-stu-id="cd494-129">Property</span></span>|<span data-ttu-id="cd494-130">类型</span><span class="sxs-lookup"><span data-stu-id="cd494-130">Type</span></span>|<span data-ttu-id="cd494-131">说明</span><span class="sxs-lookup"><span data-stu-id="cd494-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd494-132">id</span><span class="sxs-lookup"><span data-stu-id="cd494-132">id</span></span>|<span data-ttu-id="cd494-133">String</span><span class="sxs-lookup"><span data-stu-id="cd494-133">String</span></span>|<span data-ttu-id="cd494-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd494-134">Key of the entity.</span></span>|
|<span data-ttu-id="cd494-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd494-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cd494-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd494-136">DateTimeOffset</span></span>|<span data-ttu-id="cd494-137">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cd494-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="cd494-138">target</span><span class="sxs-lookup"><span data-stu-id="cd494-138">target</span></span>|[<span data-ttu-id="cd494-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cd494-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cd494-140">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="cd494-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="cd494-141">响应</span><span class="sxs-lookup"><span data-stu-id="cd494-141">Response</span></span>
<span data-ttu-id="cd494-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cd494-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd494-143">示例</span><span class="sxs-lookup"><span data-stu-id="cd494-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd494-144">请求</span><span class="sxs-lookup"><span data-stu-id="cd494-144">Request</span></span>
<span data-ttu-id="cd494-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd494-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="cd494-146">响应</span><span class="sxs-lookup"><span data-stu-id="cd494-146">Response</span></span>
<span data-ttu-id="cd494-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd494-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





