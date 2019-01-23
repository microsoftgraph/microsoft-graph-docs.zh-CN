---
title: 更新 mobileAppProvisioningConfigGroupAssignment
description: 更新 mobileAppProvisioningConfigGroupAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b897e377ef221cc14034dbd48958a2092dbf956
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413428"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="aac31-103">更新 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aac31-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="aac31-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="aac31-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aac31-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aac31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aac31-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aac31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac31-107">更新[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aac31-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac31-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aac31-108">Prerequisites</span></span>
<span data-ttu-id="aac31-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aac31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aac31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aac31-111">Permission type</span></span>|<span data-ttu-id="aac31-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aac31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aac31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aac31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aac31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aac31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aac31-116">Not supported.</span></span>|
|<span data-ttu-id="aac31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aac31-117">Application</span></span>|<span data-ttu-id="aac31-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aac31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aac31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aac31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aac31-120">Request headers</span></span>
|<span data-ttu-id="aac31-121">标头</span><span class="sxs-lookup"><span data-stu-id="aac31-121">Header</span></span>|<span data-ttu-id="aac31-122">值</span><span class="sxs-lookup"><span data-stu-id="aac31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac31-123">Authorization</span></span>|<span data-ttu-id="aac31-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aac31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aac31-125">Accept</span></span>|<span data-ttu-id="aac31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aac31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac31-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aac31-127">Request body</span></span>
<span data-ttu-id="aac31-128">在请求正文中，提供[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aac31-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="aac31-129">下表显示时创建[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aac31-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="aac31-130">属性</span><span class="sxs-lookup"><span data-stu-id="aac31-130">Property</span></span>|<span data-ttu-id="aac31-131">类型</span><span class="sxs-lookup"><span data-stu-id="aac31-131">Type</span></span>|<span data-ttu-id="aac31-132">说明</span><span class="sxs-lookup"><span data-stu-id="aac31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac31-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="aac31-133">targetGroupId</span></span>|<span data-ttu-id="aac31-134">String</span><span class="sxs-lookup"><span data-stu-id="aac31-134">String</span></span>|<span data-ttu-id="aac31-135">AAD 组顺序为目标应用程序设置配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="aac31-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="aac31-136">id</span><span class="sxs-lookup"><span data-stu-id="aac31-136">id</span></span>|<span data-ttu-id="aac31-137">String</span><span class="sxs-lookup"><span data-stu-id="aac31-137">String</span></span>|<span data-ttu-id="aac31-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aac31-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="aac31-139">响应</span><span class="sxs-lookup"><span data-stu-id="aac31-139">Response</span></span>
<span data-ttu-id="aac31-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aac31-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac31-141">示例</span><span class="sxs-lookup"><span data-stu-id="aac31-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac31-142">请求</span><span class="sxs-lookup"><span data-stu-id="aac31-142">Request</span></span>
<span data-ttu-id="aac31-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aac31-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="aac31-144">响应</span><span class="sxs-lookup"><span data-stu-id="aac31-144">Response</span></span>
<span data-ttu-id="aac31-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aac31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




