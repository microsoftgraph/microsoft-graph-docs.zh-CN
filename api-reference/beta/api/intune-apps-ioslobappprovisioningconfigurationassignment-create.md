---
title: 创建 iosLobAppProvisioningConfigurationAssignment
description: 创建新的 iosLobAppProvisioningConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c478bb6c00408f353c63bedc10a5774b1ff6e9c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144240"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="782b6-103">创建 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="782b6-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="782b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="782b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="782b6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="782b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="782b6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="782b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="782b6-107">创建新的 [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="782b6-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="782b6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="782b6-108">Prerequisites</span></span>
<span data-ttu-id="782b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="782b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="782b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="782b6-111">Permission type</span></span>|<span data-ttu-id="782b6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="782b6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="782b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="782b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="782b6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="782b6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="782b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="782b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="782b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="782b6-116">Not supported.</span></span>|
|<span data-ttu-id="782b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="782b6-117">Application</span></span>|<span data-ttu-id="782b6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="782b6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="782b6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="782b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="782b6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="782b6-120">Request headers</span></span>
|<span data-ttu-id="782b6-121">标头</span><span class="sxs-lookup"><span data-stu-id="782b6-121">Header</span></span>|<span data-ttu-id="782b6-122">值</span><span class="sxs-lookup"><span data-stu-id="782b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="782b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="782b6-123">Authorization</span></span>|<span data-ttu-id="782b6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="782b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="782b6-125">接受</span><span class="sxs-lookup"><span data-stu-id="782b6-125">Accept</span></span>|<span data-ttu-id="782b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="782b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="782b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="782b6-127">Request body</span></span>
<span data-ttu-id="782b6-128">在请求正文中，提供 iosLobAppProvisioningConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="782b6-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="782b6-129">下表显示创建 iosLobAppProvisioningConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="782b6-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="782b6-130">属性</span><span class="sxs-lookup"><span data-stu-id="782b6-130">Property</span></span>|<span data-ttu-id="782b6-131">类型</span><span class="sxs-lookup"><span data-stu-id="782b6-131">Type</span></span>|<span data-ttu-id="782b6-132">说明</span><span class="sxs-lookup"><span data-stu-id="782b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="782b6-133">id</span><span class="sxs-lookup"><span data-stu-id="782b6-133">id</span></span>|<span data-ttu-id="782b6-134">String</span><span class="sxs-lookup"><span data-stu-id="782b6-134">String</span></span>|<span data-ttu-id="782b6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="782b6-135">Key of the entity.</span></span>|
|<span data-ttu-id="782b6-136">target</span><span class="sxs-lookup"><span data-stu-id="782b6-136">target</span></span>|[<span data-ttu-id="782b6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="782b6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="782b6-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="782b6-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="782b6-139">响应</span><span class="sxs-lookup"><span data-stu-id="782b6-139">Response</span></span>
<span data-ttu-id="782b6-140">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="782b6-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="782b6-141">示例</span><span class="sxs-lookup"><span data-stu-id="782b6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="782b6-142">请求</span><span class="sxs-lookup"><span data-stu-id="782b6-142">Request</span></span>
<span data-ttu-id="782b6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="782b6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="782b6-144">响应</span><span class="sxs-lookup"><span data-stu-id="782b6-144">Response</span></span>
<span data-ttu-id="782b6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="782b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




