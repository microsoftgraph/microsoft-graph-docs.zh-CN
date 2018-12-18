---
title: 列出 auditEvents
description: 列出 auditEvent 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: b4ef3d3993884c045428134c03b5097643b3b171
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309501"
---
# <a name="list-auditevents"></a><span data-ttu-id="dc73c-103">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="dc73c-103">List auditEvents</span></span>

> <span data-ttu-id="dc73c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dc73c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc73c-105">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc73c-105">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc73c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc73c-106">Prerequisites</span></span>
<span data-ttu-id="dc73c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="dc73c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc73c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc73c-109">Permission type</span></span>|<span data-ttu-id="dc73c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dc73c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc73c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc73c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc73c-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc73c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dc73c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc73c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc73c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc73c-114">Not supported.</span></span>|
|<span data-ttu-id="dc73c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc73c-115">Application</span></span>|<span data-ttu-id="dc73c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc73c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc73c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc73c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="dc73c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc73c-118">Request headers</span></span>
|<span data-ttu-id="dc73c-119">标头</span><span class="sxs-lookup"><span data-stu-id="dc73c-119">Header</span></span>|<span data-ttu-id="dc73c-120">值</span><span class="sxs-lookup"><span data-stu-id="dc73c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc73c-121">授权</span><span class="sxs-lookup"><span data-stu-id="dc73c-121">Authorization</span></span>|<span data-ttu-id="dc73c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc73c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc73c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc73c-123">Accept</span></span>|<span data-ttu-id="dc73c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc73c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc73c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc73c-125">Request body</span></span>
<span data-ttu-id="dc73c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc73c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc73c-127">响应</span><span class="sxs-lookup"><span data-stu-id="dc73c-127">Response</span></span>
<span data-ttu-id="dc73c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dc73c-128">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc73c-129">示例</span><span class="sxs-lookup"><span data-stu-id="dc73c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc73c-130">请求</span><span class="sxs-lookup"><span data-stu-id="dc73c-130">Request</span></span>
<span data-ttu-id="dc73c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc73c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="dc73c-132">响应</span><span class="sxs-lookup"><span data-stu-id="dc73c-132">Response</span></span>
<span data-ttu-id="dc73c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc73c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
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
  ]
}
```



