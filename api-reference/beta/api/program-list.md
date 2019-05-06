---
title: 列出程序
description: 在 "Azure AD access 评论" 功能中, 列出所有程序对象。
localization_priority: Normal
ms.openlocfilehash: b71b75119dfeba79df2b326979f87db695427fd4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611268"
---
# <a name="list-programs"></a><span data-ttu-id="ea198-103">列出程序</span><span class="sxs-lookup"><span data-stu-id="ea198-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea198-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea198-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea198-105">权限</span><span class="sxs-lookup"><span data-stu-id="ea198-105">Permissions</span></span>
<span data-ttu-id="ea198-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea198-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea198-108">Permission type</span></span>                        | <span data-ttu-id="ea198-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea198-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea198-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea198-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea198-111">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="ea198-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="ea198-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea198-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea198-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea198-113">Not supported.</span></span> |
|<span data-ttu-id="ea198-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea198-114">Application</span></span>                            | <span data-ttu-id="ea198-115">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="ea198-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="ea198-116">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="ea198-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ea198-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea198-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="ea198-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea198-118">Request headers</span></span>
| <span data-ttu-id="ea198-119">名称</span><span class="sxs-lookup"><span data-stu-id="ea198-119">Name</span></span>         | <span data-ttu-id="ea198-120">类型</span><span class="sxs-lookup"><span data-stu-id="ea198-120">Type</span></span>        | <span data-ttu-id="ea198-121">说明</span><span class="sxs-lookup"><span data-stu-id="ea198-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ea198-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea198-122">Authorization</span></span> | <span data-ttu-id="ea198-123">string</span><span class="sxs-lookup"><span data-stu-id="ea198-123">string</span></span> | <span data-ttu-id="ea198-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea198-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea198-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea198-126">Request body</span></span>
<span data-ttu-id="ea198-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea198-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ea198-128">响应</span><span class="sxs-lookup"><span data-stu-id="ea198-128">Response</span></span>
<span data-ttu-id="ea198-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[program](../resources/program.md)对象数组。</span><span class="sxs-lookup"><span data-stu-id="ea198-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea198-130">示例</span><span class="sxs-lookup"><span data-stu-id="ea198-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea198-131">请求</span><span class="sxs-lookup"><span data-stu-id="ea198-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="ea198-132">响应</span><span class="sxs-lookup"><span data-stu-id="ea198-132">Response</span></span>
><span data-ttu-id="ea198-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ea198-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ea198-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ea198-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ea198-136">语言</span><span class="sxs-lookup"><span data-stu-id="ea198-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea198-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ea198-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="ea198-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ea198-138">See also</span></span>

| <span data-ttu-id="ea198-139">方法</span><span class="sxs-lookup"><span data-stu-id="ea198-139">Method</span></span>           | <span data-ttu-id="ea198-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea198-140">Return Type</span></span>    |<span data-ttu-id="ea198-141">说明</span><span class="sxs-lookup"><span data-stu-id="ea198-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea198-142">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="ea198-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ea198-143">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="ea198-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ea198-144">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="ea198-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
