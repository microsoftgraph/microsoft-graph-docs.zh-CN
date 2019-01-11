---
title: 删除 iosMobileAppConfiguration
description: 删除 iosMobileAppConfiguration。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 60c94926eec662ec4ed5e9e800de1f19973bccfb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875255"
---
# <a name="delete-iosmobileappconfiguration"></a><span data-ttu-id="1bb27-103">删除 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bb27-103">Delete iosMobileAppConfiguration</span></span>

> <span data-ttu-id="1bb27-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1bb27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bb27-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1bb27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bb27-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1bb27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bb27-107">删除 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1bb27-107">Deletes a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1bb27-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bb27-108">Prerequisites</span></span>
<span data-ttu-id="1bb27-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1bb27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb27-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bb27-111">Permission type</span></span>|<span data-ttu-id="1bb27-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bb27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb27-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bb27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb27-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb27-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bb27-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bb27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb27-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bb27-116">Not supported.</span></span>|
|<span data-ttu-id="1bb27-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bb27-117">Application</span></span>|<span data-ttu-id="1bb27-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bb27-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb27-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bb27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1bb27-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bb27-120">Request headers</span></span>
|<span data-ttu-id="1bb27-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bb27-121">Header</span></span>|<span data-ttu-id="1bb27-122">值</span><span class="sxs-lookup"><span data-stu-id="1bb27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bb27-123">Authorization</span></span>|<span data-ttu-id="1bb27-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bb27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bb27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bb27-125">Accept</span></span>|<span data-ttu-id="1bb27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb27-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bb27-127">Request body</span></span>
<span data-ttu-id="1bb27-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bb27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bb27-129">响应</span><span class="sxs-lookup"><span data-stu-id="1bb27-129">Response</span></span>
<span data-ttu-id="1bb27-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1bb27-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bb27-131">示例</span><span class="sxs-lookup"><span data-stu-id="1bb27-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1bb27-132">请求</span><span class="sxs-lookup"><span data-stu-id="1bb27-132">Request</span></span>
<span data-ttu-id="1bb27-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bb27-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1bb27-134">响应</span><span class="sxs-lookup"><span data-stu-id="1bb27-134">Response</span></span>
<span data-ttu-id="1bb27-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bb27-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





