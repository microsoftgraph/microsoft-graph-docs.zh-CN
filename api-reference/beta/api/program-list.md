---
title: 列出程序
description: 在 Azure AD 访问评审功能中，列出所有程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 4995cd66af99031051e67a2853f4a2453430f684
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049833"
---
# <a name="list-programs"></a><span data-ttu-id="95cd5-103">列出程序</span><span class="sxs-lookup"><span data-stu-id="95cd5-103">List programs</span></span>

<span data-ttu-id="95cd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95cd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95cd5-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，列出所有 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95cd5-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="95cd5-106">权限</span><span class="sxs-lookup"><span data-stu-id="95cd5-106">Permissions</span></span>
<span data-ttu-id="95cd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95cd5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="95cd5-109">Permission type</span></span>                        | <span data-ttu-id="95cd5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95cd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="95cd5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95cd5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95cd5-112">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95cd5-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="95cd5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95cd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95cd5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="95cd5-114">Not supported.</span></span> |
|<span data-ttu-id="95cd5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="95cd5-115">Application</span></span>                            | <span data-ttu-id="95cd5-116">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95cd5-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="95cd5-117">登录用户还必须具有允许其读取程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="95cd5-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="95cd5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95cd5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="95cd5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95cd5-119">Request headers</span></span>
| <span data-ttu-id="95cd5-120">名称</span><span class="sxs-lookup"><span data-stu-id="95cd5-120">Name</span></span>         | <span data-ttu-id="95cd5-121">类型</span><span class="sxs-lookup"><span data-stu-id="95cd5-121">Type</span></span>        | <span data-ttu-id="95cd5-122">说明</span><span class="sxs-lookup"><span data-stu-id="95cd5-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="95cd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95cd5-123">Authorization</span></span> | <span data-ttu-id="95cd5-124">string</span><span class="sxs-lookup"><span data-stu-id="95cd5-124">string</span></span> | <span data-ttu-id="95cd5-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="95cd5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95cd5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95cd5-127">Request body</span></span>
<span data-ttu-id="95cd5-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="95cd5-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="95cd5-129">响应</span><span class="sxs-lookup"><span data-stu-id="95cd5-129">Response</span></span>
<span data-ttu-id="95cd5-130">如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [program](../resources/program.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="95cd5-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95cd5-131">示例</span><span class="sxs-lookup"><span data-stu-id="95cd5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95cd5-132">请求</span><span class="sxs-lookup"><span data-stu-id="95cd5-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="95cd5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="95cd5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="95cd5-134">C#</span><span class="sxs-lookup"><span data-stu-id="95cd5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95cd5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95cd5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95cd5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95cd5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95cd5-137">Java</span><span class="sxs-lookup"><span data-stu-id="95cd5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95cd5-138">响应</span><span class="sxs-lookup"><span data-stu-id="95cd5-138">Response</span></span>
><span data-ttu-id="95cd5-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95cd5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="95cd5-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="95cd5-140">See also</span></span>

| <span data-ttu-id="95cd5-141">方法</span><span class="sxs-lookup"><span data-stu-id="95cd5-141">Method</span></span>           | <span data-ttu-id="95cd5-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="95cd5-142">Return Type</span></span>    |<span data-ttu-id="95cd5-143">说明</span><span class="sxs-lookup"><span data-stu-id="95cd5-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95cd5-144">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="95cd5-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="95cd5-145">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95cd5-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="95cd5-146">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="95cd5-146">Get a collection of the controls of a program.</span></span>|


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


