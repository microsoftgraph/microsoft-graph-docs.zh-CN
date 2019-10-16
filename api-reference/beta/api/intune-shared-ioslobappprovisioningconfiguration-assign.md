---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f929e9c2d07ac22cbbce72333b8eea1847f8570
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538355"
---
# <a name="assign-action"></a><span data-ttu-id="d3afa-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="d3afa-103">assign action</span></span>

> <span data-ttu-id="d3afa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3afa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3afa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3afa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3afa-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3afa-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3afa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3afa-107">Prerequisites</span></span>
<span data-ttu-id="d3afa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3afa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3afa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3afa-110">Permission type</span></span>|<span data-ttu-id="d3afa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3afa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3afa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3afa-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d3afa-113">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d3afa-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d3afa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3afa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3afa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3afa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3afa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3afa-116">Not supported.</span></span>|
|<span data-ttu-id="d3afa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3afa-117">Application</span></span>||
| <span data-ttu-id="d3afa-118">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="d3afa-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d3afa-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3afa-119">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3afa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3afa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d3afa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3afa-121">Request headers</span></span>
|<span data-ttu-id="d3afa-122">标头</span><span class="sxs-lookup"><span data-stu-id="d3afa-122">Header</span></span>|<span data-ttu-id="d3afa-123">值</span><span class="sxs-lookup"><span data-stu-id="d3afa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3afa-124">授权</span><span class="sxs-lookup"><span data-stu-id="d3afa-124">Authorization</span></span>|<span data-ttu-id="d3afa-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3afa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3afa-126">接受</span><span class="sxs-lookup"><span data-stu-id="d3afa-126">Accept</span></span>|<span data-ttu-id="d3afa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d3afa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3afa-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3afa-128">Request body</span></span>
<span data-ttu-id="d3afa-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3afa-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d3afa-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d3afa-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d3afa-131">属性</span><span class="sxs-lookup"><span data-stu-id="d3afa-131">Property</span></span>|<span data-ttu-id="d3afa-132">类型</span><span class="sxs-lookup"><span data-stu-id="d3afa-132">Type</span></span>|<span data-ttu-id="d3afa-133">说明</span><span class="sxs-lookup"><span data-stu-id="d3afa-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3afa-134">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d3afa-134">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="d3afa-135">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3afa-135">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="d3afa-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3afa-136">Not yet documented</span></span>|
|<span data-ttu-id="d3afa-137">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="d3afa-137">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="d3afa-138">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3afa-138">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d3afa-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3afa-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d3afa-140">响应</span><span class="sxs-lookup"><span data-stu-id="d3afa-140">Response</span></span>
<span data-ttu-id="d3afa-141">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d3afa-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3afa-142">示例</span><span class="sxs-lookup"><span data-stu-id="d3afa-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3afa-143">请求</span><span class="sxs-lookup"><span data-stu-id="d3afa-143">Request</span></span>
<span data-ttu-id="d3afa-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3afa-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3afa-145">响应</span><span class="sxs-lookup"><span data-stu-id="d3afa-145">Response</span></span>
<span data-ttu-id="d3afa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3afa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






