---
title: scheduleActionsForRules 操作
description: 尚未记录
ms.openlocfilehash: 9b51c826d6b31a51ac97d52daf23f9dc9cb18985
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046768"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="fe734-103">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="fe734-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="fe734-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe734-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe734-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe734-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe734-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fe734-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe734-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe734-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe734-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe734-108">Prerequisites</span></span>
<span data-ttu-id="fe734-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fe734-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe734-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe734-111">Permission type</span></span>|<span data-ttu-id="fe734-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe734-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe734-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe734-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe734-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe734-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe734-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe734-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe734-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe734-116">Not supported.</span></span>|
|<span data-ttu-id="fe734-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe734-117">Application</span></span>|<span data-ttu-id="fe734-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe734-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe734-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe734-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="fe734-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe734-120">Request headers</span></span>
|<span data-ttu-id="fe734-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe734-121">Header</span></span>|<span data-ttu-id="fe734-122">值</span><span class="sxs-lookup"><span data-stu-id="fe734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe734-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe734-123">Authorization</span></span>|<span data-ttu-id="fe734-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe734-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe734-125">Accept</span></span>|<span data-ttu-id="fe734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe734-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe734-127">Request body</span></span>
<span data-ttu-id="fe734-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe734-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fe734-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fe734-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fe734-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe734-130">Property</span></span>|<span data-ttu-id="fe734-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe734-131">Type</span></span>|<span data-ttu-id="fe734-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe734-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe734-133">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="fe734-133">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="fe734-134">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe734-134">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="fe734-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe734-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fe734-136">响应</span><span class="sxs-lookup"><span data-stu-id="fe734-136">Response</span></span>
<span data-ttu-id="fe734-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fe734-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe734-138">示例</span><span class="sxs-lookup"><span data-stu-id="fe734-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe734-139">请求</span><span class="sxs-lookup"><span data-stu-id="fe734-139">Request</span></span>
<span data-ttu-id="fe734-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe734-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

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

### <a name="response"></a><span data-ttu-id="fe734-141">响应</span><span class="sxs-lookup"><span data-stu-id="fe734-141">Response</span></span>
<span data-ttu-id="fe734-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe734-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





