---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6f28f61499e5e3e9f0b664692d3f7d706c28bad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458453"
---
# <a name="assign-action"></a><span data-ttu-id="2c417-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="2c417-103">assign action</span></span>

<span data-ttu-id="2c417-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2c417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c417-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c417-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c417-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c417-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2c417-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c417-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c417-108">Prerequisites</span></span>
<span data-ttu-id="2c417-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c417-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c417-111">Permission type</span></span>|<span data-ttu-id="2c417-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c417-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c417-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c417-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2c417-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="2c417-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2c417-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c417-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c417-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c417-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c417-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c417-117">Not supported.</span></span>|
|<span data-ttu-id="2c417-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c417-118">Application</span></span>||
| <span data-ttu-id="2c417-119">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="2c417-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2c417-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c417-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c417-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c417-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2c417-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c417-122">Request headers</span></span>
|<span data-ttu-id="2c417-123">标头</span><span class="sxs-lookup"><span data-stu-id="2c417-123">Header</span></span>|<span data-ttu-id="2c417-124">值</span><span class="sxs-lookup"><span data-stu-id="2c417-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c417-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c417-125">Authorization</span></span>|<span data-ttu-id="2c417-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c417-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c417-127">接受</span><span class="sxs-lookup"><span data-stu-id="2c417-127">Accept</span></span>|<span data-ttu-id="2c417-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2c417-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c417-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c417-129">Request body</span></span>
<span data-ttu-id="2c417-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c417-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2c417-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2c417-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2c417-132">属性</span><span class="sxs-lookup"><span data-stu-id="2c417-132">Property</span></span>|<span data-ttu-id="2c417-133">类型</span><span class="sxs-lookup"><span data-stu-id="2c417-133">Type</span></span>|<span data-ttu-id="2c417-134">说明</span><span class="sxs-lookup"><span data-stu-id="2c417-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c417-135">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="2c417-135">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="2c417-136">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c417-136">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="2c417-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2c417-137">Not yet documented</span></span>|
|<span data-ttu-id="2c417-138">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="2c417-138">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="2c417-139">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c417-139">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2c417-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2c417-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2c417-141">响应</span><span class="sxs-lookup"><span data-stu-id="2c417-141">Response</span></span>
<span data-ttu-id="2c417-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2c417-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c417-143">示例</span><span class="sxs-lookup"><span data-stu-id="2c417-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c417-144">请求</span><span class="sxs-lookup"><span data-stu-id="2c417-144">Request</span></span>
<span data-ttu-id="2c417-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c417-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign

Content-type: application/json
Content-length: 578

{
  "appProvisioningConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ],
  "iOSLobAppProvisioningConfigAssignments": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2c417-146">响应</span><span class="sxs-lookup"><span data-stu-id="2c417-146">Response</span></span>
<span data-ttu-id="2c417-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c417-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








