---
title: 删除 androidForWorkGmailEasConfiguration
description: 删除 androidForWorkGmailEasConfiguration。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a28d21b63360d4d3c5ef24637dfe098b7dc8feff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832583"
---
# <a name="delete-androidforworkgmaileasconfiguration"></a><span data-ttu-id="36242-103">删除 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="36242-103">Delete androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="36242-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="36242-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36242-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36242-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36242-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="36242-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36242-107">删除[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="36242-107">Deletes a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36242-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="36242-108">Prerequisites</span></span>
<span data-ttu-id="36242-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="36242-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36242-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36242-111">Permission type</span></span>|<span data-ttu-id="36242-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36242-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36242-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36242-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36242-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36242-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36242-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36242-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36242-116">Not supported.</span></span>|
|<span data-ttu-id="36242-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36242-117">Application</span></span>|<span data-ttu-id="36242-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="36242-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36242-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36242-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="36242-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36242-120">Request headers</span></span>
|<span data-ttu-id="36242-121">标头</span><span class="sxs-lookup"><span data-stu-id="36242-121">Header</span></span>|<span data-ttu-id="36242-122">值</span><span class="sxs-lookup"><span data-stu-id="36242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36242-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36242-123">Authorization</span></span>|<span data-ttu-id="36242-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36242-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36242-125">Accept</span></span>|<span data-ttu-id="36242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36242-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36242-127">Request body</span></span>
<span data-ttu-id="36242-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36242-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36242-129">响应</span><span class="sxs-lookup"><span data-stu-id="36242-129">Response</span></span>
<span data-ttu-id="36242-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="36242-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36242-131">示例</span><span class="sxs-lookup"><span data-stu-id="36242-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36242-132">请求</span><span class="sxs-lookup"><span data-stu-id="36242-132">Request</span></span>
<span data-ttu-id="36242-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36242-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36242-134">响应</span><span class="sxs-lookup"><span data-stu-id="36242-134">Response</span></span>
<span data-ttu-id="36242-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36242-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





