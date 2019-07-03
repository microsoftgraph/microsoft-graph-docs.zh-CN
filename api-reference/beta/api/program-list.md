---
title: 列出程序
description: 在 "Azure AD access 评论" 功能中, 列出所有程序对象。
localization_priority: Normal
ms.openlocfilehash: 8919e67df0b2f77279df1324483d8524de8aa2ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455341"
---
# <a name="list-programs"></a><span data-ttu-id="62b2a-103">列出程序</span><span class="sxs-lookup"><span data-stu-id="62b2a-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62b2a-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62b2a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="62b2a-105">权限</span><span class="sxs-lookup"><span data-stu-id="62b2a-105">Permissions</span></span>
<span data-ttu-id="62b2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b2a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62b2a-108">Permission type</span></span>                        | <span data-ttu-id="62b2a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62b2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="62b2a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62b2a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62b2a-111">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="62b2a-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="62b2a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62b2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62b2a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="62b2a-113">Not supported.</span></span> |
|<span data-ttu-id="62b2a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="62b2a-114">Application</span></span>                            | <span data-ttu-id="62b2a-115">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="62b2a-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="62b2a-116">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="62b2a-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="62b2a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62b2a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="62b2a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62b2a-118">Request headers</span></span>
| <span data-ttu-id="62b2a-119">名称</span><span class="sxs-lookup"><span data-stu-id="62b2a-119">Name</span></span>         | <span data-ttu-id="62b2a-120">类型</span><span class="sxs-lookup"><span data-stu-id="62b2a-120">Type</span></span>        | <span data-ttu-id="62b2a-121">说明</span><span class="sxs-lookup"><span data-stu-id="62b2a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="62b2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b2a-122">Authorization</span></span> | <span data-ttu-id="62b2a-123">string</span><span class="sxs-lookup"><span data-stu-id="62b2a-123">string</span></span> | <span data-ttu-id="62b2a-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="62b2a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62b2a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="62b2a-126">Request body</span></span>
<span data-ttu-id="62b2a-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="62b2a-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="62b2a-128">响应</span><span class="sxs-lookup"><span data-stu-id="62b2a-128">Response</span></span>
<span data-ttu-id="62b2a-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[program](../resources/program.md)对象数组。</span><span class="sxs-lookup"><span data-stu-id="62b2a-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b2a-130">示例</span><span class="sxs-lookup"><span data-stu-id="62b2a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62b2a-131">请求</span><span class="sxs-lookup"><span data-stu-id="62b2a-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62b2a-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="62b2a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62b2a-133">C#</span><span class="sxs-lookup"><span data-stu-id="62b2a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62b2a-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="62b2a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62b2a-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="62b2a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="62b2a-136">响应</span><span class="sxs-lookup"><span data-stu-id="62b2a-136">Response</span></span>
><span data-ttu-id="62b2a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62b2a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="62b2a-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="62b2a-139">See also</span></span>

| <span data-ttu-id="62b2a-140">方法</span><span class="sxs-lookup"><span data-stu-id="62b2a-140">Method</span></span>           | <span data-ttu-id="62b2a-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="62b2a-141">Return Type</span></span>    |<span data-ttu-id="62b2a-142">说明</span><span class="sxs-lookup"><span data-stu-id="62b2a-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="62b2a-143">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="62b2a-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="62b2a-144">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="62b2a-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="62b2a-145">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="62b2a-145">Get a collection of the controls of a program.</span></span>|


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
