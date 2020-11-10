---
title: 列出程序
description: 在 "Azure AD access 评论" 功能中，列出所有程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: f16532566f27498f837ec54d4f55b4c40248a507
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966866"
---
# <a name="list-programs"></a><span data-ttu-id="0c346-103">列出程序</span><span class="sxs-lookup"><span data-stu-id="0c346-103">List programs</span></span>

<span data-ttu-id="0c346-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c346-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c346-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，列出所有 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c346-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c346-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c346-106">Permissions</span></span>
<span data-ttu-id="0c346-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c346-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c346-109">Permission type</span></span>                        | <span data-ttu-id="0c346-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c346-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c346-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c346-112">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="0c346-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="0c346-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c346-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c346-114">Not supported.</span></span> |
|<span data-ttu-id="0c346-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c346-115">Application</span></span>                            | <span data-ttu-id="0c346-116">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="0c346-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="0c346-117">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="0c346-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c346-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c346-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="0c346-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c346-119">Request headers</span></span>
| <span data-ttu-id="0c346-120">名称</span><span class="sxs-lookup"><span data-stu-id="0c346-120">Name</span></span>         | <span data-ttu-id="0c346-121">类型</span><span class="sxs-lookup"><span data-stu-id="0c346-121">Type</span></span>        | <span data-ttu-id="0c346-122">说明</span><span class="sxs-lookup"><span data-stu-id="0c346-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0c346-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c346-123">Authorization</span></span> | <span data-ttu-id="0c346-124">string</span><span class="sxs-lookup"><span data-stu-id="0c346-124">string</span></span> | <span data-ttu-id="0c346-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c346-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c346-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c346-127">Request body</span></span>
<span data-ttu-id="0c346-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c346-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0c346-129">响应</span><span class="sxs-lookup"><span data-stu-id="0c346-129">Response</span></span>
<span data-ttu-id="0c346-130">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [program](../resources/program.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="0c346-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c346-131">示例</span><span class="sxs-lookup"><span data-stu-id="0c346-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c346-132">请求</span><span class="sxs-lookup"><span data-stu-id="0c346-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0c346-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c346-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="0c346-134">C#</span><span class="sxs-lookup"><span data-stu-id="0c346-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c346-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c346-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c346-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c346-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c346-137">Java</span><span class="sxs-lookup"><span data-stu-id="0c346-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c346-138">响应</span><span class="sxs-lookup"><span data-stu-id="0c346-138">Response</span></span>
><span data-ttu-id="0c346-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0c346-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="0c346-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0c346-141">See also</span></span>

| <span data-ttu-id="0c346-142">方法</span><span class="sxs-lookup"><span data-stu-id="0c346-142">Method</span></span>           | <span data-ttu-id="0c346-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c346-143">Return Type</span></span>    |<span data-ttu-id="0c346-144">说明</span><span class="sxs-lookup"><span data-stu-id="0c346-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c346-145">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="0c346-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="0c346-146">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c346-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="0c346-147">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="0c346-147">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


