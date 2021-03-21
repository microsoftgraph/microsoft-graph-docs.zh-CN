---
title: 列出 unifiedRoleAssignments
description: 获取 unifiedRoleAssignment 对象的列表。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b267a347537b46a29fd2d74afc1161e026a84bcc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959069"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="da4aa-103">列出 unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="da4aa-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="da4aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da4aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da4aa-105">获取提供商的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="da4aa-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="da4aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="da4aa-106">Permissions</span></span>

<span data-ttu-id="da4aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da4aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da4aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="da4aa-109">Permission type</span></span>      | <span data-ttu-id="da4aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da4aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da4aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da4aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da4aa-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da4aa-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da4aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da4aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da4aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="da4aa-114">Not supported.</span></span>    |
|<span data-ttu-id="da4aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="da4aa-115">Application</span></span> | <span data-ttu-id="da4aa-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da4aa-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da4aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da4aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da4aa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da4aa-118">Optional query parameters</span></span>

<span data-ttu-id="da4aa-119">此操作需要 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="da4aa-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="da4aa-120">可以筛选 或 `roleDefinitionId` `principalId` 属性。</span><span class="sxs-lookup"><span data-stu-id="da4aa-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="da4aa-121">属性 `roleDefinitionId` 可以是角色对象 ID 或角色模板对象 ID。</span><span class="sxs-lookup"><span data-stu-id="da4aa-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="da4aa-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="da4aa-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da4aa-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="da4aa-123">Request headers</span></span>

| <span data-ttu-id="da4aa-124">名称</span><span class="sxs-lookup"><span data-stu-id="da4aa-124">Name</span></span>      |<span data-ttu-id="da4aa-125">说明</span><span class="sxs-lookup"><span data-stu-id="da4aa-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da4aa-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="da4aa-126">Authorization</span></span> | <span data-ttu-id="da4aa-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="da4aa-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="da4aa-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="da4aa-128">Request body</span></span>

<span data-ttu-id="da4aa-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da4aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da4aa-130">响应</span><span class="sxs-lookup"><span data-stu-id="da4aa-130">Response</span></span>

<span data-ttu-id="da4aa-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="da4aa-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da4aa-132">示例</span><span class="sxs-lookup"><span data-stu-id="da4aa-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="da4aa-133">示例 1：对角色定义 ID 使用筛选器的请求</span><span class="sxs-lookup"><span data-stu-id="da4aa-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="da4aa-134">请求</span><span class="sxs-lookup"><span data-stu-id="da4aa-134">Request</span></span>

<span data-ttu-id="da4aa-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da4aa-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="da4aa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="da4aa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="da4aa-137">C#</span><span class="sxs-lookup"><span data-stu-id="da4aa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da4aa-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da4aa-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da4aa-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da4aa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da4aa-140">Java</span><span class="sxs-lookup"><span data-stu-id="da4aa-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da4aa-141">响应</span><span class="sxs-lookup"><span data-stu-id="da4aa-141">Response</span></span>

<span data-ttu-id="da4aa-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da4aa-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments(principal())",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMmO4KwRqtpKkUWt3wOYIz4-1",
            "principalId": "ace08ec9-aa11-4ada-9145-addf0398233e",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "ace08ec9-aa11-4ada-9145-addf0398233e",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": "Redmond",
                "createdDateTime": "2019-02-22T20:29:07Z",
                "creationType": null,
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": "US",
                "department": "Office of the CEO",
                "displayName": "Joey Cruz",
                "employeeId": null,
                "faxNumber": null,
                "givenName": "Joey",
                "imAddresses": [
                    "joeyc@woodgrove.ms"
                ],
                "infoCatalogs": [],
                "isResourceAccount": null,
                "jobTitle": "Chief Security Officer",
                "legalAgeGroupClassification": null,
                "mail": "joeyc@woodgrove.ms",
                "mailNickname": "joeyc",
                "mobilePhone": null,
                "onPremisesDistinguishedName": null,
                "officeLocation": null,
                "userType": "Member",   

            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEC6Xh29-LklLmYDrOIi9z-E-1",
            "principalId": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-07-18T01:38:36Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Kalyan Krishna",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
    
            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMgc_BA2rIZBuZsM-BSqLdU-1",
            "principalId": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-11-13T21:54:27Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Markie Downing",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
        
            }
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="da4aa-143">示例 2：对主体 ID 使用筛选器的请求</span><span class="sxs-lookup"><span data-stu-id="da4aa-143">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="da4aa-144">请求</span><span class="sxs-lookup"><span data-stu-id="da4aa-144">Request</span></span>

<span data-ttu-id="da4aa-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da4aa-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="da4aa-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="da4aa-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="da4aa-147">C#</span><span class="sxs-lookup"><span data-stu-id="da4aa-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da4aa-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da4aa-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da4aa-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da4aa-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da4aa-150">Java</span><span class="sxs-lookup"><span data-stu-id="da4aa-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da4aa-151">响应</span><span class="sxs-lookup"><span data-stu-id="da4aa-151">Response</span></span>

<span data-ttu-id="da4aa-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da4aa-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEHJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "LJnv8vs6uUa3z6Em7nTEUXJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


