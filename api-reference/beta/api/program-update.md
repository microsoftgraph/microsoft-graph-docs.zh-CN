---
title: 更新程序
description: 在 Azure AD 访问评审功能中，更新现有程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b1e601908a8f12523f9e02549e3fd24903e77bda
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442220"
---
# <a name="update-program"></a><span data-ttu-id="33ea6-103">更新程序</span><span class="sxs-lookup"><span data-stu-id="33ea6-103">Update program</span></span>

<span data-ttu-id="33ea6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33ea6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33ea6-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33ea6-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33ea6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="33ea6-106">Permissions</span></span>
<span data-ttu-id="33ea6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33ea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33ea6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="33ea6-109">Permission type</span></span>                        | <span data-ttu-id="33ea6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33ea6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="33ea6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33ea6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33ea6-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ea6-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="33ea6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33ea6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33ea6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33ea6-114">Not supported.</span></span> |
|<span data-ttu-id="33ea6-115">Application</span><span class="sxs-lookup"><span data-stu-id="33ea6-115">Application</span></span>                            | <span data-ttu-id="33ea6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33ea6-116">Not supported.</span></span> |

<span data-ttu-id="33ea6-117">登录用户还必须是允许其更新程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="33ea6-117">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="33ea6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33ea6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="33ea6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="33ea6-119">Request headers</span></span>
| <span data-ttu-id="33ea6-120">名称</span><span class="sxs-lookup"><span data-stu-id="33ea6-120">Name</span></span>         | <span data-ttu-id="33ea6-121">类型</span><span class="sxs-lookup"><span data-stu-id="33ea6-121">Type</span></span>        | <span data-ttu-id="33ea6-122">说明</span><span class="sxs-lookup"><span data-stu-id="33ea6-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="33ea6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33ea6-123">Authorization</span></span> | <span data-ttu-id="33ea6-124">string</span><span class="sxs-lookup"><span data-stu-id="33ea6-124">string</span></span> | <span data-ttu-id="33ea6-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="33ea6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33ea6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="33ea6-127">Request body</span></span>
<span data-ttu-id="33ea6-128">在请求正文中，提供程序对象的 JSON [表示形式](../resources/program.md) 。</span><span class="sxs-lookup"><span data-stu-id="33ea6-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="33ea6-129">下表显示更新程序时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="33ea6-129">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="33ea6-130">属性</span><span class="sxs-lookup"><span data-stu-id="33ea6-130">Property</span></span>     | <span data-ttu-id="33ea6-131">类型</span><span class="sxs-lookup"><span data-stu-id="33ea6-131">Type</span></span>        | <span data-ttu-id="33ea6-132">说明</span><span class="sxs-lookup"><span data-stu-id="33ea6-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="33ea6-133">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="33ea6-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="33ea6-134">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="33ea6-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="33ea6-135">响应</span><span class="sxs-lookup"><span data-stu-id="33ea6-135">Response</span></span>
<span data-ttu-id="33ea6-136">如果成功，此方法在响应正文中返回 `204, Accepted` 响应[](../resources/program.md)代码和 program 对象。</span><span class="sxs-lookup"><span data-stu-id="33ea6-136">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33ea6-137">示例</span><span class="sxs-lookup"><span data-stu-id="33ea6-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33ea6-138">请求</span><span class="sxs-lookup"><span data-stu-id="33ea6-138">Request</span></span>
<span data-ttu-id="33ea6-139">在请求正文中，提供要更改 [的程序](../resources/program.md) 对象参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33ea6-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="http"></a>[<span data-ttu-id="33ea6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="33ea6-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33ea6-141">C#</span><span class="sxs-lookup"><span data-stu-id="33ea6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33ea6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33ea6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33ea6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33ea6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33ea6-144">Java</span><span class="sxs-lookup"><span data-stu-id="33ea6-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33ea6-145">响应</span><span class="sxs-lookup"><span data-stu-id="33ea6-145">Response</span></span>
><span data-ttu-id="33ea6-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33ea6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="33ea6-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="33ea6-148">See also</span></span>

| <span data-ttu-id="33ea6-149">方法</span><span class="sxs-lookup"><span data-stu-id="33ea6-149">Method</span></span>           | <span data-ttu-id="33ea6-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="33ea6-150">Return Type</span></span>    |<span data-ttu-id="33ea6-151">说明</span><span class="sxs-lookup"><span data-stu-id="33ea6-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33ea6-152">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="33ea6-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="33ea6-153">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33ea6-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="33ea6-154">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="33ea6-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="33ea6-155">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="33ea6-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="33ea6-156">programControl</span><span class="sxs-lookup"><span data-stu-id="33ea6-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="33ea6-157">将 programControl 添加到程序。</span><span class="sxs-lookup"><span data-stu-id="33ea6-157">Add a programControl to a program.</span></span>|

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


