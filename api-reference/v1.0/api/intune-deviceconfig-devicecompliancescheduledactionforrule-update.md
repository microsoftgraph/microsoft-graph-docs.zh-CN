---
title: 更新 deviceComplianceScheduledActionForRule
description: 更新 deviceComplianceScheduledActionForRule 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad688779451f0320f7296ff91946ee1a7bcecb61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916416"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="20133-103">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="20133-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="20133-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20133-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20133-105">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20133-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20133-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="20133-106">Prerequisites</span></span>
<span data-ttu-id="20133-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="20133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20133-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20133-109">Permission type</span></span>|<span data-ttu-id="20133-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20133-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20133-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20133-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20133-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20133-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20133-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20133-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20133-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20133-114">Not supported.</span></span>|
|<span data-ttu-id="20133-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20133-115">Application</span></span>|<span data-ttu-id="20133-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20133-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20133-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20133-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="20133-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="20133-118">Request headers</span></span>
|<span data-ttu-id="20133-119">标头</span><span class="sxs-lookup"><span data-stu-id="20133-119">Header</span></span>|<span data-ttu-id="20133-120">值</span><span class="sxs-lookup"><span data-stu-id="20133-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20133-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20133-121">Authorization</span></span>|<span data-ttu-id="20133-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20133-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20133-123">Accept</span><span class="sxs-lookup"><span data-stu-id="20133-123">Accept</span></span>|<span data-ttu-id="20133-124">application/json</span><span class="sxs-lookup"><span data-stu-id="20133-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20133-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="20133-125">Request body</span></span>
<span data-ttu-id="20133-126">在请求正文中，提供 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20133-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="20133-127">下表显示创建 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20133-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="20133-128">属性</span><span class="sxs-lookup"><span data-stu-id="20133-128">Property</span></span>|<span data-ttu-id="20133-129">类型</span><span class="sxs-lookup"><span data-stu-id="20133-129">Type</span></span>|<span data-ttu-id="20133-130">说明</span><span class="sxs-lookup"><span data-stu-id="20133-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20133-131">id</span><span class="sxs-lookup"><span data-stu-id="20133-131">id</span></span>|<span data-ttu-id="20133-132">String</span><span class="sxs-lookup"><span data-stu-id="20133-132">String</span></span>|<span data-ttu-id="20133-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="20133-133">Key of the entity.</span></span>|
|<span data-ttu-id="20133-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="20133-134">ruleName</span></span>|<span data-ttu-id="20133-135">String</span><span class="sxs-lookup"><span data-stu-id="20133-135">String</span></span>|<span data-ttu-id="20133-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="20133-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="20133-137">响应</span><span class="sxs-lookup"><span data-stu-id="20133-137">Response</span></span>
<span data-ttu-id="20133-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20133-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20133-139">示例</span><span class="sxs-lookup"><span data-stu-id="20133-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="20133-140">请求</span><span class="sxs-lookup"><span data-stu-id="20133-140">Request</span></span>
<span data-ttu-id="20133-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20133-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="20133-142">响应</span><span class="sxs-lookup"><span data-stu-id="20133-142">Response</span></span>
<span data-ttu-id="20133-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20133-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



