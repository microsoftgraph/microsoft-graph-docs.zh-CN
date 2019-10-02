---
title: 获取 deviceComplianceActionItem
description: 读取 deviceComplianceActionItem 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea02bc0768272fc2501959d04623ee7c2b6309ba
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354355"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="3c258-103">获取 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="3c258-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="3c258-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c258-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c258-105">读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c258-105">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c258-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c258-106">Prerequisites</span></span>
<span data-ttu-id="3c258-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c258-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c258-109">Permission type</span></span>|<span data-ttu-id="3c258-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c258-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c258-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c258-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c258-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c258-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c258-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c258-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c258-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c258-114">Not supported.</span></span>|
|<span data-ttu-id="3c258-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c258-115">Application</span></span>|<span data-ttu-id="3c258-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c258-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c258-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c258-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c258-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c258-118">Optional query parameters</span></span>
<span data-ttu-id="3c258-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c258-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c258-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c258-120">Request headers</span></span>
|<span data-ttu-id="3c258-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c258-121">Header</span></span>|<span data-ttu-id="3c258-122">值</span><span class="sxs-lookup"><span data-stu-id="3c258-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c258-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c258-123">Authorization</span></span>|<span data-ttu-id="3c258-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c258-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c258-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c258-125">Accept</span></span>|<span data-ttu-id="3c258-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c258-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c258-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c258-127">Request body</span></span>
<span data-ttu-id="3c258-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c258-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c258-129">响应</span><span class="sxs-lookup"><span data-stu-id="3c258-129">Response</span></span>
<span data-ttu-id="3c258-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c258-130">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c258-131">示例</span><span class="sxs-lookup"><span data-stu-id="3c258-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c258-132">请求</span><span class="sxs-lookup"><span data-stu-id="3c258-132">Request</span></span>
<span data-ttu-id="3c258-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c258-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="3c258-134">响应</span><span class="sxs-lookup"><span data-stu-id="3c258-134">Response</span></span>
<span data-ttu-id="3c258-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c258-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```




