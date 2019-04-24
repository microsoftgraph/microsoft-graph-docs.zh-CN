---
title: 创建 deviceComplianceScheduledActionForRule
description: 创建新的 deviceComplianceScheduledActionForRule 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e8d5093150871e747c44f4ee83d7a04e172e5ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32470403"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="9b543-103">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="9b543-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="9b543-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b543-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b543-106">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b543-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b543-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b543-107">Prerequisites</span></span>
<span data-ttu-id="9b543-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b543-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b543-110">Permission type</span></span>|<span data-ttu-id="9b543-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b543-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b543-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b543-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b543-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b543-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b543-115">Not supported.</span></span>|
|<span data-ttu-id="9b543-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b543-116">Application</span></span>|<span data-ttu-id="9b543-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b543-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b543-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="9b543-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b543-119">Request headers</span></span>
|<span data-ttu-id="9b543-120">标头</span><span class="sxs-lookup"><span data-stu-id="9b543-120">Header</span></span>|<span data-ttu-id="9b543-121">值</span><span class="sxs-lookup"><span data-stu-id="9b543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b543-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b543-122">Authorization</span></span>|<span data-ttu-id="9b543-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b543-124">接受</span><span class="sxs-lookup"><span data-stu-id="9b543-124">Accept</span></span>|<span data-ttu-id="9b543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b543-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b543-126">Request body</span></span>
<span data-ttu-id="9b543-127">在请求正文中，提供 deviceComplianceScheduledActionForRule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b543-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="9b543-128">下表显示创建 deviceComplianceScheduledActionForRule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b543-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="9b543-129">属性</span><span class="sxs-lookup"><span data-stu-id="9b543-129">Property</span></span>|<span data-ttu-id="9b543-130">类型</span><span class="sxs-lookup"><span data-stu-id="9b543-130">Type</span></span>|<span data-ttu-id="9b543-131">说明</span><span class="sxs-lookup"><span data-stu-id="9b543-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b543-132">id</span><span class="sxs-lookup"><span data-stu-id="9b543-132">id</span></span>|<span data-ttu-id="9b543-133">String</span><span class="sxs-lookup"><span data-stu-id="9b543-133">String</span></span>|<span data-ttu-id="9b543-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b543-134">Key of the entity.</span></span>|
|<span data-ttu-id="9b543-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="9b543-135">ruleName</span></span>|<span data-ttu-id="9b543-136">String</span><span class="sxs-lookup"><span data-stu-id="9b543-136">String</span></span>|<span data-ttu-id="9b543-137">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="9b543-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="9b543-138">响应</span><span class="sxs-lookup"><span data-stu-id="9b543-138">Response</span></span>
<span data-ttu-id="9b543-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b543-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b543-140">示例</span><span class="sxs-lookup"><span data-stu-id="9b543-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b543-141">请求</span><span class="sxs-lookup"><span data-stu-id="9b543-141">Request</span></span>
<span data-ttu-id="9b543-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b543-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="9b543-143">响应</span><span class="sxs-lookup"><span data-stu-id="9b543-143">Response</span></span>
<span data-ttu-id="9b543-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b543-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





