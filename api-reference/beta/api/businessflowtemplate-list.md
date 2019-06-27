---
title: 列出 businessFlowTemplates
description: 在 "Azure AD access 评论" 功能中, 列出所有 businessFlowTemplate 对象。
localization_priority: Normal
ms.openlocfilehash: 3f7fc6ac155b22845c13c75fddd1af49f7b32e32
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262445"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="82200-103">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="82200-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82200-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[businessFlowTemplate](../resources/businessflowtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82200-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="82200-105">权限</span><span class="sxs-lookup"><span data-stu-id="82200-105">Permissions</span></span>
<span data-ttu-id="82200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82200-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="82200-108">Permission type</span></span>                        | <span data-ttu-id="82200-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82200-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="82200-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82200-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82200-111">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="82200-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="82200-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82200-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82200-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="82200-113">Not supported.</span></span> |
|<span data-ttu-id="82200-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="82200-114">Application</span></span>                            | <span data-ttu-id="82200-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="82200-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="82200-116">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="82200-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="82200-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82200-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="82200-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="82200-118">Request headers</span></span>
| <span data-ttu-id="82200-119">名称</span><span class="sxs-lookup"><span data-stu-id="82200-119">Name</span></span>         | <span data-ttu-id="82200-120">类型</span><span class="sxs-lookup"><span data-stu-id="82200-120">Type</span></span>        | <span data-ttu-id="82200-121">说明</span><span class="sxs-lookup"><span data-stu-id="82200-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="82200-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82200-122">Authorization</span></span> | <span data-ttu-id="82200-123">string</span><span class="sxs-lookup"><span data-stu-id="82200-123">string</span></span> | <span data-ttu-id="82200-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="82200-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82200-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82200-126">Request body</span></span>
<span data-ttu-id="82200-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="82200-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="82200-128">响应</span><span class="sxs-lookup"><span data-stu-id="82200-128">Response</span></span>
<span data-ttu-id="82200-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[businessFlowTemplate](../resources/businessflowtemplate.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="82200-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82200-130">示例</span><span class="sxs-lookup"><span data-stu-id="82200-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82200-131">请求</span><span class="sxs-lookup"><span data-stu-id="82200-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="82200-132">响应</span><span class="sxs-lookup"><span data-stu-id="82200-132">Response</span></span>
><span data-ttu-id="82200-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="82200-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="82200-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="82200-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="82200-136">C#</span><span class="sxs-lookup"><span data-stu-id="82200-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82200-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="82200-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="82200-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="82200-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="82200-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82200-139">See also</span></span>

| <span data-ttu-id="82200-140">方法</span><span class="sxs-lookup"><span data-stu-id="82200-140">Method</span></span>           | <span data-ttu-id="82200-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="82200-141">Return Type</span></span>    |<span data-ttu-id="82200-142">说明</span><span class="sxs-lookup"><span data-stu-id="82200-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82200-143">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="82200-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="82200-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="82200-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="82200-145">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="82200-145">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}
-->
