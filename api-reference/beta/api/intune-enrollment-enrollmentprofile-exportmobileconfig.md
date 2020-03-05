---
title: exportMobileConfig 函数
description: 导出移动配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9caca41864f98bd47f474ff96abc2eb09240de38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466890"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="9c8a0-103">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="9c8a0-103">exportMobileConfig function</span></span>

<span data-ttu-id="9c8a0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9c8a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c8a0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c8a0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c8a0-107">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="9c8a0-107">Exports the mobile configuration</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c8a0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c8a0-108">Prerequisites</span></span>
<span data-ttu-id="9c8a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c8a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c8a0-111">Permission type</span></span>|<span data-ttu-id="9c8a0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c8a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c8a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c8a0-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c8a0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c8a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c8a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-116">Not supported.</span></span>|
|<span data-ttu-id="9c8a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c8a0-117">Application</span></span>|<span data-ttu-id="9c8a0-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c8a0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c8a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c8a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="9c8a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c8a0-120">Request headers</span></span>
|<span data-ttu-id="9c8a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c8a0-121">Header</span></span>|<span data-ttu-id="9c8a0-122">值</span><span class="sxs-lookup"><span data-stu-id="9c8a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c8a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c8a0-123">Authorization</span></span>|<span data-ttu-id="9c8a0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c8a0-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c8a0-125">Accept</span></span>|<span data-ttu-id="9c8a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c8a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c8a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c8a0-127">Request body</span></span>
<span data-ttu-id="9c8a0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c8a0-129">响应</span><span class="sxs-lookup"><span data-stu-id="9c8a0-129">Response</span></span>
<span data-ttu-id="9c8a0-130">如果成功，此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c8a0-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c8a0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c8a0-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c8a0-132">Request</span></span>
<span data-ttu-id="9c8a0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="9c8a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c8a0-134">Response</span></span>
<span data-ttu-id="9c8a0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c8a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```





