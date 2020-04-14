---
title: 更新 deviceComplianceScheduledActionForRule
description: 更新 deviceComplianceScheduledActionForRule 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c28275e5ddbaf0ce0720c5da54902313fbf345df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433867"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="5a5b1-103">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="5a5b1-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="5a5b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a5b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a5b1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a5b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a5b1-107">更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a5b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a5b1-108">Prerequisites</span></span>
<span data-ttu-id="5a5b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a5b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a5b1-111">Permission type</span></span>|<span data-ttu-id="5a5b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a5b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a5b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a5b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a5b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a5b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a5b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a5b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a5b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-116">Not supported.</span></span>|
|<span data-ttu-id="5a5b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a5b1-117">Application</span></span>|<span data-ttu-id="5a5b1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a5b1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a5b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a5b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="5a5b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a5b1-120">Request headers</span></span>
|<span data-ttu-id="5a5b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="5a5b1-121">Header</span></span>|<span data-ttu-id="5a5b1-122">值</span><span class="sxs-lookup"><span data-stu-id="5a5b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a5b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a5b1-123">Authorization</span></span>|<span data-ttu-id="5a5b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a5b1-125">接受</span><span class="sxs-lookup"><span data-stu-id="5a5b1-125">Accept</span></span>|<span data-ttu-id="5a5b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a5b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a5b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a5b1-127">Request body</span></span>
<span data-ttu-id="5a5b1-128">在请求正文中，提供 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="5a5b1-129">下表显示创建 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="5a5b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="5a5b1-130">Property</span></span>|<span data-ttu-id="5a5b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="5a5b1-131">Type</span></span>|<span data-ttu-id="5a5b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="5a5b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a5b1-133">id</span><span class="sxs-lookup"><span data-stu-id="5a5b1-133">id</span></span>|<span data-ttu-id="5a5b1-134">String</span><span class="sxs-lookup"><span data-stu-id="5a5b1-134">String</span></span>|<span data-ttu-id="5a5b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-135">Key of the entity.</span></span>|
|<span data-ttu-id="5a5b1-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="5a5b1-136">ruleName</span></span>|<span data-ttu-id="5a5b1-137">String</span><span class="sxs-lookup"><span data-stu-id="5a5b1-137">String</span></span>|<span data-ttu-id="5a5b1-138">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="5a5b1-139">响应</span><span class="sxs-lookup"><span data-stu-id="5a5b1-139">Response</span></span>
<span data-ttu-id="5a5b1-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a5b1-141">示例</span><span class="sxs-lookup"><span data-stu-id="5a5b1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a5b1-142">请求</span><span class="sxs-lookup"><span data-stu-id="5a5b1-142">Request</span></span>
<span data-ttu-id="5a5b1-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="5a5b1-144">响应</span><span class="sxs-lookup"><span data-stu-id="5a5b1-144">Response</span></span>
<span data-ttu-id="5a5b1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a5b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



