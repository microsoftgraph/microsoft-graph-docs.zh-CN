---
title: 创建 mobileAppProvisioningConfigGroupAssignment
description: 创建新的 mobileAppProvisioningConfigGroupAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d08b5001f5c9ef8abc42085fb9840f726ede4446
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925488"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="3c9e9-103">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3c9e9-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="3c9e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c9e9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c9e9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c9e9-107">创建新的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c9e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c9e9-108">Prerequisites</span></span>
<span data-ttu-id="3c9e9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3c9e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c9e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c9e9-111">Permission type</span></span>|<span data-ttu-id="3c9e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c9e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c9e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c9e9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9e9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c9e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c9e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c9e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-116">Not supported.</span></span>|
|<span data-ttu-id="3c9e9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c9e9-117">Application</span></span>|<span data-ttu-id="3c9e9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c9e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c9e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="3c9e9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c9e9-120">Request headers</span></span>
|<span data-ttu-id="3c9e9-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c9e9-121">Header</span></span>|<span data-ttu-id="3c9e9-122">值</span><span class="sxs-lookup"><span data-stu-id="3c9e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c9e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c9e9-123">Authorization</span></span>|<span data-ttu-id="3c9e9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c9e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c9e9-125">Accept</span></span>|<span data-ttu-id="3c9e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c9e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c9e9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c9e9-127">Request body</span></span>
<span data-ttu-id="3c9e9-128">在请求正文中，提供 mobileAppProvisioningConfigGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="3c9e9-129">下表显示时创建 mobileAppProvisioningConfigGroupAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="3c9e9-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c9e9-130">Property</span></span>|<span data-ttu-id="3c9e9-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c9e9-131">Type</span></span>|<span data-ttu-id="3c9e9-132">Description</span><span class="sxs-lookup"><span data-stu-id="3c9e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c9e9-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3c9e9-133">targetGroupId</span></span>|<span data-ttu-id="3c9e9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3c9e9-134">String</span></span>|<span data-ttu-id="3c9e9-135">AAD 组顺序为目标应用程序设置配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="3c9e9-136">id</span><span class="sxs-lookup"><span data-stu-id="3c9e9-136">id</span></span>|<span data-ttu-id="3c9e9-137">String</span><span class="sxs-lookup"><span data-stu-id="3c9e9-137">String</span></span>|<span data-ttu-id="3c9e9-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3c9e9-139">响应</span><span class="sxs-lookup"><span data-stu-id="3c9e9-139">Response</span></span>
<span data-ttu-id="3c9e9-140">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9e9-141">示例</span><span class="sxs-lookup"><span data-stu-id="3c9e9-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c9e9-142">请求</span><span class="sxs-lookup"><span data-stu-id="3c9e9-142">Request</span></span>
<span data-ttu-id="3c9e9-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="3c9e9-144">响应</span><span class="sxs-lookup"><span data-stu-id="3c9e9-144">Response</span></span>
<span data-ttu-id="3c9e9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c9e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





