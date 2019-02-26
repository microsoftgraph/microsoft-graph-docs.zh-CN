---
title: 获取 auditEvent
description: 读取 auditEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a97f8e774d7f3ccb855ff8f9c923bbc8109581f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255120"
---
# <a name="get-auditevent"></a><span data-ttu-id="9c1f9-103">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="9c1f9-103">Get auditEvent</span></span>

> <span data-ttu-id="9c1f9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1f9-105">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c1f9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c1f9-106">Prerequisites</span></span>
<span data-ttu-id="9c1f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9c1f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c1f9-109">Permission type</span></span>|<span data-ttu-id="9c1f9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c1f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1f9-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1f9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9c1f9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1f9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-114">Not supported.</span></span>|
|<span data-ttu-id="9c1f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c1f9-115">Application</span></span>|<span data-ttu-id="9c1f9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c1f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c1f9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9c1f9-118">Optional query parameters</span></span>
<span data-ttu-id="9c1f9-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c1f9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c1f9-120">Request headers</span></span>
|<span data-ttu-id="9c1f9-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c1f9-121">Header</span></span>|<span data-ttu-id="9c1f9-122">值</span><span class="sxs-lookup"><span data-stu-id="9c1f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c1f9-123">Authorization</span></span>|<span data-ttu-id="9c1f9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c1f9-125">Accept</span></span>|<span data-ttu-id="9c1f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1f9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c1f9-127">Request body</span></span>
<span data-ttu-id="9c1f9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c1f9-129">响应</span><span class="sxs-lookup"><span data-stu-id="9c1f9-129">Response</span></span>
<span data-ttu-id="9c1f9-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1f9-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c1f9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c1f9-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c1f9-132">Request</span></span>
<span data-ttu-id="9c1f9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="9c1f9-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c1f9-134">Response</span></span>
<span data-ttu-id="9c1f9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c1f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value"
    },
    "activity": "Activity value",
    "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "displayName": "Display Name value",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "displayName": "Display Name value",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "type": "Type value",
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```



