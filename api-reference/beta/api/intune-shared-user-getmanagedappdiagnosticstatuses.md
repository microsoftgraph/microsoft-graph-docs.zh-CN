---
title: getManagedAppDiagnosticStatuses 函数
description: 获取给定用户的诊断验证状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c3930dd8e70deb2324fbb6e95694cf0be9a05c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447505"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="4719b-103">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="4719b-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="4719b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4719b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4719b-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4719b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4719b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4719b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4719b-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4719b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4719b-108">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="4719b-108">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4719b-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="4719b-109">Prerequisites</span></span>
<span data-ttu-id="4719b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4719b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4719b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4719b-112">Permission type</span></span>|<span data-ttu-id="4719b-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4719b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4719b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4719b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4719b-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4719b-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4719b-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4719b-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4719b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4719b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4719b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4719b-118">Not supported.</span></span>|
|<span data-ttu-id="4719b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4719b-119">Application</span></span>||
| <span data-ttu-id="4719b-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4719b-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4719b-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4719b-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4719b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4719b-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4719b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4719b-123">Request headers</span></span>
|<span data-ttu-id="4719b-124">标头</span><span class="sxs-lookup"><span data-stu-id="4719b-124">Header</span></span>|<span data-ttu-id="4719b-125">值</span><span class="sxs-lookup"><span data-stu-id="4719b-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4719b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4719b-126">Authorization</span></span>|<span data-ttu-id="4719b-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4719b-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4719b-128">接受</span><span class="sxs-lookup"><span data-stu-id="4719b-128">Accept</span></span>|<span data-ttu-id="4719b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4719b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4719b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4719b-130">Request body</span></span>
<span data-ttu-id="4719b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4719b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4719b-132">响应</span><span class="sxs-lookup"><span data-stu-id="4719b-132">Response</span></span>
<span data-ttu-id="4719b-133">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4719b-133">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4719b-134">示例</span><span class="sxs-lookup"><span data-stu-id="4719b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="4719b-135">请求</span><span class="sxs-lookup"><span data-stu-id="4719b-135">Request</span></span>
<span data-ttu-id="4719b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4719b-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="4719b-137">响应</span><span class="sxs-lookup"><span data-stu-id="4719b-137">Response</span></span>
<span data-ttu-id="4719b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4719b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












