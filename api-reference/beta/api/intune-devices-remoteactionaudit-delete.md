---
title: 删除 remoteActionAudit
description: 删除 remoteActionAudit。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 639e394f474c92fd758cdab9b7ec0ccdce17e1e9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958156"
---
# <a name="delete-remoteactionaudit"></a><span data-ttu-id="cff27-103">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="cff27-103">Delete remoteActionAudit</span></span>

> <span data-ttu-id="cff27-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cff27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cff27-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cff27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cff27-106">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="cff27-106">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cff27-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cff27-107">Prerequisites</span></span>
<span data-ttu-id="cff27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cff27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff27-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cff27-110">Permission type</span></span>|<span data-ttu-id="cff27-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cff27-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff27-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cff27-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cff27-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cff27-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cff27-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cff27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff27-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff27-115">Not supported.</span></span>|
|<span data-ttu-id="cff27-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cff27-116">Application</span></span>|<span data-ttu-id="cff27-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cff27-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff27-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cff27-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="cff27-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cff27-119">Request headers</span></span>
|<span data-ttu-id="cff27-120">标头</span><span class="sxs-lookup"><span data-stu-id="cff27-120">Header</span></span>|<span data-ttu-id="cff27-121">值</span><span class="sxs-lookup"><span data-stu-id="cff27-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff27-122">Authorization</span></span>|<span data-ttu-id="cff27-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cff27-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff27-124">接受</span><span class="sxs-lookup"><span data-stu-id="cff27-124">Accept</span></span>|<span data-ttu-id="cff27-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cff27-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff27-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cff27-126">Request body</span></span>
<span data-ttu-id="cff27-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cff27-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cff27-128">响应</span><span class="sxs-lookup"><span data-stu-id="cff27-128">Response</span></span>
<span data-ttu-id="cff27-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cff27-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cff27-130">示例</span><span class="sxs-lookup"><span data-stu-id="cff27-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cff27-131">请求</span><span class="sxs-lookup"><span data-stu-id="cff27-131">Request</span></span>
<span data-ttu-id="cff27-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cff27-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="cff27-133">响应</span><span class="sxs-lookup"><span data-stu-id="cff27-133">Response</span></span>
<span data-ttu-id="cff27-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cff27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





