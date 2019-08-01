---
title: getManagedAppDiagnosticStatuses 函数
description: 获取给定用户的诊断验证状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c12d3f03fd608f23a94afcf4ac7a2a75a6d8f846
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025797"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="263b7-103">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="263b7-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="263b7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="263b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263b7-105">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="263b7-105">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="263b7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="263b7-106">Prerequisites</span></span>
<span data-ttu-id="263b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="263b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="263b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="263b7-109">Permission type</span></span>|<span data-ttu-id="263b7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="263b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="263b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="263b7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="263b7-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="263b7-112">_varies by context_</span></span>|
| <span data-ttu-id="263b7-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="263b7-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="263b7-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="263b7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="263b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="263b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="263b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="263b7-116">Not supported.</span></span>|
|<span data-ttu-id="263b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="263b7-117">Application</span></span>|<span data-ttu-id="263b7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="263b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="263b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="263b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="263b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="263b7-120">Request headers</span></span>
|<span data-ttu-id="263b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="263b7-121">Header</span></span>|<span data-ttu-id="263b7-122">值</span><span class="sxs-lookup"><span data-stu-id="263b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="263b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="263b7-123">Authorization</span></span>|<span data-ttu-id="263b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="263b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="263b7-125">接受</span><span class="sxs-lookup"><span data-stu-id="263b7-125">Accept</span></span>|<span data-ttu-id="263b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="263b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="263b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="263b7-127">Request body</span></span>
<span data-ttu-id="263b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="263b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="263b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="263b7-129">Response</span></span>
<span data-ttu-id="263b7-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="263b7-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="263b7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="263b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="263b7-132">Request</span></span>
<span data-ttu-id="263b7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="263b7-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="263b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="263b7-134">Response</span></span>
<span data-ttu-id="263b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="263b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



