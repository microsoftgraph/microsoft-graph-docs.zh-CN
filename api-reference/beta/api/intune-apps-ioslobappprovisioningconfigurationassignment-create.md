---
title: 创建 iosLobAppProvisioningConfigurationAssignment
description: 创建新的 iosLobAppProvisioningConfigurationAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: daf8a934119c57ce5b797fffbf699e51b5e341c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951797"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="36507-103">创建 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="36507-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="36507-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36507-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36507-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36507-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36507-106">创建新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36507-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36507-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="36507-107">Prerequisites</span></span>
<span data-ttu-id="36507-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36507-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36507-110">Permission type</span></span>|<span data-ttu-id="36507-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36507-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36507-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36507-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36507-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36507-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36507-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36507-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36507-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36507-115">Not supported.</span></span>|
|<span data-ttu-id="36507-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36507-116">Application</span></span>|<span data-ttu-id="36507-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="36507-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36507-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36507-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="36507-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="36507-119">Request headers</span></span>
|<span data-ttu-id="36507-120">标头</span><span class="sxs-lookup"><span data-stu-id="36507-120">Header</span></span>|<span data-ttu-id="36507-121">值</span><span class="sxs-lookup"><span data-stu-id="36507-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36507-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36507-122">Authorization</span></span>|<span data-ttu-id="36507-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36507-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36507-124">接受</span><span class="sxs-lookup"><span data-stu-id="36507-124">Accept</span></span>|<span data-ttu-id="36507-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36507-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36507-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36507-126">Request body</span></span>
<span data-ttu-id="36507-127">在请求正文中, 提供 iosLobAppProvisioningConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36507-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="36507-128">下表显示创建 iosLobAppProvisioningConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36507-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="36507-129">属性</span><span class="sxs-lookup"><span data-stu-id="36507-129">Property</span></span>|<span data-ttu-id="36507-130">类型</span><span class="sxs-lookup"><span data-stu-id="36507-130">Type</span></span>|<span data-ttu-id="36507-131">说明</span><span class="sxs-lookup"><span data-stu-id="36507-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36507-132">id</span><span class="sxs-lookup"><span data-stu-id="36507-132">id</span></span>|<span data-ttu-id="36507-133">String</span><span class="sxs-lookup"><span data-stu-id="36507-133">String</span></span>|<span data-ttu-id="36507-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="36507-134">Key of the entity.</span></span>|
|<span data-ttu-id="36507-135">target</span><span class="sxs-lookup"><span data-stu-id="36507-135">target</span></span>|[<span data-ttu-id="36507-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="36507-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="36507-137">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="36507-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="36507-138">响应</span><span class="sxs-lookup"><span data-stu-id="36507-138">Response</span></span>
<span data-ttu-id="36507-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36507-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36507-140">示例</span><span class="sxs-lookup"><span data-stu-id="36507-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="36507-141">请求</span><span class="sxs-lookup"><span data-stu-id="36507-141">Request</span></span>
<span data-ttu-id="36507-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36507-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="36507-143">响应</span><span class="sxs-lookup"><span data-stu-id="36507-143">Response</span></span>
<span data-ttu-id="36507-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36507-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





