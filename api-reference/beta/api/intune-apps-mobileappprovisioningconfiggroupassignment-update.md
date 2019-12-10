---
title: 更新 mobileAppProvisioningConfigGroupAssignment
description: 更新 mobileAppProvisioningConfigGroupAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d3917e60e7e895921c2eed735bf718461b44abb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934880"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="eab6b-103">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="eab6b-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="eab6b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eab6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eab6b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eab6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eab6b-106">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eab6b-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eab6b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eab6b-107">Prerequisites</span></span>
<span data-ttu-id="eab6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eab6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab6b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eab6b-110">Permission type</span></span>|<span data-ttu-id="eab6b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eab6b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eab6b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eab6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eab6b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab6b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eab6b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eab6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eab6b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eab6b-115">Not supported.</span></span>|
|<span data-ttu-id="eab6b-116">Application</span><span class="sxs-lookup"><span data-stu-id="eab6b-116">Application</span></span>|<span data-ttu-id="eab6b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab6b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eab6b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eab6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eab6b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eab6b-119">Request headers</span></span>
|<span data-ttu-id="eab6b-120">标头</span><span class="sxs-lookup"><span data-stu-id="eab6b-120">Header</span></span>|<span data-ttu-id="eab6b-121">值</span><span class="sxs-lookup"><span data-stu-id="eab6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eab6b-122">授权</span><span class="sxs-lookup"><span data-stu-id="eab6b-122">Authorization</span></span>|<span data-ttu-id="eab6b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eab6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eab6b-124">接受</span><span class="sxs-lookup"><span data-stu-id="eab6b-124">Accept</span></span>|<span data-ttu-id="eab6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eab6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eab6b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eab6b-126">Request body</span></span>
<span data-ttu-id="eab6b-127">在请求正文中，提供[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eab6b-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="eab6b-128">下表显示创建[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eab6b-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="eab6b-129">属性</span><span class="sxs-lookup"><span data-stu-id="eab6b-129">Property</span></span>|<span data-ttu-id="eab6b-130">类型</span><span class="sxs-lookup"><span data-stu-id="eab6b-130">Type</span></span>|<span data-ttu-id="eab6b-131">说明</span><span class="sxs-lookup"><span data-stu-id="eab6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eab6b-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="eab6b-132">targetGroupId</span></span>|<span data-ttu-id="eab6b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="eab6b-133">String</span></span>|<span data-ttu-id="eab6b-134">要在其中定向应用程序设置配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="eab6b-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="eab6b-135">id</span><span class="sxs-lookup"><span data-stu-id="eab6b-135">id</span></span>|<span data-ttu-id="eab6b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="eab6b-136">String</span></span>|<span data-ttu-id="eab6b-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eab6b-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="eab6b-138">响应</span><span class="sxs-lookup"><span data-stu-id="eab6b-138">Response</span></span>
<span data-ttu-id="eab6b-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eab6b-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab6b-140">示例</span><span class="sxs-lookup"><span data-stu-id="eab6b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="eab6b-141">请求</span><span class="sxs-lookup"><span data-stu-id="eab6b-141">Request</span></span>
<span data-ttu-id="eab6b-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eab6b-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="eab6b-143">响应</span><span class="sxs-lookup"><span data-stu-id="eab6b-143">Response</span></span>
<span data-ttu-id="eab6b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eab6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





