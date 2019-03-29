---
title: 列出 deviceComplianceScheduledActionForRules
description: 列出 deviceComplianceScheduledActionForRule 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b255a4350ad4bd9009f8f377324ab41ea54167c6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984350"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="a3764-103">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="a3764-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="a3764-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3764-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3764-105">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3764-105">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3764-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3764-106">Prerequisites</span></span>
<span data-ttu-id="a3764-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3764-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3764-109">Permission type</span></span>|<span data-ttu-id="a3764-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3764-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3764-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3764-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3764-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3764-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3764-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3764-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3764-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3764-114">Not supported.</span></span>|
|<span data-ttu-id="a3764-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3764-115">Application</span></span>|<span data-ttu-id="a3764-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3764-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3764-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3764-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="a3764-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3764-118">Request headers</span></span>
|<span data-ttu-id="a3764-119">标头</span><span class="sxs-lookup"><span data-stu-id="a3764-119">Header</span></span>|<span data-ttu-id="a3764-120">值</span><span class="sxs-lookup"><span data-stu-id="a3764-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3764-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3764-121">Authorization</span></span>|<span data-ttu-id="a3764-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3764-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3764-123">接受</span><span class="sxs-lookup"><span data-stu-id="a3764-123">Accept</span></span>|<span data-ttu-id="a3764-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3764-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3764-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3764-125">Request body</span></span>
<span data-ttu-id="a3764-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3764-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3764-127">响应</span><span class="sxs-lookup"><span data-stu-id="a3764-127">Response</span></span>
<span data-ttu-id="a3764-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a3764-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3764-129">示例</span><span class="sxs-lookup"><span data-stu-id="a3764-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3764-130">请求</span><span class="sxs-lookup"><span data-stu-id="a3764-130">Request</span></span>
<span data-ttu-id="a3764-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3764-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="a3764-132">响应</span><span class="sxs-lookup"><span data-stu-id="a3764-132">Response</span></span>
<span data-ttu-id="a3764-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3764-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 208

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```



