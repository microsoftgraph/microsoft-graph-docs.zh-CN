---
title: 更新 managedDeviceMobileAppConfigurationAssignment
description: 更新 managedDeviceMobileAppConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10b7e1d9a07d367d74f2ce4232fcf02d1179156a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140166"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="49469-103">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49469-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="49469-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49469-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49469-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49469-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49469-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49469-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49469-107">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49469-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49469-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="49469-108">Prerequisites</span></span>
<span data-ttu-id="49469-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49469-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49469-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="49469-111">Permission type</span></span>|<span data-ttu-id="49469-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49469-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49469-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49469-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49469-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49469-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49469-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49469-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49469-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49469-116">Not supported.</span></span>|
|<span data-ttu-id="49469-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="49469-117">Application</span></span>|<span data-ttu-id="49469-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49469-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49469-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49469-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="49469-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49469-120">Request headers</span></span>
|<span data-ttu-id="49469-121">标头</span><span class="sxs-lookup"><span data-stu-id="49469-121">Header</span></span>|<span data-ttu-id="49469-122">值</span><span class="sxs-lookup"><span data-stu-id="49469-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49469-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49469-123">Authorization</span></span>|<span data-ttu-id="49469-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49469-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49469-125">接受</span><span class="sxs-lookup"><span data-stu-id="49469-125">Accept</span></span>|<span data-ttu-id="49469-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49469-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49469-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="49469-127">Request body</span></span>
<span data-ttu-id="49469-128">在请求正文中，提供 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49469-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="49469-129">下表显示创建 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="49469-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="49469-130">属性</span><span class="sxs-lookup"><span data-stu-id="49469-130">Property</span></span>|<span data-ttu-id="49469-131">类型</span><span class="sxs-lookup"><span data-stu-id="49469-131">Type</span></span>|<span data-ttu-id="49469-132">说明</span><span class="sxs-lookup"><span data-stu-id="49469-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49469-133">id</span><span class="sxs-lookup"><span data-stu-id="49469-133">id</span></span>|<span data-ttu-id="49469-134">String</span><span class="sxs-lookup"><span data-stu-id="49469-134">String</span></span>|<span data-ttu-id="49469-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="49469-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="49469-136">target</span><span class="sxs-lookup"><span data-stu-id="49469-136">target</span></span>|[<span data-ttu-id="49469-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="49469-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="49469-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="49469-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="49469-139">响应</span><span class="sxs-lookup"><span data-stu-id="49469-139">Response</span></span>
<span data-ttu-id="49469-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49469-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49469-141">示例</span><span class="sxs-lookup"><span data-stu-id="49469-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="49469-142">请求</span><span class="sxs-lookup"><span data-stu-id="49469-142">Request</span></span>
<span data-ttu-id="49469-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49469-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="49469-144">响应</span><span class="sxs-lookup"><span data-stu-id="49469-144">Response</span></span>
<span data-ttu-id="49469-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49469-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




