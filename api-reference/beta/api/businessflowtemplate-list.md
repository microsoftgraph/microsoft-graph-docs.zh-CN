---
title: 列出 businessFlowTemplates
description: 在 "Azure AD access 评论" 功能中，列出所有 businessFlowTemplate 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: adfa33bda915fcc74e234ab7473d62a761716d05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987710"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="72099-103">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="72099-103">List businessFlowTemplates</span></span>

<span data-ttu-id="72099-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72099-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72099-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，列出所有 [businessFlowTemplate](../resources/businessflowtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72099-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="72099-106">权限</span><span class="sxs-lookup"><span data-stu-id="72099-106">Permissions</span></span>
<span data-ttu-id="72099-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72099-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72099-109">Permission type</span></span>                        | <span data-ttu-id="72099-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72099-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="72099-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72099-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72099-112">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="72099-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="72099-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72099-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72099-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72099-114">Not supported.</span></span> |
|<span data-ttu-id="72099-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72099-115">Application</span></span>                            | <span data-ttu-id="72099-116">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="72099-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="72099-117">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="72099-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="72099-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72099-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="72099-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72099-119">Request headers</span></span>
| <span data-ttu-id="72099-120">名称</span><span class="sxs-lookup"><span data-stu-id="72099-120">Name</span></span>         | <span data-ttu-id="72099-121">类型</span><span class="sxs-lookup"><span data-stu-id="72099-121">Type</span></span>        | <span data-ttu-id="72099-122">说明</span><span class="sxs-lookup"><span data-stu-id="72099-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="72099-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72099-123">Authorization</span></span> | <span data-ttu-id="72099-124">string</span><span class="sxs-lookup"><span data-stu-id="72099-124">string</span></span> | <span data-ttu-id="72099-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="72099-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72099-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72099-127">Request body</span></span>
<span data-ttu-id="72099-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="72099-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="72099-129">响应</span><span class="sxs-lookup"><span data-stu-id="72099-129">Response</span></span>
<span data-ttu-id="72099-130">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [businessFlowTemplate](../resources/businessflowtemplate.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="72099-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72099-131">示例</span><span class="sxs-lookup"><span data-stu-id="72099-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72099-132">请求</span><span class="sxs-lookup"><span data-stu-id="72099-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="72099-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="72099-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="72099-134">C#</span><span class="sxs-lookup"><span data-stu-id="72099-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72099-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72099-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72099-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72099-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72099-137">响应</span><span class="sxs-lookup"><span data-stu-id="72099-137">Response</span></span>
><span data-ttu-id="72099-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72099-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="72099-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="72099-140">See also</span></span>

| <span data-ttu-id="72099-141">方法</span><span class="sxs-lookup"><span data-stu-id="72099-141">Method</span></span>           | <span data-ttu-id="72099-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="72099-142">Return Type</span></span>    |<span data-ttu-id="72099-143">说明</span><span class="sxs-lookup"><span data-stu-id="72099-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72099-144">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="72099-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="72099-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="72099-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="72099-146">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="72099-146">Create a new accessReview.</span></span> |




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


