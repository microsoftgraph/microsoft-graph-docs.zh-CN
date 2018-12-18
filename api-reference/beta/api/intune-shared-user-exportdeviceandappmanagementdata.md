---
title: exportDeviceAndAppManagementData 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 3ec79080a2e4f6f5da3622dedfedc486231703ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352218"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="27ac6-103">exportDeviceAndAppManagementData 函数</span><span class="sxs-lookup"><span data-stu-id="27ac6-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="27ac6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27ac6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27ac6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27ac6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27ac6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="27ac6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27ac6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27ac6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27ac6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27ac6-108">Prerequisites</span></span>

<span data-ttu-id="27ac6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="27ac6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27ac6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27ac6-111">Permission type</span></span>|<span data-ttu-id="27ac6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27ac6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27ac6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27ac6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27ac6-114">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="27ac6-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="27ac6-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27ac6-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27ac6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27ac6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27ac6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="27ac6-117">Not supported.</span></span>|
|<span data-ttu-id="27ac6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="27ac6-118">Application</span></span>|<span data-ttu-id="27ac6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="27ac6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27ac6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27ac6-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="27ac6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="27ac6-121">Request headers</span></span>

|<span data-ttu-id="27ac6-122">标头</span><span class="sxs-lookup"><span data-stu-id="27ac6-122">Header</span></span>|<span data-ttu-id="27ac6-123">值</span><span class="sxs-lookup"><span data-stu-id="27ac6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27ac6-124">授权</span><span class="sxs-lookup"><span data-stu-id="27ac6-124">Authorization</span></span>|<span data-ttu-id="27ac6-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27ac6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27ac6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="27ac6-126">Accept</span></span>|<span data-ttu-id="27ac6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="27ac6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27ac6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="27ac6-128">Request body</span></span>

<span data-ttu-id="27ac6-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="27ac6-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="27ac6-130">属性</span><span class="sxs-lookup"><span data-stu-id="27ac6-130">Property</span></span>|<span data-ttu-id="27ac6-131">类型</span><span class="sxs-lookup"><span data-stu-id="27ac6-131">Type</span></span>|<span data-ttu-id="27ac6-132">说明</span><span class="sxs-lookup"><span data-stu-id="27ac6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ac6-133">skip</span><span class="sxs-lookup"><span data-stu-id="27ac6-133">skip</span></span>|<span data-ttu-id="27ac6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="27ac6-134">Int32</span></span>|<span data-ttu-id="27ac6-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27ac6-135">Not yet documented</span></span>|
|<span data-ttu-id="27ac6-136">top</span><span class="sxs-lookup"><span data-stu-id="27ac6-136">top</span></span>|<span data-ttu-id="27ac6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="27ac6-137">Int32</span></span>|<span data-ttu-id="27ac6-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27ac6-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="27ac6-139">响应</span><span class="sxs-lookup"><span data-stu-id="27ac6-139">Response</span></span>

<span data-ttu-id="27ac6-140">如果成功，此函数返回`200 OK`响应代码和响应正文中[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) 。</span><span class="sxs-lookup"><span data-stu-id="27ac6-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27ac6-141">示例</span><span class="sxs-lookup"><span data-stu-id="27ac6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="27ac6-142">请求</span><span class="sxs-lookup"><span data-stu-id="27ac6-142">Request</span></span>

<span data-ttu-id="27ac6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27ac6-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="27ac6-144">响应</span><span class="sxs-lookup"><span data-stu-id="27ac6-144">Response</span></span>

<span data-ttu-id="27ac6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27ac6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



