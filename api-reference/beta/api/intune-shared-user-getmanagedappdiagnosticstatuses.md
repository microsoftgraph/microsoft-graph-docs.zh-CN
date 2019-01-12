---
title: getManagedAppDiagnosticStatuses 函数
description: 获取给定用户的诊断验证状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cb8beac36b1f0892164fad41de4bdc11aee00094
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939887"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="43b8d-103">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="43b8d-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="43b8d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="43b8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43b8d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="43b8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43b8d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="43b8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43b8d-107">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="43b8d-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43b8d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43b8d-108">Prerequisites</span></span>
<span data-ttu-id="43b8d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="43b8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b8d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43b8d-111">Permission type</span></span>|<span data-ttu-id="43b8d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43b8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43b8d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43b8d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="43b8d-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="43b8d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="43b8d-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43b8d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43b8d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43b8d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43b8d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="43b8d-117">Not supported.</span></span>|
|<span data-ttu-id="43b8d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="43b8d-118">Application</span></span>|<span data-ttu-id="43b8d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="43b8d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43b8d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43b8d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="43b8d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="43b8d-121">Request headers</span></span>
|<span data-ttu-id="43b8d-122">标头</span><span class="sxs-lookup"><span data-stu-id="43b8d-122">Header</span></span>|<span data-ttu-id="43b8d-123">值</span><span class="sxs-lookup"><span data-stu-id="43b8d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43b8d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43b8d-124">Authorization</span></span>|<span data-ttu-id="43b8d-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43b8d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43b8d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="43b8d-126">Accept</span></span>|<span data-ttu-id="43b8d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="43b8d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b8d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="43b8d-128">Request body</span></span>
<span data-ttu-id="43b8d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43b8d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43b8d-130">响应</span><span class="sxs-lookup"><span data-stu-id="43b8d-130">Response</span></span>
<span data-ttu-id="43b8d-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="43b8d-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43b8d-132">示例</span><span class="sxs-lookup"><span data-stu-id="43b8d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="43b8d-133">请求</span><span class="sxs-lookup"><span data-stu-id="43b8d-133">Request</span></span>
<span data-ttu-id="43b8d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43b8d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="43b8d-135">响应</span><span class="sxs-lookup"><span data-stu-id="43b8d-135">Response</span></span>
<span data-ttu-id="43b8d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43b8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






