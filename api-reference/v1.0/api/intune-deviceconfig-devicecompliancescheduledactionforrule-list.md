---
title: 列出 deviceComplianceScheduledActionForRules
description: 列出 deviceComplianceScheduledActionForRule 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 32c5b75f9d0d2af699a3ed8f41e6294e43e49c12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965234"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="65e29-103">列出 deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="65e29-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="65e29-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="65e29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65e29-105">列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65e29-105">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65e29-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="65e29-106">Prerequisites</span></span>
<span data-ttu-id="65e29-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="65e29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e29-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65e29-109">Permission type</span></span>|<span data-ttu-id="65e29-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65e29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e29-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65e29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65e29-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65e29-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="65e29-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65e29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e29-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65e29-114">Not supported.</span></span>|
|<span data-ttu-id="65e29-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65e29-115">Application</span></span>|<span data-ttu-id="65e29-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65e29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e29-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65e29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="65e29-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65e29-118">Request headers</span></span>
|<span data-ttu-id="65e29-119">标头</span><span class="sxs-lookup"><span data-stu-id="65e29-119">Header</span></span>|<span data-ttu-id="65e29-120">值</span><span class="sxs-lookup"><span data-stu-id="65e29-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e29-121">Authorization</span></span>|<span data-ttu-id="65e29-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65e29-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e29-123">Accept</span><span class="sxs-lookup"><span data-stu-id="65e29-123">Accept</span></span>|<span data-ttu-id="65e29-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65e29-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e29-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="65e29-125">Request body</span></span>
<span data-ttu-id="65e29-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65e29-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65e29-127">响应</span><span class="sxs-lookup"><span data-stu-id="65e29-127">Response</span></span>
<span data-ttu-id="65e29-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="65e29-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e29-129">示例</span><span class="sxs-lookup"><span data-stu-id="65e29-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="65e29-130">请求</span><span class="sxs-lookup"><span data-stu-id="65e29-130">Request</span></span>
<span data-ttu-id="65e29-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65e29-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="65e29-132">响应</span><span class="sxs-lookup"><span data-stu-id="65e29-132">Response</span></span>
<span data-ttu-id="65e29-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65e29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



