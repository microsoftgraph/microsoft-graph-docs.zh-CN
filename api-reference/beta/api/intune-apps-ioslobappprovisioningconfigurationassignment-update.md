---
title: 更新 iosLobAppProvisioningConfigurationAssignment
description: 更新 iosLobAppProvisioningConfigurationAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f80f07feb9027054b5b88f1fa4fdcf868e0b3f84
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397615"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="1bacf-103">更新 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1bacf-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="1bacf-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1bacf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1bacf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1bacf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bacf-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bacf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bacf-107">更新[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1bacf-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bacf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bacf-108">Prerequisites</span></span>
<span data-ttu-id="1bacf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1bacf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1bacf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bacf-111">Permission type</span></span>|<span data-ttu-id="1bacf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bacf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bacf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bacf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bacf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bacf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bacf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bacf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bacf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bacf-116">Not supported.</span></span>|
|<span data-ttu-id="1bacf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bacf-117">Application</span></span>|<span data-ttu-id="1bacf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bacf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bacf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bacf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1bacf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bacf-120">Request headers</span></span>
|<span data-ttu-id="1bacf-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bacf-121">Header</span></span>|<span data-ttu-id="1bacf-122">值</span><span class="sxs-lookup"><span data-stu-id="1bacf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bacf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bacf-123">Authorization</span></span>|<span data-ttu-id="1bacf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bacf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bacf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bacf-125">Accept</span></span>|<span data-ttu-id="1bacf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bacf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bacf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bacf-127">Request body</span></span>
<span data-ttu-id="1bacf-128">在请求正文中，提供[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bacf-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1bacf-129">下表显示时创建[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1bacf-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="1bacf-130">属性</span><span class="sxs-lookup"><span data-stu-id="1bacf-130">Property</span></span>|<span data-ttu-id="1bacf-131">类型</span><span class="sxs-lookup"><span data-stu-id="1bacf-131">Type</span></span>|<span data-ttu-id="1bacf-132">说明</span><span class="sxs-lookup"><span data-stu-id="1bacf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bacf-133">id</span><span class="sxs-lookup"><span data-stu-id="1bacf-133">id</span></span>|<span data-ttu-id="1bacf-134">String</span><span class="sxs-lookup"><span data-stu-id="1bacf-134">String</span></span>|<span data-ttu-id="1bacf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1bacf-135">Key of the entity.</span></span>|
|<span data-ttu-id="1bacf-136">target</span><span class="sxs-lookup"><span data-stu-id="1bacf-136">target</span></span>|[<span data-ttu-id="1bacf-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1bacf-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1bacf-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="1bacf-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="1bacf-139">响应</span><span class="sxs-lookup"><span data-stu-id="1bacf-139">Response</span></span>
<span data-ttu-id="1bacf-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1bacf-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bacf-141">示例</span><span class="sxs-lookup"><span data-stu-id="1bacf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bacf-142">请求</span><span class="sxs-lookup"><span data-stu-id="1bacf-142">Request</span></span>
<span data-ttu-id="1bacf-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bacf-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1bacf-144">响应</span><span class="sxs-lookup"><span data-stu-id="1bacf-144">Response</span></span>
<span data-ttu-id="1bacf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bacf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




