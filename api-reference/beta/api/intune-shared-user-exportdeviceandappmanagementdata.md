---
title: exportDeviceAndAppManagementData 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9178a63a02297e21bdc9d14c81560867fea400d6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195774"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="227b8-103">exportDeviceAndAppManagementData 函数</span><span class="sxs-lookup"><span data-stu-id="227b8-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="227b8-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="227b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="227b8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="227b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="227b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="227b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227b8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="227b8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="227b8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="227b8-108">Prerequisites</span></span>

<span data-ttu-id="227b8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="227b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227b8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="227b8-111">Permission type</span></span>|<span data-ttu-id="227b8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="227b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="227b8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="227b8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="227b8-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="227b8-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="227b8-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227b8-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="227b8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="227b8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="227b8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="227b8-117">Not supported.</span></span>|
|<span data-ttu-id="227b8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="227b8-118">Application</span></span>||
| <span data-ttu-id="227b8-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="227b8-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="227b8-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227b8-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="227b8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="227b8-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="227b8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="227b8-122">Request headers</span></span>

|<span data-ttu-id="227b8-123">标头</span><span class="sxs-lookup"><span data-stu-id="227b8-123">Header</span></span>|<span data-ttu-id="227b8-124">值</span><span class="sxs-lookup"><span data-stu-id="227b8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="227b8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="227b8-125">Authorization</span></span>|<span data-ttu-id="227b8-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="227b8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="227b8-127">接受</span><span class="sxs-lookup"><span data-stu-id="227b8-127">Accept</span></span>|<span data-ttu-id="227b8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="227b8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="227b8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="227b8-129">Request body</span></span>

<span data-ttu-id="227b8-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="227b8-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="227b8-131">属性</span><span class="sxs-lookup"><span data-stu-id="227b8-131">Property</span></span>|<span data-ttu-id="227b8-132">类型</span><span class="sxs-lookup"><span data-stu-id="227b8-132">Type</span></span>|<span data-ttu-id="227b8-133">说明</span><span class="sxs-lookup"><span data-stu-id="227b8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227b8-134">skip</span><span class="sxs-lookup"><span data-stu-id="227b8-134">skip</span></span>|<span data-ttu-id="227b8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="227b8-135">Int32</span></span>|<span data-ttu-id="227b8-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="227b8-136">Not yet documented</span></span>|
|<span data-ttu-id="227b8-137">top</span><span class="sxs-lookup"><span data-stu-id="227b8-137">top</span></span>|<span data-ttu-id="227b8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="227b8-138">Int32</span></span>|<span data-ttu-id="227b8-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="227b8-139">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="227b8-140">响应</span><span class="sxs-lookup"><span data-stu-id="227b8-140">Response</span></span>

<span data-ttu-id="227b8-141">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) 。</span><span class="sxs-lookup"><span data-stu-id="227b8-141">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="227b8-142">示例</span><span class="sxs-lookup"><span data-stu-id="227b8-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="227b8-143">请求</span><span class="sxs-lookup"><span data-stu-id="227b8-143">Request</span></span>

<span data-ttu-id="227b8-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="227b8-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="227b8-145">响应</span><span class="sxs-lookup"><span data-stu-id="227b8-145">Response</span></span>

<span data-ttu-id="227b8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="227b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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







