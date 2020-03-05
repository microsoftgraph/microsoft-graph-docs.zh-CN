---
title: 创建程序
description: 在 "Azure AD access 评论" 功能中，创建一个新的程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f7d51254d9ecf67861eb93f45c1db6a868b6ad33
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455016"
---
# <a name="create-program"></a><span data-ttu-id="b467f-103">创建程序</span><span class="sxs-lookup"><span data-stu-id="b467f-103">Create program</span></span>

<span data-ttu-id="b467f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b467f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b467f-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，创建一个新的[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b467f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b467f-106">权限</span><span class="sxs-lookup"><span data-stu-id="b467f-106">Permissions</span></span>
<span data-ttu-id="b467f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b467f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b467f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b467f-109">Permission type</span></span>                        | <span data-ttu-id="b467f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b467f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b467f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b467f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b467f-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b467f-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="b467f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b467f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b467f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b467f-114">Not supported.</span></span> |
|<span data-ttu-id="b467f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b467f-115">Application</span></span>                            | <span data-ttu-id="b467f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b467f-116">Not supported.</span></span> |

<span data-ttu-id="b467f-117">登录用户还必须位于允许他们创建程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="b467f-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="b467f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b467f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="b467f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b467f-119">Request headers</span></span>
| <span data-ttu-id="b467f-120">名称</span><span class="sxs-lookup"><span data-stu-id="b467f-120">Name</span></span>         | <span data-ttu-id="b467f-121">类型</span><span class="sxs-lookup"><span data-stu-id="b467f-121">Type</span></span>        | <span data-ttu-id="b467f-122">说明</span><span class="sxs-lookup"><span data-stu-id="b467f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b467f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b467f-123">Authorization</span></span> | <span data-ttu-id="b467f-124">string</span><span class="sxs-lookup"><span data-stu-id="b467f-124">string</span></span> | <span data-ttu-id="b467f-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="b467f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b467f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b467f-127">Request body</span></span>
<span data-ttu-id="b467f-128">在请求正文中，提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b467f-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="b467f-129">下表显示创建程序时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b467f-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="b467f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b467f-130">Property</span></span>     | <span data-ttu-id="b467f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b467f-131">Type</span></span>        | <span data-ttu-id="b467f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b467f-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="b467f-133">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="b467f-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="b467f-134">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="b467f-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="b467f-135">响应</span><span class="sxs-lookup"><span data-stu-id="b467f-135">Response</span></span>
<span data-ttu-id="b467f-136">如果成功，此方法在响应`201, Created`正文中返回响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b467f-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b467f-137">示例</span><span class="sxs-lookup"><span data-stu-id="b467f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b467f-138">请求</span><span class="sxs-lookup"><span data-stu-id="b467f-138">Request</span></span>
<span data-ttu-id="b467f-139">在请求正文中，提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b467f-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="b467f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b467f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="c"></a>[<span data-ttu-id="b467f-141">C#</span><span class="sxs-lookup"><span data-stu-id="b467f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b467f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b467f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b467f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b467f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b467f-144">响应</span><span class="sxs-lookup"><span data-stu-id="b467f-144">Response</span></span>
><span data-ttu-id="b467f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b467f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="b467f-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b467f-147">See also</span></span>

| <span data-ttu-id="b467f-148">方法</span><span class="sxs-lookup"><span data-stu-id="b467f-148">Method</span></span>           | <span data-ttu-id="b467f-149">返回类型</span><span class="sxs-lookup"><span data-stu-id="b467f-149">Return Type</span></span>    |<span data-ttu-id="b467f-150">说明</span><span class="sxs-lookup"><span data-stu-id="b467f-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b467f-151">列出程序</span><span class="sxs-lookup"><span data-stu-id="b467f-151">List programs</span></span>](program-list.md) | <span data-ttu-id="b467f-152">[程序](../resources/program.md)集</span><span class="sxs-lookup"><span data-stu-id="b467f-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="b467f-153">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="b467f-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b467f-154">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="b467f-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b467f-155">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="b467f-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b467f-156">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="b467f-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b467f-157">更新程序</span><span class="sxs-lookup"><span data-stu-id="b467f-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="b467f-158">主程序</span><span class="sxs-lookup"><span data-stu-id="b467f-158">program</span></span>](../resources/program.md)| <span data-ttu-id="b467f-159">更新程序。</span><span class="sxs-lookup"><span data-stu-id="b467f-159">Update a program.</span></span>|
|[<span data-ttu-id="b467f-160">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="b467f-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="b467f-161">programControl</span><span class="sxs-lookup"><span data-stu-id="b467f-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="b467f-162">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="b467f-162">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
