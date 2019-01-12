---
title: 获取 auditEvent
description: 读取 auditEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 675a4c29c2efd73e14c11d1e7ce4ef6e6b0917c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920938"
---
# <a name="get-auditevent"></a><span data-ttu-id="c25c4-103">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="c25c4-103">Get auditEvent</span></span>

> <span data-ttu-id="c25c4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c25c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c25c4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c25c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c25c4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c25c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c25c4-107">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c25c4-107">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c25c4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c25c4-108">Prerequisites</span></span>
<span data-ttu-id="c25c4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c25c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c25c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c25c4-111">Permission type</span></span>|<span data-ttu-id="c25c4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c25c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c25c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c25c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c25c4-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c25c4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c25c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c25c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c25c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c25c4-116">Not supported.</span></span>|
|<span data-ttu-id="c25c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c25c4-117">Application</span></span>|<span data-ttu-id="c25c4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c25c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c25c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c25c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c25c4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c25c4-120">Optional query parameters</span></span>
<span data-ttu-id="c25c4-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c25c4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c25c4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c25c4-122">Request headers</span></span>
|<span data-ttu-id="c25c4-123">标头</span><span class="sxs-lookup"><span data-stu-id="c25c4-123">Header</span></span>|<span data-ttu-id="c25c4-124">值</span><span class="sxs-lookup"><span data-stu-id="c25c4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c25c4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c25c4-125">Authorization</span></span>|<span data-ttu-id="c25c4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c25c4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c25c4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c25c4-127">Accept</span></span>|<span data-ttu-id="c25c4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c25c4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c25c4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c25c4-129">Request body</span></span>
<span data-ttu-id="c25c4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c25c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c25c4-131">响应</span><span class="sxs-lookup"><span data-stu-id="c25c4-131">Response</span></span>
<span data-ttu-id="c25c4-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c25c4-132">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c25c4-133">示例</span><span class="sxs-lookup"><span data-stu-id="c25c4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c25c4-134">请求</span><span class="sxs-lookup"><span data-stu-id="c25c4-134">Request</span></span>
<span data-ttu-id="c25c4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c25c4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="c25c4-136">响应</span><span class="sxs-lookup"><span data-stu-id="c25c4-136">Response</span></span>
<span data-ttu-id="c25c4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c25c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





