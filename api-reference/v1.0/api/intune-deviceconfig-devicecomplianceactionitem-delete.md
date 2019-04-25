---
title: 删除 deviceComplianceActionItem
description: 删除 deviceComplianceActionItem。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189152018478877b4ee61f437f1c160d0fad1234
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572680"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="25b99-103">删除 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="25b99-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="25b99-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25b99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b99-105">删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。</span><span class="sxs-lookup"><span data-stu-id="25b99-105">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25b99-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="25b99-106">Prerequisites</span></span>
<span data-ttu-id="25b99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b99-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25b99-109">Permission type</span></span>|<span data-ttu-id="25b99-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25b99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b99-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25b99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25b99-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b99-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25b99-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25b99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b99-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="25b99-114">Not supported.</span></span>|
|<span data-ttu-id="25b99-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="25b99-115">Application</span></span>|<span data-ttu-id="25b99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="25b99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b99-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25b99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="25b99-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25b99-118">Request headers</span></span>
|<span data-ttu-id="25b99-119">标头</span><span class="sxs-lookup"><span data-stu-id="25b99-119">Header</span></span>|<span data-ttu-id="25b99-120">值</span><span class="sxs-lookup"><span data-stu-id="25b99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25b99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b99-121">Authorization</span></span>|<span data-ttu-id="25b99-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25b99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25b99-123">接受</span><span class="sxs-lookup"><span data-stu-id="25b99-123">Accept</span></span>|<span data-ttu-id="25b99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25b99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b99-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="25b99-125">Request body</span></span>
<span data-ttu-id="25b99-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25b99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b99-127">响应</span><span class="sxs-lookup"><span data-stu-id="25b99-127">Response</span></span>
<span data-ttu-id="25b99-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25b99-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25b99-129">示例</span><span class="sxs-lookup"><span data-stu-id="25b99-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="25b99-130">请求</span><span class="sxs-lookup"><span data-stu-id="25b99-130">Request</span></span>
<span data-ttu-id="25b99-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25b99-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="25b99-132">响应</span><span class="sxs-lookup"><span data-stu-id="25b99-132">Response</span></span>
<span data-ttu-id="25b99-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25b99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



