---
title: 更新 deviceConfigurationAssignment
description: 更新 deviceConfigurationAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d31914b287707ef62a2d3771ffecac99817ebbee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971428"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="4578f-103">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4578f-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="4578f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4578f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4578f-105">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4578f-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4578f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4578f-106">Prerequisites</span></span>
<span data-ttu-id="4578f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4578f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4578f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4578f-109">Permission type</span></span>|<span data-ttu-id="4578f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4578f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4578f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4578f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4578f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4578f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4578f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4578f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4578f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4578f-114">Not supported.</span></span>|
|<span data-ttu-id="4578f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4578f-115">Application</span></span>|<span data-ttu-id="4578f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4578f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4578f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4578f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4578f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4578f-118">Request headers</span></span>
|<span data-ttu-id="4578f-119">标头</span><span class="sxs-lookup"><span data-stu-id="4578f-119">Header</span></span>|<span data-ttu-id="4578f-120">值</span><span class="sxs-lookup"><span data-stu-id="4578f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4578f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4578f-121">Authorization</span></span>|<span data-ttu-id="4578f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4578f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4578f-123">接受</span><span class="sxs-lookup"><span data-stu-id="4578f-123">Accept</span></span>|<span data-ttu-id="4578f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4578f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4578f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4578f-125">Request body</span></span>
<span data-ttu-id="4578f-126">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4578f-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4578f-127">下表显示创建 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4578f-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="4578f-128">属性</span><span class="sxs-lookup"><span data-stu-id="4578f-128">Property</span></span>|<span data-ttu-id="4578f-129">类型</span><span class="sxs-lookup"><span data-stu-id="4578f-129">Type</span></span>|<span data-ttu-id="4578f-130">说明</span><span class="sxs-lookup"><span data-stu-id="4578f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4578f-131">id</span><span class="sxs-lookup"><span data-stu-id="4578f-131">id</span></span>|<span data-ttu-id="4578f-132">String</span><span class="sxs-lookup"><span data-stu-id="4578f-132">String</span></span>|<span data-ttu-id="4578f-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="4578f-133">The key of the assignment.</span></span>|
|<span data-ttu-id="4578f-134">target</span><span class="sxs-lookup"><span data-stu-id="4578f-134">target</span></span>|[<span data-ttu-id="4578f-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4578f-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4578f-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="4578f-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="4578f-137">响应</span><span class="sxs-lookup"><span data-stu-id="4578f-137">Response</span></span>
<span data-ttu-id="4578f-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4578f-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4578f-139">示例</span><span class="sxs-lookup"><span data-stu-id="4578f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="4578f-140">请求</span><span class="sxs-lookup"><span data-stu-id="4578f-140">Request</span></span>
<span data-ttu-id="4578f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4578f-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4578f-142">响应</span><span class="sxs-lookup"><span data-stu-id="4578f-142">Response</span></span>
<span data-ttu-id="4578f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4578f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



