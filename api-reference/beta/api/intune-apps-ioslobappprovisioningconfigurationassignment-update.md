---
title: 更新 iosLobAppProvisioningConfigurationAssignment
description: 更新 iosLobAppProvisioningConfigurationAssignment 对象的属性。
ms.openlocfilehash: d58f10d47a27b89cd64d53cefcfb849fa5fd1ce9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047864"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="c62b0-103">更新 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c62b0-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="c62b0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c62b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c62b0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c62b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c62b0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c62b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c62b0-107">更新[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c62b0-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c62b0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c62b0-108">Prerequisites</span></span>
<span data-ttu-id="c62b0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c62b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c62b0-111">Permission type</span></span>|<span data-ttu-id="c62b0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c62b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c62b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c62b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c62b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c62b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c62b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c62b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c62b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c62b0-116">Not supported.</span></span>|
|<span data-ttu-id="c62b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c62b0-117">Application</span></span>|<span data-ttu-id="c62b0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c62b0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c62b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c62b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c62b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c62b0-120">Request headers</span></span>
|<span data-ttu-id="c62b0-121">标头</span><span class="sxs-lookup"><span data-stu-id="c62b0-121">Header</span></span>|<span data-ttu-id="c62b0-122">值</span><span class="sxs-lookup"><span data-stu-id="c62b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c62b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c62b0-123">Authorization</span></span>|<span data-ttu-id="c62b0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c62b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c62b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c62b0-125">Accept</span></span>|<span data-ttu-id="c62b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c62b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62b0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c62b0-127">Request body</span></span>
<span data-ttu-id="c62b0-128">在请求正文中，提供[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c62b0-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c62b0-129">下表显示时创建[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c62b0-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="c62b0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c62b0-130">Property</span></span>|<span data-ttu-id="c62b0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c62b0-131">Type</span></span>|<span data-ttu-id="c62b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c62b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c62b0-133">id</span><span class="sxs-lookup"><span data-stu-id="c62b0-133">id</span></span>|<span data-ttu-id="c62b0-134">String</span><span class="sxs-lookup"><span data-stu-id="c62b0-134">String</span></span>|<span data-ttu-id="c62b0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c62b0-135">Key of the entity.</span></span>|
|<span data-ttu-id="c62b0-136">target</span><span class="sxs-lookup"><span data-stu-id="c62b0-136">target</span></span>|[<span data-ttu-id="c62b0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c62b0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c62b0-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="c62b0-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="c62b0-139">响应</span><span class="sxs-lookup"><span data-stu-id="c62b0-139">Response</span></span>
<span data-ttu-id="c62b0-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c62b0-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62b0-141">示例</span><span class="sxs-lookup"><span data-stu-id="c62b0-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c62b0-142">请求</span><span class="sxs-lookup"><span data-stu-id="c62b0-142">Request</span></span>
<span data-ttu-id="c62b0-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c62b0-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c62b0-144">响应</span><span class="sxs-lookup"><span data-stu-id="c62b0-144">Response</span></span>
<span data-ttu-id="c62b0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c62b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





