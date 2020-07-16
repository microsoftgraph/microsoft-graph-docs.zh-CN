---
title: 更新 iosLobAppProvisioningConfigurationAssignment
description: 更新 iosLobAppProvisioningConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 356c4ad3b8d2530ce083c77ce0c88bc5ac51c86e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793379"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="1401f-103">更新 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1401f-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="1401f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1401f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1401f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1401f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1401f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1401f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1401f-107">更新[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1401f-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1401f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1401f-108">Prerequisites</span></span>
<span data-ttu-id="1401f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1401f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1401f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1401f-111">Permission type</span></span>|<span data-ttu-id="1401f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1401f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1401f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1401f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1401f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1401f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1401f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1401f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1401f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1401f-116">Not supported.</span></span>|
|<span data-ttu-id="1401f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1401f-117">Application</span></span>|<span data-ttu-id="1401f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1401f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1401f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1401f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1401f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1401f-120">Request headers</span></span>
|<span data-ttu-id="1401f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1401f-121">Header</span></span>|<span data-ttu-id="1401f-122">值</span><span class="sxs-lookup"><span data-stu-id="1401f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1401f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1401f-123">Authorization</span></span>|<span data-ttu-id="1401f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1401f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1401f-125">接受</span><span class="sxs-lookup"><span data-stu-id="1401f-125">Accept</span></span>|<span data-ttu-id="1401f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1401f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1401f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1401f-127">Request body</span></span>
<span data-ttu-id="1401f-128">在请求正文中，提供[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1401f-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1401f-129">下表显示创建[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1401f-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="1401f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1401f-130">Property</span></span>|<span data-ttu-id="1401f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1401f-131">Type</span></span>|<span data-ttu-id="1401f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1401f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1401f-133">id</span><span class="sxs-lookup"><span data-stu-id="1401f-133">id</span></span>|<span data-ttu-id="1401f-134">String</span><span class="sxs-lookup"><span data-stu-id="1401f-134">String</span></span>|<span data-ttu-id="1401f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1401f-135">Key of the entity.</span></span>|
|<span data-ttu-id="1401f-136">target</span><span class="sxs-lookup"><span data-stu-id="1401f-136">target</span></span>|[<span data-ttu-id="1401f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1401f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1401f-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="1401f-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="1401f-139">响应</span><span class="sxs-lookup"><span data-stu-id="1401f-139">Response</span></span>
<span data-ttu-id="1401f-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1401f-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1401f-141">示例</span><span class="sxs-lookup"><span data-stu-id="1401f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1401f-142">请求</span><span class="sxs-lookup"><span data-stu-id="1401f-142">Request</span></span>
<span data-ttu-id="1401f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1401f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 351

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="1401f-144">响应</span><span class="sxs-lookup"><span data-stu-id="1401f-144">Response</span></span>
<span data-ttu-id="1401f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1401f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



