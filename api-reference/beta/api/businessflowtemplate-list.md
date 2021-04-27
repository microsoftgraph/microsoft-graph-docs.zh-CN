---
title: 列出 businessFlowTemplates
description: 在 Azure AD 访问评审功能中，列出所有 businessFlowTemplate 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 1b6a970e9e7336ba4773c3ecbe0e53f7c02e8700
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047768"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="db188-103">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="db188-103">List businessFlowTemplates</span></span>

<span data-ttu-id="db188-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db188-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db188-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，列出 [所有 businessFlowTemplate](../resources/businessflowtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db188-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="db188-106">权限</span><span class="sxs-lookup"><span data-stu-id="db188-106">Permissions</span></span>
<span data-ttu-id="db188-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db188-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db188-109">Permission type</span></span>                        | <span data-ttu-id="db188-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db188-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="db188-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db188-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db188-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db188-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="db188-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db188-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db188-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db188-114">Not supported.</span></span> |
|<span data-ttu-id="db188-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db188-115">Application</span></span>                            | <span data-ttu-id="db188-116">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="db188-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="db188-117">登录用户还必须具有允许其阅读访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="db188-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="db188-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db188-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="db188-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db188-119">Request headers</span></span>
| <span data-ttu-id="db188-120">名称</span><span class="sxs-lookup"><span data-stu-id="db188-120">Name</span></span>         | <span data-ttu-id="db188-121">类型</span><span class="sxs-lookup"><span data-stu-id="db188-121">Type</span></span>        | <span data-ttu-id="db188-122">说明</span><span class="sxs-lookup"><span data-stu-id="db188-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="db188-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db188-123">Authorization</span></span> | <span data-ttu-id="db188-124">string</span><span class="sxs-lookup"><span data-stu-id="db188-124">string</span></span> | <span data-ttu-id="db188-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="db188-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db188-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db188-127">Request body</span></span>
<span data-ttu-id="db188-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="db188-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="db188-129">响应</span><span class="sxs-lookup"><span data-stu-id="db188-129">Response</span></span>
<span data-ttu-id="db188-130">如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [businessFlowTemplate](../resources/businessflowtemplate.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="db188-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db188-131">示例</span><span class="sxs-lookup"><span data-stu-id="db188-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db188-132">请求</span><span class="sxs-lookup"><span data-stu-id="db188-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="db188-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db188-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="db188-134">C#</span><span class="sxs-lookup"><span data-stu-id="db188-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db188-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db188-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db188-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db188-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db188-137">Java</span><span class="sxs-lookup"><span data-stu-id="db188-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db188-138">响应</span><span class="sxs-lookup"><span data-stu-id="db188-138">Response</span></span>
><span data-ttu-id="db188-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db188-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access reviews of guest user memberships of a group"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access reviews of guest user assignments to an application"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access reviews of assignments to an application"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access reviews of memberships of a group"
        },
        {
            "id": "d7e0b82d-997f-44d0-ac5e-de9deb087c15",
            "displayName": "Access reviews of memberships of an Azure AD role"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="db188-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="db188-140">See also</span></span>

| <span data-ttu-id="db188-141">方法</span><span class="sxs-lookup"><span data-stu-id="db188-141">Method</span></span>           | <span data-ttu-id="db188-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="db188-142">Return Type</span></span>    |<span data-ttu-id="db188-143">说明</span><span class="sxs-lookup"><span data-stu-id="db188-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db188-144">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="db188-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="db188-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="db188-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="db188-146">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="db188-146">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


