---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 128c4c84879ec11c6ac0b54991247b84125285f2
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108404"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="24bf5-103">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="24bf5-103">Create accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24bf5-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，创建一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24bf5-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="24bf5-105">此操作用于将用户分配给访问包，或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="24bf5-105">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="24bf5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="24bf5-106">Permissions</span></span>

<span data-ttu-id="24bf5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24bf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24bf5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24bf5-109">Permission type</span></span>                        | <span data-ttu-id="24bf5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24bf5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="24bf5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24bf5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24bf5-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24bf5-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="24bf5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24bf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24bf5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24bf5-114">Not supported.</span></span> |
| <span data-ttu-id="24bf5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24bf5-115">Application</span></span>                            | <span data-ttu-id="24bf5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24bf5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24bf5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24bf5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="24bf5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="24bf5-118">Request headers</span></span>

| <span data-ttu-id="24bf5-119">名称</span><span class="sxs-lookup"><span data-stu-id="24bf5-119">Name</span></span>          | <span data-ttu-id="24bf5-120">说明</span><span class="sxs-lookup"><span data-stu-id="24bf5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24bf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24bf5-121">Authorization</span></span> | <span data-ttu-id="24bf5-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="24bf5-122">Bearer \{token\}.</span></span> <span data-ttu-id="24bf5-123">必填。</span><span class="sxs-lookup"><span data-stu-id="24bf5-123">Required.</span></span> |
| <span data-ttu-id="24bf5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24bf5-124">Content-Type</span></span>  | <span data-ttu-id="24bf5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="24bf5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24bf5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24bf5-127">Request body</span></span>

<span data-ttu-id="24bf5-128">在请求正文中，提供[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24bf5-128">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="24bf5-129">若要为用户创建分配， **requestType** `AdminAdd`属性的值是， **accessPackageAssignment**属性包含`targetId`被分配的用户、 **assignmentPolicyId**属性（标识[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)）和标识[accessPackage](../resources/accesspackage.md)的**accessPackageId**属性。</span><span class="sxs-lookup"><span data-stu-id="24bf5-129">To create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="24bf5-130">若要删除分配， **requestType**属性`AdminRemove`的值是， **accessPackageAssignment**属性包含标识要删除的[accessPackageAssignment](../resources/accesspackageassignment.md)的**id**属性。</span><span class="sxs-lookup"><span data-stu-id="24bf5-130">To remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

## <a name="response"></a><span data-ttu-id="24bf5-131">响应</span><span class="sxs-lookup"><span data-stu-id="24bf5-131">Response</span></span>

<span data-ttu-id="24bf5-132">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24bf5-132">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24bf5-133">示例</span><span class="sxs-lookup"><span data-stu-id="24bf5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24bf5-134">请求</span><span class="sxs-lookup"><span data-stu-id="24bf5-134">Request</span></span>

<span data-ttu-id="24bf5-135">下面是一个直接分配请求的示例。</span><span class="sxs-lookup"><span data-stu-id="24bf5-135">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="24bf5-136">**TargetID**的值是要分配的用户的对象 ID， **accessPackageId**的值是所需的访问包，而**assignmentPolicyId**的值是该访问包中的直接分配策略。</span><span class="sxs-lookup"><span data-stu-id="24bf5-136">The value of the **targetID** is the object ID of a user being assigned, the value of the **accessPackageId** is the desired access package, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="24bf5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="24bf5-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="24bf5-138">C#</span><span class="sxs-lookup"><span data-stu-id="24bf5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24bf5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24bf5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24bf5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24bf5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24bf5-141">响应</span><span class="sxs-lookup"><span data-stu-id="24bf5-141">Response</span></span>

<span data-ttu-id="24bf5-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="24bf5-142">The following is an example of the response.</span></span>

> <span data-ttu-id="24bf5-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="24bf5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
