---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ff0f60841fe852d67e5c76268fe4e00ce277af11
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048594"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="0b398-103">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="0b398-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="0b398-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b398-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，创建新的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b398-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="0b398-106">此操作用于将用户分配给访问包或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="0b398-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b398-107">权限</span><span class="sxs-lookup"><span data-stu-id="0b398-107">Permissions</span></span>

<span data-ttu-id="0b398-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b398-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b398-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b398-110">Permission type</span></span>                        | <span data-ttu-id="0b398-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b398-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b398-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b398-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b398-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b398-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0b398-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b398-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b398-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b398-115">Not supported.</span></span> |
| <span data-ttu-id="0b398-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b398-116">Application</span></span>                            | <span data-ttu-id="0b398-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b398-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b398-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b398-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="0b398-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b398-119">Request headers</span></span>

| <span data-ttu-id="0b398-120">名称</span><span class="sxs-lookup"><span data-stu-id="0b398-120">Name</span></span>          | <span data-ttu-id="0b398-121">说明</span><span class="sxs-lookup"><span data-stu-id="0b398-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0b398-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b398-122">Authorization</span></span> | <span data-ttu-id="0b398-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b398-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="0b398-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b398-125">Content-Type</span></span>  | <span data-ttu-id="0b398-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0b398-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b398-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b398-128">Request body</span></span>

<span data-ttu-id="0b398-129">在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b398-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="0b398-130">对于请求为用户创建工作分配的管理员 **，requestType** 属性的值为 ，accessPackageAssignment 属性包含要分配的用户的 、标识 `AdminAdd`  `targetId` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)的 **assignmentPolicyId** 属性和标识 accessPackage 的 **accessPackageId**[](../resources/accesspackage.md)属性。</span><span class="sxs-lookup"><span data-stu-id="0b398-130">For an administrator to request to create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="0b398-131">对于请求删除分配的管理员 **，requestType** 属性的值为 `AdminRemove` **，accessPackageAssignment** 属性包含标识要删除的 [accessPackageAssignment](../resources/accesspackageassignment.md)的 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="0b398-131">For an administrator to request to remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

<span data-ttu-id="0b398-132">对于需要自行创建工作分配的非管理员用户 **，requestType** 属性的值为 ，accessPackageAssignment 属性包含具有用户本身 ID 的 、 `UserAdd`  `targetId` 标识 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)的 **assignmentPolicyId** 属性和标识 accessPackage 的 **accessPackageId**[](../resources/accesspackage.md)属性。</span><span class="sxs-lookup"><span data-stu-id="0b398-132">For a non-administrator user to request to create an assignment for themselves, the value of the **requestType** property is `UserAdd`, and the **accessPackageAssignment** property contains the `targetId` with the ID of the users themselves, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>  <span data-ttu-id="0b398-133">提出请求的用户必须已存在于 目录中。</span><span class="sxs-lookup"><span data-stu-id="0b398-133">The user making the request must already exist in the directory.</span></span>

## <a name="response"></a><span data-ttu-id="0b398-134">响应</span><span class="sxs-lookup"><span data-stu-id="0b398-134">Response</span></span>

<span data-ttu-id="0b398-135">如果成功，此方法在响应正文中返回 200 系列响应代码和新 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b398-135">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  

<span data-ttu-id="0b398-136">如果这是请求，则随后会 `AdminAdd` [创建 accessPackageAssignment，](../resources/accesspackageassignment.md)如果需要，还会创建[accessPackageSubject。](../resources/accesspackagesubject.md)</span><span class="sxs-lookup"><span data-stu-id="0b398-136">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="0b398-137">在列出 [accessPackageAssignments](accesspackageassignment-list.md)时，可以使用查询参数查找这些参数。</span><span class="sxs-lookup"><span data-stu-id="0b398-137">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="0b398-138">示例</span><span class="sxs-lookup"><span data-stu-id="0b398-138">Examples</span></span>
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a><span data-ttu-id="0b398-139">示例 1：管理员请求直接分配用户</span><span class="sxs-lookup"><span data-stu-id="0b398-139">Example 1: Admin requests a direct assignment for a user</span></span>
#### <a name="request"></a><span data-ttu-id="0b398-140">请求</span><span class="sxs-lookup"><span data-stu-id="0b398-140">Request</span></span>

<span data-ttu-id="0b398-141">下面是直接分配请求的一个示例，其中管理员请求为用户创建工作分配。</span><span class="sxs-lookup"><span data-stu-id="0b398-141">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="0b398-142">由于 [accessPackageSubject](../resources/accesspackagesubject.md) 可能尚不存在 **，targetID** 的值是分配的用户的对象 **ID，accessPackageId** 的值是该用户所需的访问包 **，assignmentPolicyId** 的值是该访问包中的直接分配策略。</span><span class="sxs-lookup"><span data-stu-id="0b398-142">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="0b398-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b398-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
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
# <a name="c"></a>[<span data-ttu-id="0b398-144">C#</span><span class="sxs-lookup"><span data-stu-id="0b398-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b398-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b398-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b398-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b398-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b398-147">Java</span><span class="sxs-lookup"><span data-stu-id="0b398-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b398-148">响应</span><span class="sxs-lookup"><span data-stu-id="0b398-148">Response</span></span>

<span data-ttu-id="0b398-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b398-149">The following is an example of the response.</span></span>

> <span data-ttu-id="0b398-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b398-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a><span data-ttu-id="0b398-151">示例 2：用户请求程序包并回答需要审批的问题</span><span class="sxs-lookup"><span data-stu-id="0b398-151">Example 2: User requests a package and answers questions for approval</span></span>
#### <a name="request"></a><span data-ttu-id="0b398-152">请求</span><span class="sxs-lookup"><span data-stu-id="0b398-152">Request</span></span>

<span data-ttu-id="0b398-153">下面是请求的一个示例，请求者向审批者提供了答案以帮助他们做出决策。</span><span class="sxs-lookup"><span data-stu-id="0b398-153">The following is an example of a request where the requestor provided answers to the approver to help them make their decision.</span></span>
 



# <a name="http"></a>[<span data-ttu-id="0b398-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b398-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
        "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
        }
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="0b398-155">C#</span><span class="sxs-lookup"><span data-stu-id="0b398-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b398-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b398-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b398-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b398-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b398-158">Java</span><span class="sxs-lookup"><span data-stu-id="0b398-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a><span data-ttu-id="0b398-159">响应</span><span class="sxs-lookup"><span data-stu-id="0b398-159">Response</span></span>

<span data-ttu-id="0b398-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b398-160">The following is an example of the response.</span></span>

> <span data-ttu-id="0b398-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b398-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
            "isRequired": false,
            "text": {
                "defaultText": "what state are you from?",
                "localizedTexts": [{
                    "text": "¿De qué estado eres?",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
            "choices": [{
                "actualValue": "AZ",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Arizona",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "CA",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "California",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "OH",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Ohio",
                        "languageCode": "es"
                    }]
                }
            }],
            "allowsMultipleSelection": false
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
            "isRequired": false,
            "text": {
                "defaultText": "Who is your manager?",
                "localizedTexts": [{
                    "text": "por qué necesita acceso a este paquete",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": false
        }
    }]
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


