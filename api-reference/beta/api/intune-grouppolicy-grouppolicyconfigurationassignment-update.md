---
title: 更新 groupPolicyConfigurationAssignment
description: 更新 groupPolicyConfigurationAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08ff87b70b833dc1f8423a8465b5b880660fd462
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431382"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="4e16f-103">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4e16f-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="4e16f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4e16f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e16f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4e16f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e16f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e16f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e16f-107">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4e16f-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e16f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e16f-108">Prerequisites</span></span>
<span data-ttu-id="4e16f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4e16f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e16f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e16f-111">Permission type</span></span>|<span data-ttu-id="4e16f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e16f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e16f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e16f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e16f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e16f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4e16f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e16f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e16f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e16f-116">Not supported.</span></span>|
|<span data-ttu-id="4e16f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e16f-117">Application</span></span>|<span data-ttu-id="4e16f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e16f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e16f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e16f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4e16f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e16f-120">Request headers</span></span>
|<span data-ttu-id="4e16f-121">标头</span><span class="sxs-lookup"><span data-stu-id="4e16f-121">Header</span></span>|<span data-ttu-id="4e16f-122">值</span><span class="sxs-lookup"><span data-stu-id="4e16f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e16f-123">授权</span><span class="sxs-lookup"><span data-stu-id="4e16f-123">Authorization</span></span>|<span data-ttu-id="4e16f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4e16f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e16f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e16f-125">Accept</span></span>|<span data-ttu-id="4e16f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e16f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e16f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e16f-127">Request body</span></span>
<span data-ttu-id="4e16f-128">在请求正文中，提供[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e16f-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4e16f-129">下表显示时创建[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4e16f-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="4e16f-130">属性</span><span class="sxs-lookup"><span data-stu-id="4e16f-130">Property</span></span>|<span data-ttu-id="4e16f-131">类型</span><span class="sxs-lookup"><span data-stu-id="4e16f-131">Type</span></span>|<span data-ttu-id="4e16f-132">说明</span><span class="sxs-lookup"><span data-stu-id="4e16f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e16f-133">id</span><span class="sxs-lookup"><span data-stu-id="4e16f-133">id</span></span>|<span data-ttu-id="4e16f-134">String</span><span class="sxs-lookup"><span data-stu-id="4e16f-134">String</span></span>|<span data-ttu-id="4e16f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4e16f-135">Key of the entity.</span></span>|
|<span data-ttu-id="4e16f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e16f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e16f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e16f-137">DateTimeOffset</span></span>|<span data-ttu-id="4e16f-138">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="4e16f-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="4e16f-139">target</span><span class="sxs-lookup"><span data-stu-id="4e16f-139">target</span></span>|[<span data-ttu-id="4e16f-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4e16f-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4e16f-141">组类型目标组策略配置。</span><span class="sxs-lookup"><span data-stu-id="4e16f-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="4e16f-142">响应</span><span class="sxs-lookup"><span data-stu-id="4e16f-142">Response</span></span>
<span data-ttu-id="4e16f-143">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e16f-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e16f-144">示例</span><span class="sxs-lookup"><span data-stu-id="4e16f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e16f-145">请求</span><span class="sxs-lookup"><span data-stu-id="4e16f-145">Request</span></span>
<span data-ttu-id="4e16f-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e16f-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e16f-147">响应</span><span class="sxs-lookup"><span data-stu-id="4e16f-147">Response</span></span>
<span data-ttu-id="4e16f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e16f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




