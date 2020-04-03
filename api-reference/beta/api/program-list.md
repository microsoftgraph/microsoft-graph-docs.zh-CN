---
title: 列出程序
description: 在 "Azure AD access 评论" 功能中，列出所有程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: eab96053d43634cd4280e2e633b1de5da8ff5a17
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123060"
---
# <a name="list-programs"></a><span data-ttu-id="161ed-103">列出程序</span><span class="sxs-lookup"><span data-stu-id="161ed-103">List programs</span></span>

<span data-ttu-id="161ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="161ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="161ed-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，列出所有[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="161ed-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="161ed-106">权限</span><span class="sxs-lookup"><span data-stu-id="161ed-106">Permissions</span></span>
<span data-ttu-id="161ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="161ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="161ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="161ed-109">Permission type</span></span>                        | <span data-ttu-id="161ed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="161ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="161ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="161ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="161ed-112">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="161ed-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="161ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="161ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="161ed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="161ed-114">Not supported.</span></span> |
|<span data-ttu-id="161ed-115">Application</span><span class="sxs-lookup"><span data-stu-id="161ed-115">Application</span></span>                            | <span data-ttu-id="161ed-116">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="161ed-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="161ed-117">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="161ed-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="161ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="161ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="161ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="161ed-119">Request headers</span></span>
| <span data-ttu-id="161ed-120">名称</span><span class="sxs-lookup"><span data-stu-id="161ed-120">Name</span></span>         | <span data-ttu-id="161ed-121">类型</span><span class="sxs-lookup"><span data-stu-id="161ed-121">Type</span></span>        | <span data-ttu-id="161ed-122">说明</span><span class="sxs-lookup"><span data-stu-id="161ed-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="161ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="161ed-123">Authorization</span></span> | <span data-ttu-id="161ed-124">string</span><span class="sxs-lookup"><span data-stu-id="161ed-124">string</span></span> | <span data-ttu-id="161ed-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="161ed-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="161ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="161ed-127">Request body</span></span>
<span data-ttu-id="161ed-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="161ed-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="161ed-129">响应</span><span class="sxs-lookup"><span data-stu-id="161ed-129">Response</span></span>
<span data-ttu-id="161ed-130">如果成功，此方法在响应`200, OK`正文中返回响应代码和[program](../resources/program.md)对象数组。</span><span class="sxs-lookup"><span data-stu-id="161ed-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="161ed-131">示例</span><span class="sxs-lookup"><span data-stu-id="161ed-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="161ed-132">请求</span><span class="sxs-lookup"><span data-stu-id="161ed-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="161ed-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="161ed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="161ed-134">C#</span><span class="sxs-lookup"><span data-stu-id="161ed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="161ed-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="161ed-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="161ed-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="161ed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="161ed-137">响应</span><span class="sxs-lookup"><span data-stu-id="161ed-137">Response</span></span>
><span data-ttu-id="161ed-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="161ed-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="161ed-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="161ed-140">See also</span></span>

| <span data-ttu-id="161ed-141">方法</span><span class="sxs-lookup"><span data-stu-id="161ed-141">Method</span></span>           | <span data-ttu-id="161ed-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="161ed-142">Return Type</span></span>    |<span data-ttu-id="161ed-143">说明</span><span class="sxs-lookup"><span data-stu-id="161ed-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="161ed-144">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="161ed-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="161ed-145">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="161ed-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="161ed-146">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="161ed-146">Get a collection of the controls of a program.</span></span>|


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
