---
title: 列出 deviceCategories
description: 列出 deviceCategory 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9f3b484a3a518028e826f34092e7295a8a9d7d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868528"
---
# <a name="list-devicecategories"></a><span data-ttu-id="b20ab-103">列出 deviceCategories</span><span class="sxs-lookup"><span data-stu-id="b20ab-103">List deviceCategories</span></span>

> <span data-ttu-id="b20ab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b20ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b20ab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b20ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b20ab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b20ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b20ab-107">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b20ab-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b20ab-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b20ab-108">Prerequisites</span></span>
<span data-ttu-id="b20ab-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b20ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20ab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b20ab-111">Permission type</span></span>|<span data-ttu-id="b20ab-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b20ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20ab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b20ab-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b20ab-114">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="b20ab-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b20ab-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b20ab-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b20ab-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b20ab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20ab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b20ab-117">Not supported.</span></span>|
|<span data-ttu-id="b20ab-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b20ab-118">Application</span></span>|<span data-ttu-id="b20ab-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b20ab-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20ab-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b20ab-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="b20ab-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b20ab-121">Request headers</span></span>

|<span data-ttu-id="b20ab-122">标头</span><span class="sxs-lookup"><span data-stu-id="b20ab-122">Header</span></span>|<span data-ttu-id="b20ab-123">值</span><span class="sxs-lookup"><span data-stu-id="b20ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b20ab-124">Authorization</span></span>|<span data-ttu-id="b20ab-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b20ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20ab-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b20ab-126">Accept</span></span>|<span data-ttu-id="b20ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b20ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b20ab-128">Request body</span></span>

<span data-ttu-id="b20ab-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b20ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b20ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="b20ab-130">Response</span></span>

<span data-ttu-id="b20ab-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b20ab-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="b20ab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b20ab-133">请求</span><span class="sxs-lookup"><span data-stu-id="b20ab-133">Request</span></span>

<span data-ttu-id="b20ab-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b20ab-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="b20ab-135">响应</span><span class="sxs-lookup"><span data-stu-id="b20ab-135">Response</span></span>

<span data-ttu-id="b20ab-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b20ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



