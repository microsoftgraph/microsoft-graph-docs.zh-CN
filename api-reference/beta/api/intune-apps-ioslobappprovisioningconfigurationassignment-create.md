---
title: 创建 iosLobAppProvisioningConfigurationAssignment
description: 创建新的 iosLobAppProvisioningConfigurationAssignment 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d1ba6130224718c7c28c02f0866ae01144f4c66
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421527"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="0abe7-103">创建 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0abe7-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="0abe7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0abe7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0abe7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0abe7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0abe7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0abe7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0abe7-107">创建新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0abe7-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0abe7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0abe7-108">Prerequisites</span></span>
<span data-ttu-id="0abe7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0abe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0abe7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0abe7-111">Permission type</span></span>|<span data-ttu-id="0abe7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0abe7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0abe7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0abe7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0abe7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0abe7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0abe7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0abe7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0abe7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0abe7-116">Not supported.</span></span>|
|<span data-ttu-id="0abe7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0abe7-117">Application</span></span>|<span data-ttu-id="0abe7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0abe7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0abe7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0abe7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0abe7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0abe7-120">Request headers</span></span>
|<span data-ttu-id="0abe7-121">标头</span><span class="sxs-lookup"><span data-stu-id="0abe7-121">Header</span></span>|<span data-ttu-id="0abe7-122">值</span><span class="sxs-lookup"><span data-stu-id="0abe7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0abe7-123">授权</span><span class="sxs-lookup"><span data-stu-id="0abe7-123">Authorization</span></span>|<span data-ttu-id="0abe7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0abe7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0abe7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0abe7-125">Accept</span></span>|<span data-ttu-id="0abe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0abe7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0abe7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0abe7-127">Request body</span></span>
<span data-ttu-id="0abe7-128">在请求正文中，提供 iosLobAppProvisioningConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0abe7-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="0abe7-129">下表显示时创建 iosLobAppProvisioningConfigurationAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0abe7-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="0abe7-130">属性</span><span class="sxs-lookup"><span data-stu-id="0abe7-130">Property</span></span>|<span data-ttu-id="0abe7-131">类型</span><span class="sxs-lookup"><span data-stu-id="0abe7-131">Type</span></span>|<span data-ttu-id="0abe7-132">说明</span><span class="sxs-lookup"><span data-stu-id="0abe7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0abe7-133">id</span><span class="sxs-lookup"><span data-stu-id="0abe7-133">id</span></span>|<span data-ttu-id="0abe7-134">String</span><span class="sxs-lookup"><span data-stu-id="0abe7-134">String</span></span>|<span data-ttu-id="0abe7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0abe7-135">Key of the entity.</span></span>|
|<span data-ttu-id="0abe7-136">target</span><span class="sxs-lookup"><span data-stu-id="0abe7-136">target</span></span>|[<span data-ttu-id="0abe7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0abe7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0abe7-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="0abe7-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0abe7-139">响应</span><span class="sxs-lookup"><span data-stu-id="0abe7-139">Response</span></span>
<span data-ttu-id="0abe7-140">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0abe7-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0abe7-141">示例</span><span class="sxs-lookup"><span data-stu-id="0abe7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0abe7-142">请求</span><span class="sxs-lookup"><span data-stu-id="0abe7-142">Request</span></span>
<span data-ttu-id="0abe7-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0abe7-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0abe7-144">响应</span><span class="sxs-lookup"><span data-stu-id="0abe7-144">Response</span></span>
<span data-ttu-id="0abe7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0abe7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




