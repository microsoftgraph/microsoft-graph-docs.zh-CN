---
title: 更新 managedDeviceMobileAppConfigurationAssignment
description: 更新 managedDeviceMobileAppConfigurationAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f70a6e1f0f29eed83dc28e2168d4c7c76eb8bc7c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173064"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="3d062-103">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3d062-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="3d062-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d062-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d062-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d062-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d062-106">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d062-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d062-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d062-107">Prerequisites</span></span>
<span data-ttu-id="3d062-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d062-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d062-110">Permission type</span></span>|<span data-ttu-id="3d062-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d062-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d062-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d062-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d062-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d062-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d062-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d062-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d062-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d062-115">Not supported.</span></span>|
|<span data-ttu-id="3d062-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d062-116">Application</span></span>|<span data-ttu-id="3d062-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d062-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d062-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d062-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3d062-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d062-119">Request headers</span></span>
|<span data-ttu-id="3d062-120">标头</span><span class="sxs-lookup"><span data-stu-id="3d062-120">Header</span></span>|<span data-ttu-id="3d062-121">值</span><span class="sxs-lookup"><span data-stu-id="3d062-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d062-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d062-122">Authorization</span></span>|<span data-ttu-id="3d062-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d062-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d062-124">接受</span><span class="sxs-lookup"><span data-stu-id="3d062-124">Accept</span></span>|<span data-ttu-id="3d062-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d062-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d062-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d062-126">Request body</span></span>
<span data-ttu-id="3d062-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d062-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="3d062-128">下表显示创建 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d062-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="3d062-129">属性</span><span class="sxs-lookup"><span data-stu-id="3d062-129">Property</span></span>|<span data-ttu-id="3d062-130">类型</span><span class="sxs-lookup"><span data-stu-id="3d062-130">Type</span></span>|<span data-ttu-id="3d062-131">说明</span><span class="sxs-lookup"><span data-stu-id="3d062-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d062-132">id</span><span class="sxs-lookup"><span data-stu-id="3d062-132">id</span></span>|<span data-ttu-id="3d062-133">String</span><span class="sxs-lookup"><span data-stu-id="3d062-133">String</span></span>|<span data-ttu-id="3d062-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3d062-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3d062-135">target</span><span class="sxs-lookup"><span data-stu-id="3d062-135">target</span></span>|[<span data-ttu-id="3d062-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3d062-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3d062-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="3d062-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="3d062-138">响应</span><span class="sxs-lookup"><span data-stu-id="3d062-138">Response</span></span>
<span data-ttu-id="3d062-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d062-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d062-140">示例</span><span class="sxs-lookup"><span data-stu-id="3d062-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d062-141">请求</span><span class="sxs-lookup"><span data-stu-id="3d062-141">Request</span></span>
<span data-ttu-id="3d062-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d062-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3d062-143">响应</span><span class="sxs-lookup"><span data-stu-id="3d062-143">Response</span></span>
<span data-ttu-id="3d062-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d062-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




