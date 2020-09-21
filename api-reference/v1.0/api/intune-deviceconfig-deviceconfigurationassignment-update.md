---
title: 更新 deviceConfigurationAssignment
description: 更新 deviceConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee50cd2a752ab74897cac42b5a3305842cd93692
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968204"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="e0d91-103">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e0d91-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="e0d91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0d91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0d91-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0d91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0d91-106">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0d91-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0d91-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0d91-107">Prerequisites</span></span>
<span data-ttu-id="e0d91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0d91-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0d91-110">Permission type</span></span>|<span data-ttu-id="e0d91-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0d91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0d91-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0d91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0d91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0d91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0d91-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0d91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0d91-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0d91-115">Not supported.</span></span>|
|<span data-ttu-id="e0d91-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0d91-116">Application</span></span>|<span data-ttu-id="e0d91-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0d91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0d91-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0d91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e0d91-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0d91-119">Request headers</span></span>
|<span data-ttu-id="e0d91-120">标头</span><span class="sxs-lookup"><span data-stu-id="e0d91-120">Header</span></span>|<span data-ttu-id="e0d91-121">值</span><span class="sxs-lookup"><span data-stu-id="e0d91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0d91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0d91-122">Authorization</span></span>|<span data-ttu-id="e0d91-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0d91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0d91-124">接受</span><span class="sxs-lookup"><span data-stu-id="e0d91-124">Accept</span></span>|<span data-ttu-id="e0d91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0d91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0d91-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0d91-126">Request body</span></span>
<span data-ttu-id="e0d91-127">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0d91-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e0d91-128">下表显示创建 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0d91-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="e0d91-129">属性</span><span class="sxs-lookup"><span data-stu-id="e0d91-129">Property</span></span>|<span data-ttu-id="e0d91-130">类型</span><span class="sxs-lookup"><span data-stu-id="e0d91-130">Type</span></span>|<span data-ttu-id="e0d91-131">说明</span><span class="sxs-lookup"><span data-stu-id="e0d91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d91-132">id</span><span class="sxs-lookup"><span data-stu-id="e0d91-132">id</span></span>|<span data-ttu-id="e0d91-133">String</span><span class="sxs-lookup"><span data-stu-id="e0d91-133">String</span></span>|<span data-ttu-id="e0d91-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="e0d91-134">The key of the assignment.</span></span>|
|<span data-ttu-id="e0d91-135">target</span><span class="sxs-lookup"><span data-stu-id="e0d91-135">target</span></span>|[<span data-ttu-id="e0d91-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0d91-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0d91-137">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="e0d91-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="e0d91-138">响应</span><span class="sxs-lookup"><span data-stu-id="e0d91-138">Response</span></span>
<span data-ttu-id="e0d91-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0d91-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0d91-140">示例</span><span class="sxs-lookup"><span data-stu-id="e0d91-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0d91-141">请求</span><span class="sxs-lookup"><span data-stu-id="e0d91-141">Request</span></span>
<span data-ttu-id="e0d91-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0d91-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e0d91-143">响应</span><span class="sxs-lookup"><span data-stu-id="e0d91-143">Response</span></span>
<span data-ttu-id="e0d91-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0d91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```









