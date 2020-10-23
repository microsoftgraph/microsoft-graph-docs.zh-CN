---
title: exportDeviceAndAppManagementData 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e827fb1f4c6375ad8e9d090515578d0b546eaca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728632"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="b649d-103">exportDeviceAndAppManagementData 函数</span><span class="sxs-lookup"><span data-stu-id="b649d-103">exportDeviceAndAppManagementData function</span></span>

<span data-ttu-id="b649d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b649d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b649d-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b649d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b649d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b649d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b649d-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b649d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b649d-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b649d-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b649d-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="b649d-109">Prerequisites</span></span>

<span data-ttu-id="b649d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b649d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b649d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b649d-112">Permission type</span></span>|<span data-ttu-id="b649d-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b649d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b649d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b649d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b649d-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b649d-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b649d-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b649d-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b649d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b649d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b649d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b649d-118">Not supported.</span></span>|
|<span data-ttu-id="b649d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b649d-119">Application</span></span>||
| <span data-ttu-id="b649d-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b649d-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b649d-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b649d-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b649d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b649d-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="b649d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b649d-123">Request headers</span></span>

|<span data-ttu-id="b649d-124">标头</span><span class="sxs-lookup"><span data-stu-id="b649d-124">Header</span></span>|<span data-ttu-id="b649d-125">值</span><span class="sxs-lookup"><span data-stu-id="b649d-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b649d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b649d-126">Authorization</span></span>|<span data-ttu-id="b649d-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b649d-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b649d-128">接受</span><span class="sxs-lookup"><span data-stu-id="b649d-128">Accept</span></span>|<span data-ttu-id="b649d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b649d-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b649d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b649d-130">Request body</span></span>

<span data-ttu-id="b649d-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b649d-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b649d-132">属性</span><span class="sxs-lookup"><span data-stu-id="b649d-132">Property</span></span>|<span data-ttu-id="b649d-133">类型</span><span class="sxs-lookup"><span data-stu-id="b649d-133">Type</span></span>|<span data-ttu-id="b649d-134">说明</span><span class="sxs-lookup"><span data-stu-id="b649d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b649d-135">skip</span><span class="sxs-lookup"><span data-stu-id="b649d-135">skip</span></span>|<span data-ttu-id="b649d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b649d-136">Int32</span></span>|<span data-ttu-id="b649d-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b649d-137">Not yet documented</span></span>|
|<span data-ttu-id="b649d-138">top</span><span class="sxs-lookup"><span data-stu-id="b649d-138">top</span></span>|<span data-ttu-id="b649d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b649d-139">Int32</span></span>|<span data-ttu-id="b649d-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b649d-140">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="b649d-141">响应</span><span class="sxs-lookup"><span data-stu-id="b649d-141">Response</span></span>

<span data-ttu-id="b649d-142">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) 。</span><span class="sxs-lookup"><span data-stu-id="b649d-142">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b649d-143">示例</span><span class="sxs-lookup"><span data-stu-id="b649d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b649d-144">请求</span><span class="sxs-lookup"><span data-stu-id="b649d-144">Request</span></span>

<span data-ttu-id="b649d-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b649d-145">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="b649d-146">响应</span><span class="sxs-lookup"><span data-stu-id="b649d-146">Response</span></span>

<span data-ttu-id="b649d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b649d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











