---
title: setMobileDeviceManagementAuthority 操作
description: 设置移动设备管理机构
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee7032ff38f0be2336821d61d59a7086a9381483
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752495"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="b41be-103">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="b41be-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="b41be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b41be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b41be-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b41be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b41be-106">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="b41be-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b41be-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b41be-107">Prerequisites</span></span>
<span data-ttu-id="b41be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b41be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b41be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b41be-110">Permission type</span></span>|<span data-ttu-id="b41be-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b41be-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b41be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b41be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b41be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b41be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b41be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b41be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b41be-115">Not supported.</span></span>|
|<span data-ttu-id="b41be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b41be-116">Application</span></span>|<span data-ttu-id="b41be-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41be-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b41be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b41be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="b41be-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b41be-119">Request headers</span></span>
|<span data-ttu-id="b41be-120">标头</span><span class="sxs-lookup"><span data-stu-id="b41be-120">Header</span></span>|<span data-ttu-id="b41be-121">值</span><span class="sxs-lookup"><span data-stu-id="b41be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b41be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b41be-122">Authorization</span></span>|<span data-ttu-id="b41be-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b41be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b41be-124">接受</span><span class="sxs-lookup"><span data-stu-id="b41be-124">Accept</span></span>|<span data-ttu-id="b41be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b41be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b41be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b41be-126">Request body</span></span>
<span data-ttu-id="b41be-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b41be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b41be-128">响应</span><span class="sxs-lookup"><span data-stu-id="b41be-128">Response</span></span>
<span data-ttu-id="b41be-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Int32。</span><span class="sxs-lookup"><span data-stu-id="b41be-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b41be-130">示例</span><span class="sxs-lookup"><span data-stu-id="b41be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b41be-131">请求</span><span class="sxs-lookup"><span data-stu-id="b41be-131">Request</span></span>
<span data-ttu-id="b41be-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b41be-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="b41be-133">响应</span><span class="sxs-lookup"><span data-stu-id="b41be-133">Response</span></span>
<span data-ttu-id="b41be-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b41be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




