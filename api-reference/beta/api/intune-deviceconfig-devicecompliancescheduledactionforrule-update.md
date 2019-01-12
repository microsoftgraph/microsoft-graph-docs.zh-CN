---
title: 更新 deviceComplianceScheduledActionForRule
description: 更新 deviceComplianceScheduledActionForRule 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: adccf54c589fdaed64da8edae191b56fd48fde5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953845"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="12c7b-103">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="12c7b-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="12c7b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12c7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12c7b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12c7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12c7b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12c7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12c7b-107">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12c7b-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12c7b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12c7b-108">Prerequisites</span></span>
<span data-ttu-id="12c7b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="12c7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c7b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12c7b-111">Permission type</span></span>|<span data-ttu-id="12c7b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12c7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c7b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12c7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12c7b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c7b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12c7b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12c7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c7b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c7b-116">Not supported.</span></span>|
|<span data-ttu-id="12c7b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12c7b-117">Application</span></span>|<span data-ttu-id="12c7b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c7b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12c7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="12c7b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12c7b-120">Request headers</span></span>
|<span data-ttu-id="12c7b-121">标头</span><span class="sxs-lookup"><span data-stu-id="12c7b-121">Header</span></span>|<span data-ttu-id="12c7b-122">值</span><span class="sxs-lookup"><span data-stu-id="12c7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c7b-123">Authorization</span></span>|<span data-ttu-id="12c7b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12c7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12c7b-125">Accept</span></span>|<span data-ttu-id="12c7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12c7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c7b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12c7b-127">Request body</span></span>
<span data-ttu-id="12c7b-128">在请求正文中，提供 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12c7b-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="12c7b-129">下表显示创建 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12c7b-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="12c7b-130">属性</span><span class="sxs-lookup"><span data-stu-id="12c7b-130">Property</span></span>|<span data-ttu-id="12c7b-131">类型</span><span class="sxs-lookup"><span data-stu-id="12c7b-131">Type</span></span>|<span data-ttu-id="12c7b-132">说明</span><span class="sxs-lookup"><span data-stu-id="12c7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c7b-133">id</span><span class="sxs-lookup"><span data-stu-id="12c7b-133">id</span></span>|<span data-ttu-id="12c7b-134">String</span><span class="sxs-lookup"><span data-stu-id="12c7b-134">String</span></span>|<span data-ttu-id="12c7b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12c7b-135">Key of the entity.</span></span>|
|<span data-ttu-id="12c7b-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="12c7b-136">ruleName</span></span>|<span data-ttu-id="12c7b-137">String</span><span class="sxs-lookup"><span data-stu-id="12c7b-137">String</span></span>|<span data-ttu-id="12c7b-138">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="12c7b-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="12c7b-139">响应</span><span class="sxs-lookup"><span data-stu-id="12c7b-139">Response</span></span>
<span data-ttu-id="12c7b-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12c7b-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c7b-141">示例</span><span class="sxs-lookup"><span data-stu-id="12c7b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="12c7b-142">请求</span><span class="sxs-lookup"><span data-stu-id="12c7b-142">Request</span></span>
<span data-ttu-id="12c7b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12c7b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="12c7b-144">响应</span><span class="sxs-lookup"><span data-stu-id="12c7b-144">Response</span></span>
<span data-ttu-id="12c7b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12c7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





