---
title: exportDeviceAndAppManagementData 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e36936710bcd97c10c4a69c496cf56ceffa43e46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527005"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="d9496-103">exportDeviceAndAppManagementData 函数</span><span class="sxs-lookup"><span data-stu-id="d9496-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="d9496-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9496-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9496-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9496-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9496-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9496-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9496-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9496-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9496-108">Prerequisites</span></span>

<span data-ttu-id="d9496-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9496-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9496-111">Permission type</span></span>|<span data-ttu-id="d9496-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9496-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9496-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9496-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d9496-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d9496-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d9496-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9496-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9496-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9496-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9496-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9496-117">Not supported.</span></span>|
|<span data-ttu-id="d9496-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9496-118">Application</span></span>|<span data-ttu-id="d9496-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9496-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9496-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9496-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="d9496-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9496-121">Request headers</span></span>

|<span data-ttu-id="d9496-122">标头</span><span class="sxs-lookup"><span data-stu-id="d9496-122">Header</span></span>|<span data-ttu-id="d9496-123">值</span><span class="sxs-lookup"><span data-stu-id="d9496-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9496-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9496-124">Authorization</span></span>|<span data-ttu-id="d9496-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9496-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9496-126">接受</span><span class="sxs-lookup"><span data-stu-id="d9496-126">Accept</span></span>|<span data-ttu-id="d9496-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d9496-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9496-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9496-128">Request body</span></span>

<span data-ttu-id="d9496-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d9496-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d9496-130">属性</span><span class="sxs-lookup"><span data-stu-id="d9496-130">Property</span></span>|<span data-ttu-id="d9496-131">类型</span><span class="sxs-lookup"><span data-stu-id="d9496-131">Type</span></span>|<span data-ttu-id="d9496-132">说明</span><span class="sxs-lookup"><span data-stu-id="d9496-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9496-133">skip</span><span class="sxs-lookup"><span data-stu-id="d9496-133">skip</span></span>|<span data-ttu-id="d9496-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d9496-134">Int32</span></span>|<span data-ttu-id="d9496-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9496-135">Not yet documented</span></span>|
|<span data-ttu-id="d9496-136">top</span><span class="sxs-lookup"><span data-stu-id="d9496-136">top</span></span>|<span data-ttu-id="d9496-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d9496-137">Int32</span></span>|<span data-ttu-id="d9496-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9496-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="d9496-139">响应</span><span class="sxs-lookup"><span data-stu-id="d9496-139">Response</span></span>

<span data-ttu-id="d9496-140">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) 。</span><span class="sxs-lookup"><span data-stu-id="d9496-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9496-141">示例</span><span class="sxs-lookup"><span data-stu-id="d9496-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9496-142">请求</span><span class="sxs-lookup"><span data-stu-id="d9496-142">Request</span></span>

<span data-ttu-id="d9496-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9496-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="d9496-144">响应</span><span class="sxs-lookup"><span data-stu-id="d9496-144">Response</span></span>

<span data-ttu-id="d9496-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9496-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



