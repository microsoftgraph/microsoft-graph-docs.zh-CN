---
title: 创建 managedDeviceMobileAppConfigurationAssignment
description: 创建新的 managedDeviceMobileAppConfigurationAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f8fb7741aeabbf941142143f03c16217dfb58b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014072"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="d2cb7-103">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d2cb7-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="d2cb7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2cb7-105">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2cb7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2cb7-106">Prerequisites</span></span>
<span data-ttu-id="d2cb7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2cb7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2cb7-109">Permission type</span></span>|<span data-ttu-id="d2cb7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2cb7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2cb7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2cb7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2cb7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2cb7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d2cb7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2cb7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2cb7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-114">Not supported.</span></span>|
|<span data-ttu-id="d2cb7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2cb7-115">Application</span></span>|<span data-ttu-id="d2cb7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2cb7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2cb7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d2cb7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2cb7-118">Request headers</span></span>
|<span data-ttu-id="d2cb7-119">标头</span><span class="sxs-lookup"><span data-stu-id="d2cb7-119">Header</span></span>|<span data-ttu-id="d2cb7-120">值</span><span class="sxs-lookup"><span data-stu-id="d2cb7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2cb7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2cb7-121">Authorization</span></span>|<span data-ttu-id="d2cb7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2cb7-123">接受</span><span class="sxs-lookup"><span data-stu-id="d2cb7-123">Accept</span></span>|<span data-ttu-id="d2cb7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d2cb7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2cb7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2cb7-125">Request body</span></span>
<span data-ttu-id="d2cb7-126">在请求正文中，提供 managedDeviceMobileAppConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="d2cb7-127">下表显示创建 managedDeviceMobileAppConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="d2cb7-128">属性</span><span class="sxs-lookup"><span data-stu-id="d2cb7-128">Property</span></span>|<span data-ttu-id="d2cb7-129">类型</span><span class="sxs-lookup"><span data-stu-id="d2cb7-129">Type</span></span>|<span data-ttu-id="d2cb7-130">说明</span><span class="sxs-lookup"><span data-stu-id="d2cb7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2cb7-131">id</span><span class="sxs-lookup"><span data-stu-id="d2cb7-131">id</span></span>|<span data-ttu-id="d2cb7-132">String</span><span class="sxs-lookup"><span data-stu-id="d2cb7-132">String</span></span>|<span data-ttu-id="d2cb7-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d2cb7-134">target</span><span class="sxs-lookup"><span data-stu-id="d2cb7-134">target</span></span>|[<span data-ttu-id="d2cb7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2cb7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2cb7-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d2cb7-137">响应</span><span class="sxs-lookup"><span data-stu-id="d2cb7-137">Response</span></span>
<span data-ttu-id="d2cb7-138">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2cb7-139">示例</span><span class="sxs-lookup"><span data-stu-id="d2cb7-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2cb7-140">请求</span><span class="sxs-lookup"><span data-stu-id="d2cb7-140">Request</span></span>
<span data-ttu-id="d2cb7-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d2cb7-142">响应</span><span class="sxs-lookup"><span data-stu-id="d2cb7-142">Response</span></span>
<span data-ttu-id="d2cb7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2cb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



