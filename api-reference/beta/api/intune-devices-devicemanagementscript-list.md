---
title: 列表 deviceManagementScripts
description: 列出属性和 deviceManagementScript 对象之间的关系。
author: tfitzmac
ms.openlocfilehash: 4c3f9163445fce348fe3e2a9b2635a0c44cab864
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363702"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="2bb19-103">列表 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="2bb19-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="2bb19-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2bb19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bb19-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2bb19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bb19-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2bb19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bb19-107">列出属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="2bb19-107">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bb19-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2bb19-108">Prerequisites</span></span>
<span data-ttu-id="2bb19-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2bb19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bb19-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bb19-111">Permission type</span></span>|<span data-ttu-id="2bb19-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2bb19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bb19-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bb19-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bb19-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2bb19-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bb19-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bb19-116">Not supported.</span></span>|
|<span data-ttu-id="2bb19-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bb19-117">Application</span></span>|<span data-ttu-id="2bb19-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bb19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bb19-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bb19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="2bb19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bb19-120">Request headers</span></span>
|<span data-ttu-id="2bb19-121">标头</span><span class="sxs-lookup"><span data-stu-id="2bb19-121">Header</span></span>|<span data-ttu-id="2bb19-122">值</span><span class="sxs-lookup"><span data-stu-id="2bb19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bb19-123">授权</span><span class="sxs-lookup"><span data-stu-id="2bb19-123">Authorization</span></span>|<span data-ttu-id="2bb19-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2bb19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bb19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2bb19-125">Accept</span></span>|<span data-ttu-id="2bb19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bb19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb19-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bb19-127">Request body</span></span>
<span data-ttu-id="2bb19-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bb19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bb19-129">响应</span><span class="sxs-lookup"><span data-stu-id="2bb19-129">Response</span></span>
<span data-ttu-id="2bb19-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2bb19-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb19-131">示例</span><span class="sxs-lookup"><span data-stu-id="2bb19-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2bb19-132">请求</span><span class="sxs-lookup"><span data-stu-id="2bb19-132">Request</span></span>
<span data-ttu-id="2bb19-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bb19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="2bb19-134">响应</span><span class="sxs-lookup"><span data-stu-id="2bb19-134">Response</span></span>
<span data-ttu-id="2bb19-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bb19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value"
    }
  ]
}
```





