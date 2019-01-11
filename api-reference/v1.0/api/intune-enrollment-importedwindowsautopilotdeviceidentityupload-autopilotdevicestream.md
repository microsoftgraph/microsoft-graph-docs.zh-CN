---
title: autopilotDeviceStream 函数
description: 创建自动执行某些操作设备流上载请求。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5e11b4f66b68bcb5e7de083d0894567d8752d746
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867152"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="83d8a-103">autopilotDeviceStream 函数</span><span class="sxs-lookup"><span data-stu-id="83d8a-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="83d8a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="83d8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83d8a-105">创建自动执行某些操作设备流上载请求。</span><span class="sxs-lookup"><span data-stu-id="83d8a-105">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83d8a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="83d8a-106">Prerequisites</span></span>
<span data-ttu-id="83d8a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="83d8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d8a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83d8a-109">Permission type</span></span>|<span data-ttu-id="83d8a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83d8a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d8a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83d8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83d8a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d8a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="83d8a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83d8a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d8a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83d8a-114">Not supported.</span></span>|
|<span data-ttu-id="83d8a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83d8a-115">Application</span></span>|<span data-ttu-id="83d8a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83d8a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83d8a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83d8a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="83d8a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83d8a-118">Request headers</span></span>
|<span data-ttu-id="83d8a-119">标头</span><span class="sxs-lookup"><span data-stu-id="83d8a-119">Header</span></span>|<span data-ttu-id="83d8a-120">值</span><span class="sxs-lookup"><span data-stu-id="83d8a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83d8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83d8a-121">Authorization</span></span>|<span data-ttu-id="83d8a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83d8a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83d8a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83d8a-123">Accept</span></span>|<span data-ttu-id="83d8a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83d8a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d8a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="83d8a-125">Request body</span></span>
<span data-ttu-id="83d8a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83d8a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83d8a-127">响应</span><span class="sxs-lookup"><span data-stu-id="83d8a-127">Response</span></span>
<span data-ttu-id="83d8a-128">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="83d8a-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d8a-129">示例</span><span class="sxs-lookup"><span data-stu-id="83d8a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="83d8a-130">请求</span><span class="sxs-lookup"><span data-stu-id="83d8a-130">Request</span></span>
<span data-ttu-id="83d8a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83d8a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="83d8a-132">响应</span><span class="sxs-lookup"><span data-stu-id="83d8a-132">Response</span></span>
<span data-ttu-id="83d8a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83d8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



