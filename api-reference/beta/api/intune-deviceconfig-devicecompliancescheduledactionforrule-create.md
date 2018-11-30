---
title: 创建 deviceComplianceScheduledActionForRule
description: 创建新的 deviceComplianceScheduledActionForRule 对象。
ms.openlocfilehash: 29a20c0fe1246c86abffe6b59e6fd325211a2e14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042206"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="7fded-103">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="7fded-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="7fded-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7fded-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fded-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7fded-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fded-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7fded-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fded-107">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fded-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fded-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7fded-108">Prerequisites</span></span>
<span data-ttu-id="7fded-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7fded-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fded-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fded-111">Permission type</span></span>|<span data-ttu-id="7fded-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7fded-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fded-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fded-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fded-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fded-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7fded-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fded-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fded-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fded-116">Not supported.</span></span>|
|<span data-ttu-id="7fded-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fded-117">Application</span></span>|<span data-ttu-id="7fded-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fded-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fded-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fded-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="7fded-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fded-120">Request headers</span></span>
|<span data-ttu-id="7fded-121">标头</span><span class="sxs-lookup"><span data-stu-id="7fded-121">Header</span></span>|<span data-ttu-id="7fded-122">值</span><span class="sxs-lookup"><span data-stu-id="7fded-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fded-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fded-123">Authorization</span></span>|<span data-ttu-id="7fded-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7fded-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fded-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fded-125">Accept</span></span>|<span data-ttu-id="7fded-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fded-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fded-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fded-127">Request body</span></span>
<span data-ttu-id="7fded-128">在请求正文中，提供 deviceComplianceScheduledActionForRule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fded-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="7fded-129">下表显示创建 deviceComplianceScheduledActionForRule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7fded-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="7fded-130">属性</span><span class="sxs-lookup"><span data-stu-id="7fded-130">Property</span></span>|<span data-ttu-id="7fded-131">类型</span><span class="sxs-lookup"><span data-stu-id="7fded-131">Type</span></span>|<span data-ttu-id="7fded-132">说明</span><span class="sxs-lookup"><span data-stu-id="7fded-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fded-133">id</span><span class="sxs-lookup"><span data-stu-id="7fded-133">id</span></span>|<span data-ttu-id="7fded-134">String</span><span class="sxs-lookup"><span data-stu-id="7fded-134">String</span></span>|<span data-ttu-id="7fded-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fded-135">Key of the entity.</span></span>|
|<span data-ttu-id="7fded-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="7fded-136">ruleName</span></span>|<span data-ttu-id="7fded-137">String</span><span class="sxs-lookup"><span data-stu-id="7fded-137">String</span></span>|<span data-ttu-id="7fded-138">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="7fded-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="7fded-139">响应</span><span class="sxs-lookup"><span data-stu-id="7fded-139">Response</span></span>
<span data-ttu-id="7fded-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fded-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fded-141">示例</span><span class="sxs-lookup"><span data-stu-id="7fded-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fded-142">请求</span><span class="sxs-lookup"><span data-stu-id="7fded-142">Request</span></span>
<span data-ttu-id="7fded-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fded-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="7fded-144">响应</span><span class="sxs-lookup"><span data-stu-id="7fded-144">Response</span></span>
<span data-ttu-id="7fded-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fded-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```





