---
title: exportMobileConfig 函数
description: 导出移动配置
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2bb1ef99054527c058d5a1598133d3653ccf8777
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975362"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="e8abe-103">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="e8abe-103">exportMobileConfig function</span></span>

> <span data-ttu-id="e8abe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8abe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8abe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8abe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8abe-106">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="e8abe-106">Exports the mobile configuration</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8abe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8abe-107">Prerequisites</span></span>
<span data-ttu-id="e8abe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8abe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8abe-110">Permission type</span></span>|<span data-ttu-id="e8abe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8abe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8abe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8abe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8abe-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8abe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e8abe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8abe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8abe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8abe-115">Not supported.</span></span>|
|<span data-ttu-id="e8abe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8abe-116">Application</span></span>|<span data-ttu-id="e8abe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8abe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8abe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8abe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="e8abe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8abe-119">Request headers</span></span>
|<span data-ttu-id="e8abe-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8abe-120">Header</span></span>|<span data-ttu-id="e8abe-121">值</span><span class="sxs-lookup"><span data-stu-id="e8abe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8abe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8abe-122">Authorization</span></span>|<span data-ttu-id="e8abe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8abe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8abe-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8abe-124">Accept</span></span>|<span data-ttu-id="e8abe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8abe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8abe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8abe-126">Request body</span></span>
<span data-ttu-id="e8abe-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8abe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8abe-128">响应</span><span class="sxs-lookup"><span data-stu-id="e8abe-128">Response</span></span>
<span data-ttu-id="e8abe-129">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="e8abe-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8abe-130">示例</span><span class="sxs-lookup"><span data-stu-id="e8abe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8abe-131">请求</span><span class="sxs-lookup"><span data-stu-id="e8abe-131">Request</span></span>
<span data-ttu-id="e8abe-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8abe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="e8abe-133">响应</span><span class="sxs-lookup"><span data-stu-id="e8abe-133">Response</span></span>
<span data-ttu-id="e8abe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8abe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```




