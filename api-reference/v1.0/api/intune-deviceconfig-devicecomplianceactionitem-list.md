---
title: 列出 deviceComplianceActionItems
description: 列出 deviceComplianceActionItem 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c1dd0a71844d071c191c58297f683f5ff629af5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839198"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="2ab2c-103">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="2ab2c-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="2ab2c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab2c-105">列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-105">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ab2c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ab2c-106">Prerequisites</span></span>
<span data-ttu-id="2ab2c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2ab2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab2c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ab2c-109">Permission type</span></span>|<span data-ttu-id="2ab2c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ab2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab2c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ab2c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab2c-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab2c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ab2c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ab2c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab2c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-114">Not supported.</span></span>|
|<span data-ttu-id="2ab2c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ab2c-115">Application</span></span>|<span data-ttu-id="2ab2c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab2c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ab2c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2ab2c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ab2c-118">Request headers</span></span>
|<span data-ttu-id="2ab2c-119">标头</span><span class="sxs-lookup"><span data-stu-id="2ab2c-119">Header</span></span>|<span data-ttu-id="2ab2c-120">值</span><span class="sxs-lookup"><span data-stu-id="2ab2c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab2c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ab2c-121">Authorization</span></span>|<span data-ttu-id="2ab2c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab2c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2ab2c-123">Accept</span></span>|<span data-ttu-id="2ab2c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab2c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab2c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ab2c-125">Request body</span></span>
<span data-ttu-id="2ab2c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab2c-127">响应</span><span class="sxs-lookup"><span data-stu-id="2ab2c-127">Response</span></span>
<span data-ttu-id="2ab2c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab2c-129">示例</span><span class="sxs-lookup"><span data-stu-id="2ab2c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ab2c-130">请求</span><span class="sxs-lookup"><span data-stu-id="2ab2c-130">Request</span></span>
<span data-ttu-id="2ab2c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="2ab2c-132">响应</span><span class="sxs-lookup"><span data-stu-id="2ab2c-132">Response</span></span>
<span data-ttu-id="2ab2c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ab2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
      "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
      "gracePeriodHours": 0,
      "actionType": "notification",
      "notificationTemplateId": "Notification Template Id value",
      "notificationMessageCCList": [
        "Notification Message CCList value"
      ]
    }
  ]
}
```



