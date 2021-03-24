---
title: 创建 deviceComplianceScheduledActionForRule
description: 创建新的 deviceComplianceScheduledActionForRule 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f884c4168de0f8737552e7d3b367c7e60018058
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130152"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="1a382-103">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="1a382-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="1a382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a382-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a382-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a382-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a382-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a382-107">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a382-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a382-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a382-108">Prerequisites</span></span>
<span data-ttu-id="1a382-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a382-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a382-111">Permission type</span></span>|<span data-ttu-id="1a382-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a382-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a382-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a382-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a382-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a382-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a382-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a382-116">Not supported.</span></span>|
|<span data-ttu-id="1a382-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a382-117">Application</span></span>|<span data-ttu-id="1a382-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a382-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a382-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="1a382-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a382-120">Request headers</span></span>
|<span data-ttu-id="1a382-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a382-121">Header</span></span>|<span data-ttu-id="1a382-122">值</span><span class="sxs-lookup"><span data-stu-id="1a382-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a382-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a382-123">Authorization</span></span>|<span data-ttu-id="1a382-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a382-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a382-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a382-125">Accept</span></span>|<span data-ttu-id="1a382-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a382-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a382-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a382-127">Request body</span></span>
<span data-ttu-id="1a382-128">在请求正文中，提供 deviceComplianceScheduledActionForRule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a382-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="1a382-129">下表显示创建 deviceComplianceScheduledActionForRule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a382-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="1a382-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a382-130">Property</span></span>|<span data-ttu-id="1a382-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a382-131">Type</span></span>|<span data-ttu-id="1a382-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a382-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a382-133">id</span><span class="sxs-lookup"><span data-stu-id="1a382-133">id</span></span>|<span data-ttu-id="1a382-134">String</span><span class="sxs-lookup"><span data-stu-id="1a382-134">String</span></span>|<span data-ttu-id="1a382-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a382-135">Key of the entity.</span></span>|
|<span data-ttu-id="1a382-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="1a382-136">ruleName</span></span>|<span data-ttu-id="1a382-137">String</span><span class="sxs-lookup"><span data-stu-id="1a382-137">String</span></span>|<span data-ttu-id="1a382-138">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="1a382-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="1a382-139">响应</span><span class="sxs-lookup"><span data-stu-id="1a382-139">Response</span></span>
<span data-ttu-id="1a382-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a382-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a382-141">示例</span><span class="sxs-lookup"><span data-stu-id="1a382-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a382-142">请求</span><span class="sxs-lookup"><span data-stu-id="1a382-142">Request</span></span>
<span data-ttu-id="1a382-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a382-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="1a382-144">响应</span><span class="sxs-lookup"><span data-stu-id="1a382-144">Response</span></span>
<span data-ttu-id="1a382-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a382-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




