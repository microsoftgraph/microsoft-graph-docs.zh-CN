---
title: 创建 managedDeviceMobileAppConfigurationAssignment
description: 创建新的 managedDeviceMobileAppConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9bd6d4ab40942e588be370724b1d0cc8f80a529
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793365"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="1625f-103">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1625f-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="1625f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1625f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1625f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1625f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1625f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1625f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1625f-107">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1625f-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1625f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1625f-108">Prerequisites</span></span>
<span data-ttu-id="1625f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1625f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1625f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1625f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1625f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1625f-111">Permission type</span></span>|<span data-ttu-id="1625f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1625f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1625f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1625f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1625f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1625f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1625f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1625f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1625f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1625f-116">Not supported.</span></span>|
|<span data-ttu-id="1625f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1625f-117">Application</span></span>|<span data-ttu-id="1625f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1625f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1625f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1625f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1625f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1625f-120">Request headers</span></span>
|<span data-ttu-id="1625f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1625f-121">Header</span></span>|<span data-ttu-id="1625f-122">值</span><span class="sxs-lookup"><span data-stu-id="1625f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1625f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1625f-123">Authorization</span></span>|<span data-ttu-id="1625f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1625f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1625f-125">接受</span><span class="sxs-lookup"><span data-stu-id="1625f-125">Accept</span></span>|<span data-ttu-id="1625f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1625f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1625f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1625f-127">Request body</span></span>
<span data-ttu-id="1625f-128">在请求正文中，提供 managedDeviceMobileAppConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1625f-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="1625f-129">下表显示创建 managedDeviceMobileAppConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1625f-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="1625f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1625f-130">Property</span></span>|<span data-ttu-id="1625f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1625f-131">Type</span></span>|<span data-ttu-id="1625f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1625f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1625f-133">id</span><span class="sxs-lookup"><span data-stu-id="1625f-133">id</span></span>|<span data-ttu-id="1625f-134">String</span><span class="sxs-lookup"><span data-stu-id="1625f-134">String</span></span>|<span data-ttu-id="1625f-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1625f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1625f-136">target</span><span class="sxs-lookup"><span data-stu-id="1625f-136">target</span></span>|[<span data-ttu-id="1625f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1625f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1625f-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1625f-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1625f-139">响应</span><span class="sxs-lookup"><span data-stu-id="1625f-139">Response</span></span>
<span data-ttu-id="1625f-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1625f-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1625f-141">示例</span><span class="sxs-lookup"><span data-stu-id="1625f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1625f-142">请求</span><span class="sxs-lookup"><span data-stu-id="1625f-142">Request</span></span>
<span data-ttu-id="1625f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1625f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="1625f-144">响应</span><span class="sxs-lookup"><span data-stu-id="1625f-144">Response</span></span>
<span data-ttu-id="1625f-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1625f-145">Here is an example of the response.</span></span> <span data-ttu-id="1625f-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1625f-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1625f-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1625f-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



