---
title: getManagedAppDiagnosticStatuses 函数
description: 获取给定用户的诊断验证状态。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d08785b8eff6d8233476132d21934336eadd076
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511983"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="1a2f6-103">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="1a2f6-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="1a2f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a2f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a2f6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a2f6-106">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-106">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a2f6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a2f6-107">Prerequisites</span></span>
<span data-ttu-id="1a2f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a2f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a2f6-110">Permission type</span></span>|<span data-ttu-id="1a2f6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a2f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a2f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a2f6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1a2f6-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="1a2f6-113">_varies by context_</span></span>|
| <span data-ttu-id="1a2f6-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1a2f6-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="1a2f6-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a2f6-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="1a2f6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a2f6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a2f6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-117">Not supported.</span></span>|
|<span data-ttu-id="1a2f6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a2f6-118">Application</span></span>|<span data-ttu-id="1a2f6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a2f6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a2f6-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1a2f6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a2f6-121">Request headers</span></span>
|<span data-ttu-id="1a2f6-122">标头</span><span class="sxs-lookup"><span data-stu-id="1a2f6-122">Header</span></span>|<span data-ttu-id="1a2f6-123">值</span><span class="sxs-lookup"><span data-stu-id="1a2f6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a2f6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a2f6-124">Authorization</span></span>|<span data-ttu-id="1a2f6-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a2f6-126">接受</span><span class="sxs-lookup"><span data-stu-id="1a2f6-126">Accept</span></span>|<span data-ttu-id="1a2f6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1a2f6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a2f6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a2f6-128">Request body</span></span>
<span data-ttu-id="1a2f6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a2f6-130">响应</span><span class="sxs-lookup"><span data-stu-id="1a2f6-130">Response</span></span>
<span data-ttu-id="1a2f6-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a2f6-132">示例</span><span class="sxs-lookup"><span data-stu-id="1a2f6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a2f6-133">请求</span><span class="sxs-lookup"><span data-stu-id="1a2f6-133">Request</span></span>
<span data-ttu-id="1a2f6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="1a2f6-135">响应</span><span class="sxs-lookup"><span data-stu-id="1a2f6-135">Response</span></span>
<span data-ttu-id="1a2f6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a2f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```




