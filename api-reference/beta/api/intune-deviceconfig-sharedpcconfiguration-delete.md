---
title: 删除 sharedPCConfiguration
description: 删除 sharedPCConfiguration。
author: tfitzmac
ms.openlocfilehash: 2de013448728da0942b13696be87820b0229fce0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318443"
---
# <a name="delete-sharedpcconfiguration"></a><span data-ttu-id="a6939-103">删除 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6939-103">Delete sharedPCConfiguration</span></span>

> <span data-ttu-id="a6939-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6939-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6939-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6939-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6939-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a6939-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6939-107">删除 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a6939-107">Deletes a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6939-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6939-108">Prerequisites</span></span>
<span data-ttu-id="a6939-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a6939-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6939-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6939-111">Permission type</span></span>|<span data-ttu-id="a6939-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6939-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6939-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6939-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6939-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6939-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6939-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6939-116">Not supported.</span></span>|
|<span data-ttu-id="a6939-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6939-117">Application</span></span>|<span data-ttu-id="a6939-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6939-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6939-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6939-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6939-120">Request headers</span></span>
|<span data-ttu-id="a6939-121">标头</span><span class="sxs-lookup"><span data-stu-id="a6939-121">Header</span></span>|<span data-ttu-id="a6939-122">值</span><span class="sxs-lookup"><span data-stu-id="a6939-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6939-123">授权</span><span class="sxs-lookup"><span data-stu-id="a6939-123">Authorization</span></span>|<span data-ttu-id="a6939-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6939-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6939-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6939-125">Accept</span></span>|<span data-ttu-id="a6939-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6939-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6939-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6939-127">Request body</span></span>
<span data-ttu-id="a6939-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6939-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6939-129">响应</span><span class="sxs-lookup"><span data-stu-id="a6939-129">Response</span></span>
<span data-ttu-id="a6939-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a6939-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6939-131">示例</span><span class="sxs-lookup"><span data-stu-id="a6939-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6939-132">请求</span><span class="sxs-lookup"><span data-stu-id="a6939-132">Request</span></span>
<span data-ttu-id="a6939-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6939-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a6939-134">响应</span><span class="sxs-lookup"><span data-stu-id="a6939-134">Response</span></span>
<span data-ttu-id="a6939-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6939-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





