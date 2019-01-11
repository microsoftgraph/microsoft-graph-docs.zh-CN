---
title: 列出 auditEvents
description: 列出 auditEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f3587dc98dd074a9ac6e92730870bbbaf7f24ff1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863817"
---
# <a name="list-auditevents"></a><span data-ttu-id="f3f39-103">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="f3f39-103">List auditEvents</span></span>

> <span data-ttu-id="f3f39-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3f39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3f39-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3f39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3f39-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f3f39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3f39-107">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f3f39-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3f39-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3f39-108">Prerequisites</span></span>
<span data-ttu-id="f3f39-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f3f39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3f39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3f39-111">Permission type</span></span>|<span data-ttu-id="f3f39-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3f39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3f39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3f39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3f39-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3f39-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3f39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3f39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3f39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3f39-116">Not supported.</span></span>|
|<span data-ttu-id="f3f39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3f39-117">Application</span></span>|<span data-ttu-id="f3f39-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3f39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3f39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3f39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="f3f39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3f39-120">Request headers</span></span>
|<span data-ttu-id="f3f39-121">标头</span><span class="sxs-lookup"><span data-stu-id="f3f39-121">Header</span></span>|<span data-ttu-id="f3f39-122">值</span><span class="sxs-lookup"><span data-stu-id="f3f39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3f39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3f39-123">Authorization</span></span>|<span data-ttu-id="f3f39-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3f39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3f39-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3f39-125">Accept</span></span>|<span data-ttu-id="f3f39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3f39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3f39-127">Request body</span></span>
<span data-ttu-id="f3f39-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3f39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3f39-129">响应</span><span class="sxs-lookup"><span data-stu-id="f3f39-129">Response</span></span>
<span data-ttu-id="f3f39-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f3f39-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3f39-131">示例</span><span class="sxs-lookup"><span data-stu-id="f3f39-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3f39-132">请求</span><span class="sxs-lookup"><span data-stu-id="f3f39-132">Request</span></span>
<span data-ttu-id="f3f39-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3f39-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="f3f39-134">响应</span><span class="sxs-lookup"><span data-stu-id="f3f39-134">Response</span></span>
<span data-ttu-id="f3f39-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3f39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





