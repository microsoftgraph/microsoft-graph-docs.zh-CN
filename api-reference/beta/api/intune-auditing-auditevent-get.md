---
title: 获取 auditEvent
description: 读取 auditEvent 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0d3e0450a80bc2b0932fda3143d14d46e30fb89
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421030"
---
# <a name="get-auditevent"></a><span data-ttu-id="ded93-103">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="ded93-103">Get auditEvent</span></span>

> <span data-ttu-id="ded93-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ded93-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ded93-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ded93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ded93-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ded93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded93-107">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ded93-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ded93-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ded93-108">Prerequisites</span></span>
<span data-ttu-id="ded93-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ded93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ded93-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ded93-111">Permission type</span></span>|<span data-ttu-id="ded93-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ded93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ded93-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ded93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ded93-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ded93-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ded93-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ded93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ded93-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ded93-116">Not supported.</span></span>|
|<span data-ttu-id="ded93-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ded93-117">Application</span></span>|<span data-ttu-id="ded93-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ded93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ded93-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ded93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ded93-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ded93-120">Optional query parameters</span></span>
<span data-ttu-id="ded93-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ded93-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ded93-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ded93-122">Request headers</span></span>
|<span data-ttu-id="ded93-123">标头</span><span class="sxs-lookup"><span data-stu-id="ded93-123">Header</span></span>|<span data-ttu-id="ded93-124">值</span><span class="sxs-lookup"><span data-stu-id="ded93-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ded93-125">授权</span><span class="sxs-lookup"><span data-stu-id="ded93-125">Authorization</span></span>|<span data-ttu-id="ded93-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ded93-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ded93-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ded93-127">Accept</span></span>|<span data-ttu-id="ded93-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ded93-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ded93-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ded93-129">Request body</span></span>
<span data-ttu-id="ded93-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ded93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ded93-131">响应</span><span class="sxs-lookup"><span data-stu-id="ded93-131">Response</span></span>
<span data-ttu-id="ded93-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ded93-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ded93-133">示例</span><span class="sxs-lookup"><span data-stu-id="ded93-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ded93-134">请求</span><span class="sxs-lookup"><span data-stu-id="ded93-134">Request</span></span>
<span data-ttu-id="ded93-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ded93-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="ded93-136">响应</span><span class="sxs-lookup"><span data-stu-id="ded93-136">Response</span></span>
<span data-ttu-id="ded93-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ded93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




