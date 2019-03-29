---
title: scheduleActionsForRules 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced79558b7a106e57468cacd7db2e2bd5ae97bc5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963105"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="bd53b-103">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="bd53b-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="bd53b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd53b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd53b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd53b-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd53b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd53b-106">Prerequisites</span></span>
<span data-ttu-id="bd53b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd53b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd53b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd53b-109">Permission type</span></span>|<span data-ttu-id="bd53b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd53b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd53b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd53b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd53b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd53b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd53b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd53b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd53b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd53b-114">Not supported.</span></span>|
|<span data-ttu-id="bd53b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd53b-115">Application</span></span>|<span data-ttu-id="bd53b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd53b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd53b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd53b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="bd53b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd53b-118">Request headers</span></span>
|<span data-ttu-id="bd53b-119">标头</span><span class="sxs-lookup"><span data-stu-id="bd53b-119">Header</span></span>|<span data-ttu-id="bd53b-120">值</span><span class="sxs-lookup"><span data-stu-id="bd53b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd53b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd53b-121">Authorization</span></span>|<span data-ttu-id="bd53b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd53b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd53b-123">接受</span><span class="sxs-lookup"><span data-stu-id="bd53b-123">Accept</span></span>|<span data-ttu-id="bd53b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd53b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd53b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd53b-125">Request body</span></span>
<span data-ttu-id="bd53b-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd53b-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bd53b-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="bd53b-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bd53b-128">属性</span><span class="sxs-lookup"><span data-stu-id="bd53b-128">Property</span></span>|<span data-ttu-id="bd53b-129">类型</span><span class="sxs-lookup"><span data-stu-id="bd53b-129">Type</span></span>|<span data-ttu-id="bd53b-130">说明</span><span class="sxs-lookup"><span data-stu-id="bd53b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd53b-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="bd53b-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="bd53b-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bd53b-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="bd53b-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bd53b-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bd53b-134">响应</span><span class="sxs-lookup"><span data-stu-id="bd53b-134">Response</span></span>
<span data-ttu-id="bd53b-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd53b-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd53b-136">示例</span><span class="sxs-lookup"><span data-stu-id="bd53b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd53b-137">请求</span><span class="sxs-lookup"><span data-stu-id="bd53b-137">Request</span></span>
<span data-ttu-id="bd53b-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd53b-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd53b-139">响应</span><span class="sxs-lookup"><span data-stu-id="bd53b-139">Response</span></span>
<span data-ttu-id="bd53b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd53b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



