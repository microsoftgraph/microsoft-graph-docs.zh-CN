---
title: 创建 mobileAppProvisioningConfigGroupAssignment
description: 创建新的 mobileAppProvisioningConfigGroupAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbb0a1190eb24bf0a00510061e6c71f238f7c84f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164713"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="e3715-103">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="e3715-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="e3715-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3715-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3715-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3715-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3715-106">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3715-106">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3715-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e3715-107">Prerequisites</span></span>
<span data-ttu-id="e3715-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e3715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3715-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3715-110">Permission type</span></span>|<span data-ttu-id="e3715-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e3715-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3715-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3715-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3715-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3715-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3715-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3715-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3715-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3715-115">Not supported.</span></span>|
|<span data-ttu-id="e3715-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3715-116">Application</span></span>|<span data-ttu-id="e3715-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3715-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3715-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3715-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e3715-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3715-119">Request headers</span></span>
|<span data-ttu-id="e3715-120">标头</span><span class="sxs-lookup"><span data-stu-id="e3715-120">Header</span></span>|<span data-ttu-id="e3715-121">值</span><span class="sxs-lookup"><span data-stu-id="e3715-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3715-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3715-122">Authorization</span></span>|<span data-ttu-id="e3715-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e3715-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3715-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e3715-124">Accept</span></span>|<span data-ttu-id="e3715-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3715-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3715-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3715-126">Request body</span></span>
<span data-ttu-id="e3715-127">在请求正文中, 提供 mobileAppProvisioningConfigGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3715-127">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="e3715-128">下表显示创建 mobileAppProvisioningConfigGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e3715-128">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="e3715-129">属性</span><span class="sxs-lookup"><span data-stu-id="e3715-129">Property</span></span>|<span data-ttu-id="e3715-130">类型</span><span class="sxs-lookup"><span data-stu-id="e3715-130">Type</span></span>|<span data-ttu-id="e3715-131">说明</span><span class="sxs-lookup"><span data-stu-id="e3715-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3715-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="e3715-132">targetGroupId</span></span>|<span data-ttu-id="e3715-133">String</span><span class="sxs-lookup"><span data-stu-id="e3715-133">String</span></span>|<span data-ttu-id="e3715-134">要在其中定向应用程序设置配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="e3715-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="e3715-135">id</span><span class="sxs-lookup"><span data-stu-id="e3715-135">id</span></span>|<span data-ttu-id="e3715-136">String</span><span class="sxs-lookup"><span data-stu-id="e3715-136">String</span></span>|<span data-ttu-id="e3715-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e3715-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e3715-138">响应</span><span class="sxs-lookup"><span data-stu-id="e3715-138">Response</span></span>
<span data-ttu-id="e3715-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3715-139">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3715-140">示例</span><span class="sxs-lookup"><span data-stu-id="e3715-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3715-141">请求</span><span class="sxs-lookup"><span data-stu-id="e3715-141">Request</span></span>
<span data-ttu-id="e3715-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3715-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="e3715-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3715-143">Response</span></span>
<span data-ttu-id="e3715-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3715-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




