---
title: 删除 androidForWorkApp
description: 删除 androidForWorkApp。
author: tfitzmac
ms.openlocfilehash: 53ea38fe0e16f4222a9cf65395565787f63d2745
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304009"
---
# <a name="delete-androidforworkapp"></a><span data-ttu-id="30411-103">删除 androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="30411-103">Delete androidForWorkApp</span></span>

> <span data-ttu-id="30411-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="30411-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30411-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="30411-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30411-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30411-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30411-107">删除[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)。</span><span class="sxs-lookup"><span data-stu-id="30411-107">Deletes a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30411-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="30411-108">Prerequisites</span></span>
<span data-ttu-id="30411-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="30411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30411-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30411-111">Permission type</span></span>|<span data-ttu-id="30411-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30411-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30411-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30411-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30411-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30411-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30411-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30411-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30411-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30411-116">Not supported.</span></span>|
|<span data-ttu-id="30411-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="30411-117">Application</span></span>|<span data-ttu-id="30411-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="30411-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30411-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30411-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="30411-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="30411-120">Request headers</span></span>
|<span data-ttu-id="30411-121">标头</span><span class="sxs-lookup"><span data-stu-id="30411-121">Header</span></span>|<span data-ttu-id="30411-122">值</span><span class="sxs-lookup"><span data-stu-id="30411-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30411-123">授权</span><span class="sxs-lookup"><span data-stu-id="30411-123">Authorization</span></span>|<span data-ttu-id="30411-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30411-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30411-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30411-125">Accept</span></span>|<span data-ttu-id="30411-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30411-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30411-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="30411-127">Request body</span></span>
<span data-ttu-id="30411-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30411-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30411-129">响应</span><span class="sxs-lookup"><span data-stu-id="30411-129">Response</span></span>
<span data-ttu-id="30411-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="30411-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="30411-131">示例</span><span class="sxs-lookup"><span data-stu-id="30411-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="30411-132">请求</span><span class="sxs-lookup"><span data-stu-id="30411-132">Request</span></span>
<span data-ttu-id="30411-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30411-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="30411-134">响应</span><span class="sxs-lookup"><span data-stu-id="30411-134">Response</span></span>
<span data-ttu-id="30411-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30411-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





