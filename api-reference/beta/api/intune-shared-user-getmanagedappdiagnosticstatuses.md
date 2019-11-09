---
title: getManagedAppDiagnosticStatuses 函数
description: 获取给定用户的诊断验证状态。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47b9b2da1ed271cbc608a11a2b5fa07bd861fd1a
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085554"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="acd7b-103">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="acd7b-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="acd7b-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="acd7b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="acd7b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="acd7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acd7b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acd7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acd7b-107">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="acd7b-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acd7b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="acd7b-108">Prerequisites</span></span>
<span data-ttu-id="acd7b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acd7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd7b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="acd7b-111">Permission type</span></span>|<span data-ttu-id="acd7b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="acd7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acd7b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acd7b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="acd7b-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="acd7b-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="acd7b-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd7b-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="acd7b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acd7b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acd7b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="acd7b-117">Not supported.</span></span>|
|<span data-ttu-id="acd7b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="acd7b-118">Application</span></span>||
| <span data-ttu-id="acd7b-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="acd7b-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="acd7b-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd7b-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="acd7b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acd7b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="acd7b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="acd7b-122">Request headers</span></span>
|<span data-ttu-id="acd7b-123">标头</span><span class="sxs-lookup"><span data-stu-id="acd7b-123">Header</span></span>|<span data-ttu-id="acd7b-124">值</span><span class="sxs-lookup"><span data-stu-id="acd7b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acd7b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd7b-125">Authorization</span></span>|<span data-ttu-id="acd7b-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="acd7b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acd7b-127">接受</span><span class="sxs-lookup"><span data-stu-id="acd7b-127">Accept</span></span>|<span data-ttu-id="acd7b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="acd7b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd7b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="acd7b-129">Request body</span></span>
<span data-ttu-id="acd7b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="acd7b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd7b-131">响应</span><span class="sxs-lookup"><span data-stu-id="acd7b-131">Response</span></span>
<span data-ttu-id="acd7b-132">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="acd7b-132">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd7b-133">示例</span><span class="sxs-lookup"><span data-stu-id="acd7b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="acd7b-134">请求</span><span class="sxs-lookup"><span data-stu-id="acd7b-134">Request</span></span>
<span data-ttu-id="acd7b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="acd7b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="acd7b-136">响应</span><span class="sxs-lookup"><span data-stu-id="acd7b-136">Response</span></span>
<span data-ttu-id="acd7b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="acd7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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















