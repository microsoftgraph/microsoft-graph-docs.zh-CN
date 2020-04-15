---
title: setMobileDeviceManagementAuthority 操作
description: 设置移动设备管理机构
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 872a9b590aba6150a8d38789b9dea0a5a132281e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452885"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="86470-103">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="86470-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="86470-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86470-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86470-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86470-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86470-106">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="86470-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86470-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86470-107">Prerequisites</span></span>
<span data-ttu-id="86470-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86470-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86470-110">Permission type</span></span>|<span data-ttu-id="86470-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86470-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86470-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86470-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86470-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86470-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86470-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86470-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86470-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86470-115">Not supported.</span></span>|
|<span data-ttu-id="86470-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86470-116">Application</span></span>|<span data-ttu-id="86470-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="86470-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86470-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86470-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="86470-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86470-119">Request headers</span></span>
|<span data-ttu-id="86470-120">标头</span><span class="sxs-lookup"><span data-stu-id="86470-120">Header</span></span>|<span data-ttu-id="86470-121">值</span><span class="sxs-lookup"><span data-stu-id="86470-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86470-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86470-122">Authorization</span></span>|<span data-ttu-id="86470-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86470-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86470-124">接受</span><span class="sxs-lookup"><span data-stu-id="86470-124">Accept</span></span>|<span data-ttu-id="86470-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86470-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86470-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86470-126">Request body</span></span>
<span data-ttu-id="86470-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86470-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86470-128">响应</span><span class="sxs-lookup"><span data-stu-id="86470-128">Response</span></span>
<span data-ttu-id="86470-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Int32。</span><span class="sxs-lookup"><span data-stu-id="86470-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86470-130">示例</span><span class="sxs-lookup"><span data-stu-id="86470-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86470-131">请求</span><span class="sxs-lookup"><span data-stu-id="86470-131">Request</span></span>
<span data-ttu-id="86470-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86470-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="86470-133">响应</span><span class="sxs-lookup"><span data-stu-id="86470-133">Response</span></span>
<span data-ttu-id="86470-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```






