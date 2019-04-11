---
title: 获取 auditEvent
description: 读取 auditEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac6fddfbb25cdaa0be4b2e2dc15481f8945f2069
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775364"
---
# <a name="get-auditevent"></a><span data-ttu-id="412e6-103">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="412e6-103">Get auditEvent</span></span>

> <span data-ttu-id="412e6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="412e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="412e6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="412e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="412e6-106">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="412e6-106">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="412e6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="412e6-107">Prerequisites</span></span>
<span data-ttu-id="412e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="412e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412e6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="412e6-110">Permission type</span></span>|<span data-ttu-id="412e6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="412e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="412e6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="412e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="412e6-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="412e6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="412e6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="412e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="412e6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="412e6-115">Not supported.</span></span>|
|<span data-ttu-id="412e6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="412e6-116">Application</span></span>|<span data-ttu-id="412e6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="412e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="412e6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="412e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="412e6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="412e6-119">Optional query parameters</span></span>
<span data-ttu-id="412e6-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="412e6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="412e6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="412e6-121">Request headers</span></span>
|<span data-ttu-id="412e6-122">标头</span><span class="sxs-lookup"><span data-stu-id="412e6-122">Header</span></span>|<span data-ttu-id="412e6-123">值</span><span class="sxs-lookup"><span data-stu-id="412e6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="412e6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="412e6-124">Authorization</span></span>|<span data-ttu-id="412e6-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="412e6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="412e6-126">接受</span><span class="sxs-lookup"><span data-stu-id="412e6-126">Accept</span></span>|<span data-ttu-id="412e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="412e6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="412e6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="412e6-128">Request body</span></span>
<span data-ttu-id="412e6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="412e6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="412e6-130">响应</span><span class="sxs-lookup"><span data-stu-id="412e6-130">Response</span></span>
<span data-ttu-id="412e6-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="412e6-131">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="412e6-132">示例</span><span class="sxs-lookup"><span data-stu-id="412e6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="412e6-133">请求</span><span class="sxs-lookup"><span data-stu-id="412e6-133">Request</span></span>
<span data-ttu-id="412e6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="412e6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="412e6-135">响应</span><span class="sxs-lookup"><span data-stu-id="412e6-135">Response</span></span>
<span data-ttu-id="412e6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="412e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





