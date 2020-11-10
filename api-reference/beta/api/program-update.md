---
title: 更新程序
description: 在 "Azure AD access 评论" 功能中，更新现有的程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: f8651a867ae53fb191983731aa1dff29735ee535
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963507"
---
# <a name="update-program"></a><span data-ttu-id="6fc53-103">更新程序</span><span class="sxs-lookup"><span data-stu-id="6fc53-103">Update program</span></span>

<span data-ttu-id="6fc53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fc53-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，更新现有的 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fc53-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fc53-106">权限</span><span class="sxs-lookup"><span data-stu-id="6fc53-106">Permissions</span></span>
<span data-ttu-id="6fc53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fc53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fc53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fc53-109">Permission type</span></span>                        | <span data-ttu-id="6fc53-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fc53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fc53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fc53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fc53-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fc53-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="6fc53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fc53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fc53-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fc53-114">Not supported.</span></span> |
|<span data-ttu-id="6fc53-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fc53-115">Application</span></span>                            | <span data-ttu-id="6fc53-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fc53-116">Not supported.</span></span> |

<span data-ttu-id="6fc53-117">登录用户还必须位于允许他们更新程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="6fc53-117">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="6fc53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fc53-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="6fc53-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fc53-119">Request headers</span></span>
| <span data-ttu-id="6fc53-120">名称</span><span class="sxs-lookup"><span data-stu-id="6fc53-120">Name</span></span>         | <span data-ttu-id="6fc53-121">类型</span><span class="sxs-lookup"><span data-stu-id="6fc53-121">Type</span></span>        | <span data-ttu-id="6fc53-122">说明</span><span class="sxs-lookup"><span data-stu-id="6fc53-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6fc53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fc53-123">Authorization</span></span> | <span data-ttu-id="6fc53-124">string</span><span class="sxs-lookup"><span data-stu-id="6fc53-124">string</span></span> | <span data-ttu-id="6fc53-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fc53-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fc53-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fc53-127">Request body</span></span>
<span data-ttu-id="6fc53-128">在请求正文中，提供 [程序](../resources/program.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc53-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="6fc53-129">下表显示了在更新程序时可以提供的属性。</span><span class="sxs-lookup"><span data-stu-id="6fc53-129">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="6fc53-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fc53-130">Property</span></span>     | <span data-ttu-id="6fc53-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fc53-131">Type</span></span>        | <span data-ttu-id="6fc53-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fc53-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="6fc53-133">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6fc53-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="6fc53-134">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="6fc53-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="6fc53-135">响应</span><span class="sxs-lookup"><span data-stu-id="6fc53-135">Response</span></span>
<span data-ttu-id="6fc53-136">如果成功，此方法 `204, Accepted` 在响应正文中返回响应代码和 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fc53-136">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fc53-137">示例</span><span class="sxs-lookup"><span data-stu-id="6fc53-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fc53-138">请求</span><span class="sxs-lookup"><span data-stu-id="6fc53-138">Request</span></span>
<span data-ttu-id="6fc53-139">在请求正文中，提供要更改的 [program](../resources/program.md) 对象参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc53-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="http"></a>[<span data-ttu-id="6fc53-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fc53-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```
# <a name="c"></a>[<span data-ttu-id="6fc53-141">C#</span><span class="sxs-lookup"><span data-stu-id="6fc53-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fc53-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fc53-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fc53-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fc53-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fc53-144">Java</span><span class="sxs-lookup"><span data-stu-id="6fc53-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6fc53-145">响应</span><span class="sxs-lookup"><span data-stu-id="6fc53-145">Response</span></span>
><span data-ttu-id="6fc53-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6fc53-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="6fc53-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6fc53-148">See also</span></span>

| <span data-ttu-id="6fc53-149">方法</span><span class="sxs-lookup"><span data-stu-id="6fc53-149">Method</span></span>           | <span data-ttu-id="6fc53-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fc53-150">Return Type</span></span>    |<span data-ttu-id="6fc53-151">说明</span><span class="sxs-lookup"><span data-stu-id="6fc53-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6fc53-152">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="6fc53-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="6fc53-153">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc53-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="6fc53-154">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="6fc53-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="6fc53-155">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="6fc53-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="6fc53-156">programControl</span><span class="sxs-lookup"><span data-stu-id="6fc53-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="6fc53-157">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="6fc53-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


