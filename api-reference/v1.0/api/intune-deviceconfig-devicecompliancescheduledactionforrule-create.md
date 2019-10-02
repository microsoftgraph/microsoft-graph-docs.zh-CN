---
title: 创建 deviceComplianceScheduledActionForRule
description: 创建新的 deviceComplianceScheduledActionForRule 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67f97922e9ad978712d431f45393363a4b62bb4a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359752"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="0f86d-103">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="0f86d-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="0f86d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f86d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f86d-105">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f86d-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f86d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f86d-106">Prerequisites</span></span>
<span data-ttu-id="0f86d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f86d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f86d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f86d-109">Permission type</span></span>|<span data-ttu-id="0f86d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f86d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f86d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f86d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f86d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f86d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f86d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f86d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f86d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f86d-114">Not supported.</span></span>|
|<span data-ttu-id="0f86d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f86d-115">Application</span></span>|<span data-ttu-id="0f86d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f86d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f86d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f86d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="0f86d-118">请求头</span><span class="sxs-lookup"><span data-stu-id="0f86d-118">Request headers</span></span>
|<span data-ttu-id="0f86d-119">标头</span><span class="sxs-lookup"><span data-stu-id="0f86d-119">Header</span></span>|<span data-ttu-id="0f86d-120">值</span><span class="sxs-lookup"><span data-stu-id="0f86d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f86d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f86d-121">Authorization</span></span>|<span data-ttu-id="0f86d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f86d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f86d-123">接受</span><span class="sxs-lookup"><span data-stu-id="0f86d-123">Accept</span></span>|<span data-ttu-id="0f86d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f86d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f86d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f86d-125">Request body</span></span>
<span data-ttu-id="0f86d-126">在请求正文中，提供 deviceComplianceScheduledActionForRule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f86d-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="0f86d-127">下表显示创建 deviceComplianceScheduledActionForRule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f86d-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="0f86d-128">属性</span><span class="sxs-lookup"><span data-stu-id="0f86d-128">Property</span></span>|<span data-ttu-id="0f86d-129">类型</span><span class="sxs-lookup"><span data-stu-id="0f86d-129">Type</span></span>|<span data-ttu-id="0f86d-130">说明</span><span class="sxs-lookup"><span data-stu-id="0f86d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f86d-131">id</span><span class="sxs-lookup"><span data-stu-id="0f86d-131">id</span></span>|<span data-ttu-id="0f86d-132">String</span><span class="sxs-lookup"><span data-stu-id="0f86d-132">String</span></span>|<span data-ttu-id="0f86d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f86d-133">Key of the entity.</span></span>|
|<span data-ttu-id="0f86d-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="0f86d-134">ruleName</span></span>|<span data-ttu-id="0f86d-135">String</span><span class="sxs-lookup"><span data-stu-id="0f86d-135">String</span></span>|<span data-ttu-id="0f86d-136">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="0f86d-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="0f86d-137">响应</span><span class="sxs-lookup"><span data-stu-id="0f86d-137">Response</span></span>
<span data-ttu-id="0f86d-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f86d-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f86d-139">示例</span><span class="sxs-lookup"><span data-stu-id="0f86d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f86d-140">请求</span><span class="sxs-lookup"><span data-stu-id="0f86d-140">Request</span></span>
<span data-ttu-id="0f86d-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f86d-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="0f86d-142">响应</span><span class="sxs-lookup"><span data-stu-id="0f86d-142">Response</span></span>
<span data-ttu-id="0f86d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f86d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




