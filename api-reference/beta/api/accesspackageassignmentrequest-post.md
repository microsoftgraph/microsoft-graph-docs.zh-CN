---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4696a0c90e15eefe6e4dc9135438b911d8b6b591
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383467"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="939fb-103">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="939fb-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="939fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="939fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="939fb-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，创建一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="939fb-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="939fb-106">此操作用于将用户分配给访问包，或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="939fb-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="939fb-107">权限</span><span class="sxs-lookup"><span data-stu-id="939fb-107">Permissions</span></span>

<span data-ttu-id="939fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="939fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="939fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="939fb-110">Permission type</span></span>                        | <span data-ttu-id="939fb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="939fb-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="939fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="939fb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="939fb-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="939fb-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="939fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="939fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="939fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="939fb-115">Not supported.</span></span> |
| <span data-ttu-id="939fb-116">Application</span><span class="sxs-lookup"><span data-stu-id="939fb-116">Application</span></span>                            | <span data-ttu-id="939fb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="939fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="939fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="939fb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="939fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="939fb-119">Request headers</span></span>

| <span data-ttu-id="939fb-120">名称</span><span class="sxs-lookup"><span data-stu-id="939fb-120">Name</span></span>          | <span data-ttu-id="939fb-121">说明</span><span class="sxs-lookup"><span data-stu-id="939fb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="939fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="939fb-122">Authorization</span></span> | <span data-ttu-id="939fb-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="939fb-123">Bearer \{token\}.</span></span> <span data-ttu-id="939fb-124">必填。</span><span class="sxs-lookup"><span data-stu-id="939fb-124">Required.</span></span> |
| <span data-ttu-id="939fb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="939fb-125">Content-Type</span></span>  | <span data-ttu-id="939fb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="939fb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="939fb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="939fb-128">Request body</span></span>

<span data-ttu-id="939fb-129">在请求正文中，提供[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="939fb-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="939fb-130">若要为用户创建分配， **requestType**属性的值是 `AdminAdd` ， **accessPackageAssignment**属性包含 `targetId` 被分配的用户、 **assignmentPolicyId**属性（标识[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)）和标识[accessPackage](../resources/accesspackage.md)的**accessPackageId**属性。</span><span class="sxs-lookup"><span data-stu-id="939fb-130">To create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="939fb-131">若要删除分配， **requestType**属性的值是 `AdminRemove` ， **accessPackageAssignment**属性包含标识要删除的[accessPackageAssignment](../resources/accesspackageassignment.md)的**id**属性。</span><span class="sxs-lookup"><span data-stu-id="939fb-131">To remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

## <a name="response"></a><span data-ttu-id="939fb-132">响应</span><span class="sxs-lookup"><span data-stu-id="939fb-132">Response</span></span>

<span data-ttu-id="939fb-133">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="939fb-133">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  <span data-ttu-id="939fb-134">如果这是一个 `AdminAdd` 请求，则随后是[accessPackageAssignment](../resources/accesspackageassignment.md) ，如果需要，还会创建一个[accessPackageSubject](../resources/accesspackagesubject.md) 。</span><span class="sxs-lookup"><span data-stu-id="939fb-134">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="939fb-135">在[列出 accessPackageAssignments](accesspackageassignment-list.md)时，可以使用查询参数找到这些参数。</span><span class="sxs-lookup"><span data-stu-id="939fb-135">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="939fb-136">示例</span><span class="sxs-lookup"><span data-stu-id="939fb-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="939fb-137">请求</span><span class="sxs-lookup"><span data-stu-id="939fb-137">Request</span></span>

<span data-ttu-id="939fb-138">下面是一个直接分配请求的示例，在该请求中，管理员请求为用户创建分配。</span><span class="sxs-lookup"><span data-stu-id="939fb-138">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="939fb-139">由于[accessPackageSubject](../resources/accesspackagesubject.md)可能尚不存在， **targetID**的值是要分配的用户的对象 ID， **accessPackageId**的值是该用户所需的访问包， **assignmentPolicyId**的值是该访问包中的直接分配策略。</span><span class="sxs-lookup"><span data-stu-id="939fb-139">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="939fb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="939fb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="939fb-141">C#</span><span class="sxs-lookup"><span data-stu-id="939fb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="939fb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="939fb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="939fb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="939fb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="939fb-144">响应</span><span class="sxs-lookup"><span data-stu-id="939fb-144">Response</span></span>

<span data-ttu-id="939fb-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="939fb-145">The following is an example of the response.</span></span>

> <span data-ttu-id="939fb-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="939fb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
