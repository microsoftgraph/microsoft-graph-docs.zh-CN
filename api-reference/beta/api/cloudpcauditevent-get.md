---
title: 获取 cloudPcAuditEvent
description: 读取 cloudPcAuditEvent 对象的属性和关系。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1848aa35f9c4b1f31159d950e946e898ff84ad1c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211217"
---
# <a name="get-cloudpcauditevent"></a><span data-ttu-id="b709b-103">获取 cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="b709b-103">Get cloudPcAuditEvent</span></span>

<span data-ttu-id="b709b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b709b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b709b-105">读取 [cloudPcAuditEvent 对象的属性和](../resources/cloudpcauditevent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b709b-105">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="b709b-106">权限</span><span class="sxs-lookup"><span data-stu-id="b709b-106">Permissions</span></span>

<span data-ttu-id="b709b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b709b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b709b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b709b-109">Permission type</span></span>| <span data-ttu-id="b709b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b709b-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="b709b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b709b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b709b-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b709b-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b709b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b709b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b709b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b709b-114">Not supported.</span></span>|
|<span data-ttu-id="b709b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b709b-115">Application</span></span>|<span data-ttu-id="b709b-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b709b-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b709b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b709b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b709b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b709b-118">Request headers</span></span>

| <span data-ttu-id="b709b-119">名称</span><span class="sxs-lookup"><span data-stu-id="b709b-119">Name</span></span>          | <span data-ttu-id="b709b-120">说明</span><span class="sxs-lookup"><span data-stu-id="b709b-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b709b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b709b-121">Authorization</span></span> | <span data-ttu-id="b709b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b709b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b709b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b709b-124">Request body</span></span>

<span data-ttu-id="b709b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b709b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b709b-126">响应</span><span class="sxs-lookup"><span data-stu-id="b709b-126">Response</span></span>

<span data-ttu-id="b709b-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcAuditEvent](../resources/cloudpcauditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b709b-127">If successful, this method returns a `200 OK` response code and a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b709b-128">示例</span><span class="sxs-lookup"><span data-stu-id="b709b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b709b-129">请求</span><span class="sxs-lookup"><span data-stu-id="b709b-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/{id}
```

### <a name="response"></a><span data-ttu-id="b709b-130">响应</span><span class="sxs-lookup"><span data-stu-id="b709b-130">Response</span></span>

><span data-ttu-id="b709b-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b709b-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
      "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
      "id": "250473f5-029f-4037-813d-ba4768201d61",
      "displayName": "Display Name value",
      "componentName": "Component Name value",  
      "activity": "Activity value",  
      "activityDateTime": "2021-02-14T13:10:51.814636+08:00",  
      "activityType": " Activity Type value",  
      "activityOperationType": "Activity Operation Type value",  
      "activityResult": "Activity Result value",  
      "correlationId": "a5c71cc6-2271-4d5c-9bfe-d94781e83fe6",  
      "category": "Category value",
      "actor": {
          "@odata.type": "microsoft.graph.cloudPcAuditActor",
          "type": "Type value",
          "userPermissions": [
              "User Permissions value"
          ],
          "applicationId": "Application Id value",
          "applicationDisplayName": "Application Display Name value",
          "userPrincipalName": "User Principal Name value",
          "servicePrincipalName": "Service Principal Name value",
          "ipAddress": "Ip Address value",
          "userId": "User Id value",
          "userRoleScopeTags": [
              {
                  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
                  "displayName": "Display Name value",
                  "roleScopeTagId": "Role Scope Tag Id value"
              }
          ],
          "remoteTenantId": "Remote Tenant Id value",
          "remoteUserId": "Remote User Id value"
      },
      "resources": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.cloudPcAuditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
  }
}
```
