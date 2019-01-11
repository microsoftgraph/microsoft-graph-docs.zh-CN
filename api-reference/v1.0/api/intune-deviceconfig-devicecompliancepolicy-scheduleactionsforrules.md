---
title: scheduleActionsForRules 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9516edaec94aaa62980f416d1ba5ccfc30bef743
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805234"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="bd95b-103">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="bd95b-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="bd95b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd95b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd95b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd95b-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd95b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd95b-106">Prerequisites</span></span>
<span data-ttu-id="bd95b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bd95b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd95b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd95b-109">Permission type</span></span>|<span data-ttu-id="bd95b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd95b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd95b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd95b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd95b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd95b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd95b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd95b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd95b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd95b-114">Not supported.</span></span>|
|<span data-ttu-id="bd95b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd95b-115">Application</span></span>|<span data-ttu-id="bd95b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd95b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd95b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd95b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="bd95b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd95b-118">Request headers</span></span>
|<span data-ttu-id="bd95b-119">标头</span><span class="sxs-lookup"><span data-stu-id="bd95b-119">Header</span></span>|<span data-ttu-id="bd95b-120">值</span><span class="sxs-lookup"><span data-stu-id="bd95b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd95b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd95b-121">Authorization</span></span>|<span data-ttu-id="bd95b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd95b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd95b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bd95b-123">Accept</span></span>|<span data-ttu-id="bd95b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd95b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd95b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd95b-125">Request body</span></span>
<span data-ttu-id="bd95b-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd95b-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bd95b-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="bd95b-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bd95b-128">属性</span><span class="sxs-lookup"><span data-stu-id="bd95b-128">Property</span></span>|<span data-ttu-id="bd95b-129">类型</span><span class="sxs-lookup"><span data-stu-id="bd95b-129">Type</span></span>|<span data-ttu-id="bd95b-130">说明</span><span class="sxs-lookup"><span data-stu-id="bd95b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd95b-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="bd95b-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="bd95b-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bd95b-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="bd95b-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd95b-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bd95b-134">响应</span><span class="sxs-lookup"><span data-stu-id="bd95b-134">Response</span></span>
<span data-ttu-id="bd95b-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd95b-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd95b-136">示例</span><span class="sxs-lookup"><span data-stu-id="bd95b-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd95b-137">请求</span><span class="sxs-lookup"><span data-stu-id="bd95b-137">Request</span></span>
<span data-ttu-id="bd95b-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd95b-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bd95b-139">响应</span><span class="sxs-lookup"><span data-stu-id="bd95b-139">Response</span></span>
<span data-ttu-id="bd95b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd95b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



