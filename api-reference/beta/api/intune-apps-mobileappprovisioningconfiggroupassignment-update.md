---
title: 更新 mobileAppProvisioningConfigGroupAssignment
description: 更新 mobileAppProvisioningConfigGroupAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: c113c16234cb51146aa2e627d39405f740d6aab3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359141"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="89c4c-103">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="89c4c-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="89c4c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89c4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89c4c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89c4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89c4c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89c4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89c4c-107">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89c4c-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89c4c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89c4c-108">Prerequisites</span></span>
<span data-ttu-id="89c4c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="89c4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89c4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89c4c-111">Permission type</span></span>|<span data-ttu-id="89c4c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89c4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89c4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89c4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89c4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89c4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89c4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89c4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89c4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c4c-116">Not supported.</span></span>|
|<span data-ttu-id="89c4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89c4c-117">Application</span></span>|<span data-ttu-id="89c4c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c4c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89c4c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89c4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="89c4c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89c4c-120">Request headers</span></span>
|<span data-ttu-id="89c4c-121">标头</span><span class="sxs-lookup"><span data-stu-id="89c4c-121">Header</span></span>|<span data-ttu-id="89c4c-122">值</span><span class="sxs-lookup"><span data-stu-id="89c4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89c4c-123">授权</span><span class="sxs-lookup"><span data-stu-id="89c4c-123">Authorization</span></span>|<span data-ttu-id="89c4c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89c4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89c4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89c4c-125">Accept</span></span>|<span data-ttu-id="89c4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89c4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89c4c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89c4c-127">Request body</span></span>
<span data-ttu-id="89c4c-128">在请求正文中，提供[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89c4c-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="89c4c-129">下表显示时创建[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89c4c-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="89c4c-130">属性</span><span class="sxs-lookup"><span data-stu-id="89c4c-130">Property</span></span>|<span data-ttu-id="89c4c-131">类型</span><span class="sxs-lookup"><span data-stu-id="89c4c-131">Type</span></span>|<span data-ttu-id="89c4c-132">说明</span><span class="sxs-lookup"><span data-stu-id="89c4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c4c-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="89c4c-133">targetGroupId</span></span>|<span data-ttu-id="89c4c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="89c4c-134">String</span></span>|<span data-ttu-id="89c4c-135">AAD 组顺序为目标应用程序设置配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="89c4c-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="89c4c-136">id</span><span class="sxs-lookup"><span data-stu-id="89c4c-136">id</span></span>|<span data-ttu-id="89c4c-137">String</span><span class="sxs-lookup"><span data-stu-id="89c4c-137">String</span></span>|<span data-ttu-id="89c4c-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89c4c-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="89c4c-139">响应</span><span class="sxs-lookup"><span data-stu-id="89c4c-139">Response</span></span>
<span data-ttu-id="89c4c-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="89c4c-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89c4c-141">示例</span><span class="sxs-lookup"><span data-stu-id="89c4c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="89c4c-142">请求</span><span class="sxs-lookup"><span data-stu-id="89c4c-142">Request</span></span>
<span data-ttu-id="89c4c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89c4c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="89c4c-144">响应</span><span class="sxs-lookup"><span data-stu-id="89c4c-144">Response</span></span>
<span data-ttu-id="89c4c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89c4c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





