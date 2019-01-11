---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7b7f92592a0ece8169b4f4148e71df5b6297ca7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824408"
---
# <a name="assign-action"></a><span data-ttu-id="ecabe-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ecabe-103">assign action</span></span>

> <span data-ttu-id="ecabe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecabe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecabe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecabe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecabe-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecabe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecabe-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecabe-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecabe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecabe-108">Prerequisites</span></span>
<span data-ttu-id="ecabe-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ecabe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecabe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecabe-111">Permission type</span></span>|<span data-ttu-id="ecabe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecabe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecabe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecabe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecabe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecabe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecabe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecabe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecabe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecabe-116">Not supported.</span></span>|
|<span data-ttu-id="ecabe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecabe-117">Application</span></span>|<span data-ttu-id="ecabe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecabe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecabe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecabe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ecabe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecabe-120">Request headers</span></span>
|<span data-ttu-id="ecabe-121">标头</span><span class="sxs-lookup"><span data-stu-id="ecabe-121">Header</span></span>|<span data-ttu-id="ecabe-122">值</span><span class="sxs-lookup"><span data-stu-id="ecabe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecabe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecabe-123">Authorization</span></span>|<span data-ttu-id="ecabe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecabe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecabe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecabe-125">Accept</span></span>|<span data-ttu-id="ecabe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecabe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecabe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecabe-127">Request body</span></span>
<span data-ttu-id="ecabe-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecabe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ecabe-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ecabe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ecabe-130">属性</span><span class="sxs-lookup"><span data-stu-id="ecabe-130">Property</span></span>|<span data-ttu-id="ecabe-131">类型</span><span class="sxs-lookup"><span data-stu-id="ecabe-131">Type</span></span>|<span data-ttu-id="ecabe-132">Description</span><span class="sxs-lookup"><span data-stu-id="ecabe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecabe-133">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="ecabe-133">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="ecabe-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecabe-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="ecabe-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecabe-135">Not yet documented</span></span>|
|<span data-ttu-id="ecabe-136">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="ecabe-136">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="ecabe-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecabe-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ecabe-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecabe-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ecabe-139">响应</span><span class="sxs-lookup"><span data-stu-id="ecabe-139">Response</span></span>
<span data-ttu-id="ecabe-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ecabe-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ecabe-141">示例</span><span class="sxs-lookup"><span data-stu-id="ecabe-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecabe-142">请求</span><span class="sxs-lookup"><span data-stu-id="ecabe-142">Request</span></span>
<span data-ttu-id="ecabe-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecabe-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecabe-144">响应</span><span class="sxs-lookup"><span data-stu-id="ecabe-144">Response</span></span>
<span data-ttu-id="ecabe-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecabe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





