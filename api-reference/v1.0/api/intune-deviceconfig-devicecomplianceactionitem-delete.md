---
title: 删除 deviceComplianceActionItem
description: 删除 deviceComplianceActionItem。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bb5035969ef16f59cf31c571a526c838084ff7f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939313"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="d25ed-103">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="d25ed-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="d25ed-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d25ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d25ed-105">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d25ed-105">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d25ed-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d25ed-106">Prerequisites</span></span>
<span data-ttu-id="d25ed-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d25ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d25ed-109">Permission type</span></span>|<span data-ttu-id="d25ed-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d25ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d25ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d25ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d25ed-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25ed-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d25ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d25ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d25ed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d25ed-114">Not supported.</span></span>|
|<span data-ttu-id="d25ed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d25ed-115">Application</span></span>|<span data-ttu-id="d25ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d25ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d25ed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d25ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d25ed-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d25ed-118">Request headers</span></span>
|<span data-ttu-id="d25ed-119">标头</span><span class="sxs-lookup"><span data-stu-id="d25ed-119">Header</span></span>|<span data-ttu-id="d25ed-120">值</span><span class="sxs-lookup"><span data-stu-id="d25ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d25ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d25ed-121">Authorization</span></span>|<span data-ttu-id="d25ed-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d25ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d25ed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d25ed-123">Accept</span></span>|<span data-ttu-id="d25ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d25ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25ed-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d25ed-125">Request body</span></span>
<span data-ttu-id="d25ed-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d25ed-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d25ed-127">响应</span><span class="sxs-lookup"><span data-stu-id="d25ed-127">Response</span></span>
<span data-ttu-id="d25ed-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d25ed-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d25ed-129">示例</span><span class="sxs-lookup"><span data-stu-id="d25ed-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d25ed-130">请求</span><span class="sxs-lookup"><span data-stu-id="d25ed-130">Request</span></span>
<span data-ttu-id="d25ed-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d25ed-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="d25ed-132">响应</span><span class="sxs-lookup"><span data-stu-id="d25ed-132">Response</span></span>
<span data-ttu-id="d25ed-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d25ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



