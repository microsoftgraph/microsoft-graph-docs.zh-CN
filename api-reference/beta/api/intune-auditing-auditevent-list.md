---
title: 列出 auditEvents
description: 列出 auditEvent 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f092553031c1e5c12c6f35adf3858223516bfb2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934381"
---
# <a name="list-auditevents"></a><span data-ttu-id="abb3b-103">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="abb3b-103">List auditEvents</span></span>

> <span data-ttu-id="abb3b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="abb3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb3b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abb3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb3b-106">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="abb3b-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abb3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="abb3b-107">Prerequisites</span></span>
<span data-ttu-id="abb3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb3b-110">Permission type</span></span>|<span data-ttu-id="abb3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abb3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abb3b-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb3b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abb3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb3b-115">Not supported.</span></span>|
|<span data-ttu-id="abb3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb3b-116">Application</span></span>|<span data-ttu-id="abb3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="abb3b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb3b-119">Request headers</span></span>
|<span data-ttu-id="abb3b-120">标头</span><span class="sxs-lookup"><span data-stu-id="abb3b-120">Header</span></span>|<span data-ttu-id="abb3b-121">值</span><span class="sxs-lookup"><span data-stu-id="abb3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb3b-122">Authorization</span></span>|<span data-ttu-id="abb3b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abb3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb3b-124">接受</span><span class="sxs-lookup"><span data-stu-id="abb3b-124">Accept</span></span>|<span data-ttu-id="abb3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abb3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb3b-126">Request body</span></span>
<span data-ttu-id="abb3b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abb3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abb3b-128">响应</span><span class="sxs-lookup"><span data-stu-id="abb3b-128">Response</span></span>
<span data-ttu-id="abb3b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="abb3b-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb3b-130">示例</span><span class="sxs-lookup"><span data-stu-id="abb3b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb3b-131">请求</span><span class="sxs-lookup"><span data-stu-id="abb3b-131">Request</span></span>
<span data-ttu-id="abb3b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abb3b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="abb3b-133">响应</span><span class="sxs-lookup"><span data-stu-id="abb3b-133">Response</span></span>
<span data-ttu-id="abb3b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abb3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




