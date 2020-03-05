---
title: 获取 deviceManagementExchangeOnPremisesPolicy
description: 读取 deviceManagementExchangeOnPremisesPolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43e259d622981c126936c513633fd0f9f0ac90fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462116"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="b5938-103">获取 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="b5938-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="b5938-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b5938-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5938-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5938-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5938-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5938-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5938-107">读取[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5938-107">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5938-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5938-108">Prerequisites</span></span>
<span data-ttu-id="b5938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5938-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5938-111">Permission type</span></span>|<span data-ttu-id="b5938-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5938-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5938-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5938-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5938-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5938-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b5938-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5938-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5938-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5938-116">Not supported.</span></span>|
|<span data-ttu-id="b5938-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5938-117">Application</span></span>|<span data-ttu-id="b5938-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5938-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5938-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5938-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5938-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5938-120">Optional query parameters</span></span>
<span data-ttu-id="b5938-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5938-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5938-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5938-122">Request headers</span></span>
|<span data-ttu-id="b5938-123">标头</span><span class="sxs-lookup"><span data-stu-id="b5938-123">Header</span></span>|<span data-ttu-id="b5938-124">值</span><span class="sxs-lookup"><span data-stu-id="b5938-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5938-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5938-125">Authorization</span></span>|<span data-ttu-id="b5938-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5938-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5938-127">接受</span><span class="sxs-lookup"><span data-stu-id="b5938-127">Accept</span></span>|<span data-ttu-id="b5938-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b5938-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5938-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5938-129">Request body</span></span>
<span data-ttu-id="b5938-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5938-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5938-131">响应</span><span class="sxs-lookup"><span data-stu-id="b5938-131">Response</span></span>
<span data-ttu-id="b5938-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5938-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5938-133">示例</span><span class="sxs-lookup"><span data-stu-id="b5938-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5938-134">请求</span><span class="sxs-lookup"><span data-stu-id="b5938-134">Request</span></span>
<span data-ttu-id="b5938-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5938-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="b5938-136">响应</span><span class="sxs-lookup"><span data-stu-id="b5938-136">Response</span></span>
<span data-ttu-id="b5938-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5938-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```





