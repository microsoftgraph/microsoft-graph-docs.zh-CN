---
title: 列出 businessFlowTemplates
description: 在 "Azure AD access 评论" 功能中, 列出所有 businessFlowTemplate 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cce66344a9420efb6a9b78c15c6d6f66a8f20c71
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718777"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="96f73-103">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="96f73-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96f73-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[businessFlowTemplate](../resources/businessflowtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96f73-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="96f73-105">权限</span><span class="sxs-lookup"><span data-stu-id="96f73-105">Permissions</span></span>
<span data-ttu-id="96f73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f73-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96f73-108">Permission type</span></span>                        | <span data-ttu-id="96f73-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96f73-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="96f73-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96f73-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="96f73-111">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="96f73-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="96f73-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96f73-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96f73-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f73-113">Not supported.</span></span> |
|<span data-ttu-id="96f73-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96f73-114">Application</span></span>                            | <span data-ttu-id="96f73-115">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="96f73-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="96f73-116">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="96f73-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="96f73-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96f73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="96f73-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96f73-118">Request headers</span></span>
| <span data-ttu-id="96f73-119">名称</span><span class="sxs-lookup"><span data-stu-id="96f73-119">Name</span></span>         | <span data-ttu-id="96f73-120">类型</span><span class="sxs-lookup"><span data-stu-id="96f73-120">Type</span></span>        | <span data-ttu-id="96f73-121">说明</span><span class="sxs-lookup"><span data-stu-id="96f73-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="96f73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f73-122">Authorization</span></span> | <span data-ttu-id="96f73-123">string</span><span class="sxs-lookup"><span data-stu-id="96f73-123">string</span></span> | <span data-ttu-id="96f73-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="96f73-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96f73-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="96f73-126">Request body</span></span>
<span data-ttu-id="96f73-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="96f73-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="96f73-128">响应</span><span class="sxs-lookup"><span data-stu-id="96f73-128">Response</span></span>
<span data-ttu-id="96f73-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[businessFlowTemplate](../resources/businessflowtemplate.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="96f73-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f73-130">示例</span><span class="sxs-lookup"><span data-stu-id="96f73-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96f73-131">请求</span><span class="sxs-lookup"><span data-stu-id="96f73-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96f73-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="96f73-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96f73-133">C#</span><span class="sxs-lookup"><span data-stu-id="96f73-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96f73-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96f73-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96f73-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="96f73-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96f73-136">响应</span><span class="sxs-lookup"><span data-stu-id="96f73-136">Response</span></span>
><span data-ttu-id="96f73-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96f73-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="96f73-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="96f73-139">See also</span></span>

| <span data-ttu-id="96f73-140">方法</span><span class="sxs-lookup"><span data-stu-id="96f73-140">Method</span></span>           | <span data-ttu-id="96f73-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="96f73-141">Return Type</span></span>    |<span data-ttu-id="96f73-142">说明</span><span class="sxs-lookup"><span data-stu-id="96f73-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96f73-143">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="96f73-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="96f73-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="96f73-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="96f73-145">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="96f73-145">Create a new accessReview.</span></span> |




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
