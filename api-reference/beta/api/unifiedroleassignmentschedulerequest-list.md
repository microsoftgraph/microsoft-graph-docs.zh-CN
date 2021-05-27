---
title: 列出 unifiedRoleAssignmentScheduleRequests
description: 获取 unifiedRoleAssignmentScheduleRequest 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eb84749f882244d7aa3d85f5768a0bf487fed3b6
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680435"
---
# <a name="list-unifiedroleassignmentschedulerequests"></a><span data-ttu-id="dea88-103">列出 unifiedRoleAssignmentScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="dea88-103">List unifiedRoleAssignmentScheduleRequests</span></span>

<span data-ttu-id="dea88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dea88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea88-105">获取 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="dea88-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dea88-106">权限</span><span class="sxs-lookup"><span data-stu-id="dea88-106">Permissions</span></span>

<span data-ttu-id="dea88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dea88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dea88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dea88-109">Permission type</span></span>                        | <span data-ttu-id="dea88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dea88-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dea88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dea88-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dea88-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="dea88-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>          |
| <span data-ttu-id="dea88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dea88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dea88-114">不支持</span><span class="sxs-lookup"><span data-stu-id="dea88-114">Not supported</span></span>                               |
| <span data-ttu-id="dea88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dea88-115">Application</span></span>                            | <span data-ttu-id="dea88-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="dea88-116">PrivilegedAccess.Read.AzureAD</span></span>               |

## <a name="http-request"></a><span data-ttu-id="dea88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dea88-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dea88-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dea88-118">Optional query parameters</span></span>

<span data-ttu-id="dea88-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dea88-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dea88-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="dea88-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea88-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dea88-121">Request headers</span></span>

| <span data-ttu-id="dea88-122">名称</span><span class="sxs-lookup"><span data-stu-id="dea88-122">Name</span></span>          | <span data-ttu-id="dea88-123">说明</span><span class="sxs-lookup"><span data-stu-id="dea88-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dea88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dea88-124">Authorization</span></span> | <span data-ttu-id="dea88-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dea88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dea88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dea88-127">Request body</span></span>

<span data-ttu-id="dea88-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dea88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea88-129">响应</span><span class="sxs-lookup"><span data-stu-id="dea88-129">Response</span></span>

<span data-ttu-id="dea88-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dea88-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dea88-131">示例</span><span class="sxs-lookup"><span data-stu-id="dea88-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dea88-132">请求</span><span class="sxs-lookup"><span data-stu-id="dea88-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dea88-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea88-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
```
# <a name="c"></a>[<span data-ttu-id="dea88-134">C#</span><span class="sxs-lookup"><span data-stu-id="dea88-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dea88-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea88-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dea88-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea88-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dea88-137">Java</span><span class="sxs-lookup"><span data-stu-id="dea88-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dea88-138">响应</span><span class="sxs-lookup"><span data-stu-id="dea88-138">Response</span></span>

<span data-ttu-id="dea88-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dea88-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
      "action": "String",
      "principalId": "String",
      "roleDefinitionId": "String",
      "directoryScopeId": "String",
      "appScopeId": "String",
      "isValidationOnly": "Boolean",
      "targetScheduleId": "String",
      "justification": "String",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```
