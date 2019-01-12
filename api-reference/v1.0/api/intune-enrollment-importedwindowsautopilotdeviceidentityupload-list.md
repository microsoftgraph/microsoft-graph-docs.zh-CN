---
title: 列表 importedWindowsAutopilotDeviceIdentityUploads
description: 列出属性和 importedWindowsAutopilotDeviceIdentityUpload 对象之间的关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38c072ef398b3425fb114a1ec7c03918894168d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951283"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="f2fa5-103">列表 importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="f2fa5-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="f2fa5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2fa5-105">列出属性和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2fa5-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2fa5-106">Prerequisites</span></span>
<span data-ttu-id="f2fa5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f2fa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2fa5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2fa5-109">Permission type</span></span>|<span data-ttu-id="f2fa5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2fa5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2fa5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2fa5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2fa5-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2fa5-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f2fa5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2fa5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2fa5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-114">Not supported.</span></span>|
|<span data-ttu-id="f2fa5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2fa5-115">Application</span></span>|<span data-ttu-id="f2fa5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2fa5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2fa5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="f2fa5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2fa5-118">Request headers</span></span>
|<span data-ttu-id="f2fa5-119">标头</span><span class="sxs-lookup"><span data-stu-id="f2fa5-119">Header</span></span>|<span data-ttu-id="f2fa5-120">值</span><span class="sxs-lookup"><span data-stu-id="f2fa5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2fa5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2fa5-121">Authorization</span></span>|<span data-ttu-id="f2fa5-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2fa5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f2fa5-123">Accept</span></span>|<span data-ttu-id="f2fa5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2fa5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2fa5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2fa5-125">Request body</span></span>
<span data-ttu-id="f2fa5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2fa5-127">响应</span><span class="sxs-lookup"><span data-stu-id="f2fa5-127">Response</span></span>
<span data-ttu-id="f2fa5-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2fa5-129">示例</span><span class="sxs-lookup"><span data-stu-id="f2fa5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2fa5-130">请求</span><span class="sxs-lookup"><span data-stu-id="f2fa5-130">Request</span></span>
<span data-ttu-id="f2fa5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="f2fa5-132">响应</span><span class="sxs-lookup"><span data-stu-id="f2fa5-132">Response</span></span>
<span data-ttu-id="f2fa5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2fa5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```



