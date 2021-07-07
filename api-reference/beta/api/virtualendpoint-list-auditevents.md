---
title: 列出 auditEvents
description: 获取 cloudPcAuditEvent 对象及其属性的列表。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2a2694a2b854c9fbaba137506d925ba8cf4829d6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316568"
---
# <a name="list-auditevents"></a><span data-ttu-id="8262a-103">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="8262a-103">List auditEvents</span></span>

<span data-ttu-id="8262a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8262a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8262a-105">列出租户 [的所有 cloudPcAuditEvent](../resources/cloudpcauditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8262a-105">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects for the tenant.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8262a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8262a-106">Permissions</span></span>

<span data-ttu-id="8262a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8262a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8262a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8262a-109">Permission type</span></span>|<span data-ttu-id="8262a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8262a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8262a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8262a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8262a-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8262a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8262a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8262a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8262a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8262a-114">Not supported.</span></span>|
|<span data-ttu-id="8262a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8262a-115">Application</span></span>|<span data-ttu-id="8262a-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8262a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8262a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8262a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8262a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8262a-118">Optional query parameters</span></span>

<span data-ttu-id="8262a-119">此方法支持 `$skiptoken` 、 `$top` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8262a-119">This method supports `$skiptoken`, `$top` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8262a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8262a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8262a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8262a-121">Request headers</span></span>

| <span data-ttu-id="8262a-122">名称</span><span class="sxs-lookup"><span data-stu-id="8262a-122">Name</span></span>          | <span data-ttu-id="8262a-123">说明</span><span class="sxs-lookup"><span data-stu-id="8262a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8262a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8262a-124">Authorization</span></span> | <span data-ttu-id="8262a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8262a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8262a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8262a-127">Request body</span></span>

<span data-ttu-id="8262a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8262a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8262a-129">响应</span><span class="sxs-lookup"><span data-stu-id="8262a-129">Response</span></span>

<span data-ttu-id="8262a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcAuditEvent](../resources/cloudpcauditevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8262a-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8262a-131">示例</span><span class="sxs-lookup"><span data-stu-id="8262a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8262a-132">请求</span><span class="sxs-lookup"><span data-stu-id="8262a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8262a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8262a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents
```
# <a name="c"></a>[<span data-ttu-id="8262a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8262a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcauditevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8262a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8262a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcauditevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8262a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8262a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcauditevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8262a-137">Java</span><span class="sxs-lookup"><span data-stu-id="8262a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcauditevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8262a-138">响应</span><span class="sxs-lookup"><span data-stu-id="8262a-138">Response</span></span>

><span data-ttu-id="8262a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8262a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```
