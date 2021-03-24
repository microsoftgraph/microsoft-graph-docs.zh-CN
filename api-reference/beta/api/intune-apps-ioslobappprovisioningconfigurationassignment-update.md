---
title: 更新 iosLobAppProvisioningConfigurationAssignment
description: 更新 iosLobAppProvisioningConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f840150543ca6d4f5d4cfe46db0ade1d42e78eb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144219"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="47af3-103">更新 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="47af3-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="47af3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47af3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47af3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47af3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47af3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47af3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47af3-107">更新 [iosLobAppProvisioningConfigurationAssignment 对象](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="47af3-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47af3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="47af3-108">Prerequisites</span></span>
<span data-ttu-id="47af3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47af3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47af3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="47af3-111">Permission type</span></span>|<span data-ttu-id="47af3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47af3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47af3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47af3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47af3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47af3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47af3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47af3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47af3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="47af3-116">Not supported.</span></span>|
|<span data-ttu-id="47af3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="47af3-117">Application</span></span>|<span data-ttu-id="47af3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47af3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47af3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47af3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="47af3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="47af3-120">Request headers</span></span>
|<span data-ttu-id="47af3-121">标头</span><span class="sxs-lookup"><span data-stu-id="47af3-121">Header</span></span>|<span data-ttu-id="47af3-122">值</span><span class="sxs-lookup"><span data-stu-id="47af3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47af3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47af3-123">Authorization</span></span>|<span data-ttu-id="47af3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47af3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47af3-125">接受</span><span class="sxs-lookup"><span data-stu-id="47af3-125">Accept</span></span>|<span data-ttu-id="47af3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47af3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47af3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="47af3-127">Request body</span></span>
<span data-ttu-id="47af3-128">在请求正文中，提供 [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47af3-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="47af3-129">下表显示创建 [iosLobAppProvisioningConfigurationAssignment 时所需的属性](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="47af3-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="47af3-130">属性</span><span class="sxs-lookup"><span data-stu-id="47af3-130">Property</span></span>|<span data-ttu-id="47af3-131">类型</span><span class="sxs-lookup"><span data-stu-id="47af3-131">Type</span></span>|<span data-ttu-id="47af3-132">说明</span><span class="sxs-lookup"><span data-stu-id="47af3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47af3-133">id</span><span class="sxs-lookup"><span data-stu-id="47af3-133">id</span></span>|<span data-ttu-id="47af3-134">String</span><span class="sxs-lookup"><span data-stu-id="47af3-134">String</span></span>|<span data-ttu-id="47af3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47af3-135">Key of the entity.</span></span>|
|<span data-ttu-id="47af3-136">target</span><span class="sxs-lookup"><span data-stu-id="47af3-136">target</span></span>|[<span data-ttu-id="47af3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47af3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="47af3-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="47af3-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="47af3-139">响应</span><span class="sxs-lookup"><span data-stu-id="47af3-139">Response</span></span>
<span data-ttu-id="47af3-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47af3-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47af3-141">示例</span><span class="sxs-lookup"><span data-stu-id="47af3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="47af3-142">请求</span><span class="sxs-lookup"><span data-stu-id="47af3-142">Request</span></span>
<span data-ttu-id="47af3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47af3-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47af3-144">响应</span><span class="sxs-lookup"><span data-stu-id="47af3-144">Response</span></span>
<span data-ttu-id="47af3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47af3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




