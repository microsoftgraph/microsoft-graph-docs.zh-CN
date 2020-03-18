---
title: setMobileDeviceManagementAuthority 操作
description: 设置移动设备管理机构
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac3a9d30741572a91576bd93ca48e84d8606f575
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802746"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="a1498-103">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="a1498-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="a1498-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1498-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1498-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1498-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1498-106">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="a1498-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1498-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1498-107">Prerequisites</span></span>
<span data-ttu-id="a1498-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1498-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1498-110">Permission type</span></span>|<span data-ttu-id="a1498-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1498-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1498-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1498-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1498-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1498-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1498-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1498-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1498-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1498-115">Not supported.</span></span>|
|<span data-ttu-id="a1498-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1498-116">Application</span></span>|<span data-ttu-id="a1498-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1498-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1498-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1498-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="a1498-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1498-119">Request headers</span></span>
|<span data-ttu-id="a1498-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1498-120">Header</span></span>|<span data-ttu-id="a1498-121">值</span><span class="sxs-lookup"><span data-stu-id="a1498-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1498-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1498-122">Authorization</span></span>|<span data-ttu-id="a1498-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1498-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1498-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1498-124">Accept</span></span>|<span data-ttu-id="a1498-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1498-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1498-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1498-126">Request body</span></span>
<span data-ttu-id="a1498-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1498-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1498-128">响应</span><span class="sxs-lookup"><span data-stu-id="a1498-128">Response</span></span>
<span data-ttu-id="a1498-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Int32。</span><span class="sxs-lookup"><span data-stu-id="a1498-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1498-130">示例</span><span class="sxs-lookup"><span data-stu-id="a1498-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1498-131">请求</span><span class="sxs-lookup"><span data-stu-id="a1498-131">Request</span></span>
<span data-ttu-id="a1498-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1498-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="a1498-133">响应</span><span class="sxs-lookup"><span data-stu-id="a1498-133">Response</span></span>
<span data-ttu-id="a1498-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1498-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




