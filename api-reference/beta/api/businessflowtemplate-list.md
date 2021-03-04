---
title: 列出 businessFlowTemplates
description: 在 Azure AD 访问评审功能中，列出所有 businessFlowTemplate 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 1ecb7dac1020bf243f6f58e0f6a80afc0724bfdc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437987"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="d1b7a-103">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="d1b7a-103">List businessFlowTemplates</span></span>

<span data-ttu-id="d1b7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1b7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1b7a-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，列出 [所有 businessFlowTemplate](../resources/businessflowtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1b7a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1b7a-106">Permissions</span></span>
<span data-ttu-id="d1b7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1b7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1b7a-109">Permission type</span></span>                        | <span data-ttu-id="d1b7a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1b7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1b7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1b7a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1b7a-112">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1b7a-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="d1b7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1b7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1b7a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-114">Not supported.</span></span> |
|<span data-ttu-id="d1b7a-115">Application</span><span class="sxs-lookup"><span data-stu-id="d1b7a-115">Application</span></span>                            | <span data-ttu-id="d1b7a-116">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="d1b7a-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="d1b7a-117">登录用户还必须具有允许其读取访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d1b7a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1b7a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="d1b7a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1b7a-119">Request headers</span></span>
| <span data-ttu-id="d1b7a-120">名称</span><span class="sxs-lookup"><span data-stu-id="d1b7a-120">Name</span></span>         | <span data-ttu-id="d1b7a-121">类型</span><span class="sxs-lookup"><span data-stu-id="d1b7a-121">Type</span></span>        | <span data-ttu-id="d1b7a-122">说明</span><span class="sxs-lookup"><span data-stu-id="d1b7a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d1b7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1b7a-123">Authorization</span></span> | <span data-ttu-id="d1b7a-124">string</span><span class="sxs-lookup"><span data-stu-id="d1b7a-124">string</span></span> | <span data-ttu-id="d1b7a-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1b7a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1b7a-127">Request body</span></span>
<span data-ttu-id="d1b7a-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d1b7a-129">响应</span><span class="sxs-lookup"><span data-stu-id="d1b7a-129">Response</span></span>
<span data-ttu-id="d1b7a-130">如果成功，此方法在响应正文中返回响应代码 `200, OK` 和 [businessFlowTemplate](../resources/businessflowtemplate.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1b7a-131">示例</span><span class="sxs-lookup"><span data-stu-id="d1b7a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1b7a-132">请求</span><span class="sxs-lookup"><span data-stu-id="d1b7a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d1b7a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1b7a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="d1b7a-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1b7a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1b7a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1b7a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1b7a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1b7a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1b7a-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1b7a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1b7a-138">响应</span><span class="sxs-lookup"><span data-stu-id="d1b7a-138">Response</span></span>
><span data-ttu-id="d1b7a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d1b7a-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d1b7a-141">See also</span></span>

| <span data-ttu-id="d1b7a-142">方法</span><span class="sxs-lookup"><span data-stu-id="d1b7a-142">Method</span></span>           | <span data-ttu-id="d1b7a-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1b7a-143">Return Type</span></span>    |<span data-ttu-id="d1b7a-144">说明</span><span class="sxs-lookup"><span data-stu-id="d1b7a-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1b7a-145">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="d1b7a-145">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="d1b7a-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="d1b7a-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d1b7a-147">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="d1b7a-147">Create a new accessReview.</span></span> |




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


