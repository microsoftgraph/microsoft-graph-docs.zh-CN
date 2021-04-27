---
title: 创建程序
description: 在 Azure AD 访问评审功能中，创建新的程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: ba07a60b8414ab259e4ab256175e4dcc6871c00d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052871"
---
# <a name="create-program"></a><span data-ttu-id="2f9d1-103">创建程序</span><span class="sxs-lookup"><span data-stu-id="2f9d1-103">Create program</span></span>

<span data-ttu-id="2f9d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f9d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f9d1-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，创建新的 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f9d1-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f9d1-106">Permissions</span></span>
<span data-ttu-id="2f9d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f9d1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f9d1-109">Permission type</span></span>                        | <span data-ttu-id="2f9d1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f9d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f9d1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f9d1-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9d1-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="2f9d1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f9d1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-114">Not supported.</span></span> |
|<span data-ttu-id="2f9d1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f9d1-115">Application</span></span>                            | <span data-ttu-id="2f9d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-116">Not supported.</span></span> |

<span data-ttu-id="2f9d1-117">登录用户还必须具有允许其创建程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f9d1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f9d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="2f9d1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f9d1-119">Request headers</span></span>
| <span data-ttu-id="2f9d1-120">名称</span><span class="sxs-lookup"><span data-stu-id="2f9d1-120">Name</span></span>         | <span data-ttu-id="2f9d1-121">类型</span><span class="sxs-lookup"><span data-stu-id="2f9d1-121">Type</span></span>        | <span data-ttu-id="2f9d1-122">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d1-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2f9d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f9d1-123">Authorization</span></span> | <span data-ttu-id="2f9d1-124">string</span><span class="sxs-lookup"><span data-stu-id="2f9d1-124">string</span></span> | <span data-ttu-id="2f9d1-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f9d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f9d1-127">Request body</span></span>
<span data-ttu-id="2f9d1-128">在请求正文中，提供 program 对象的 JSON [表示](../resources/program.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="2f9d1-129">下表显示创建程序时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="2f9d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f9d1-130">Property</span></span>     | <span data-ttu-id="2f9d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f9d1-131">Type</span></span>        | <span data-ttu-id="2f9d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d1-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="2f9d1-133">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="2f9d1-134">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="2f9d1-135">响应</span><span class="sxs-lookup"><span data-stu-id="2f9d1-135">Response</span></span>
<span data-ttu-id="2f9d1-136">如果成功，此方法在响应 `201, Created` 正文中返回 [响应](../resources/program.md) 代码和 program 对象。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f9d1-137">示例</span><span class="sxs-lookup"><span data-stu-id="2f9d1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f9d1-138">请求</span><span class="sxs-lookup"><span data-stu-id="2f9d1-138">Request</span></span>
<span data-ttu-id="2f9d1-139">在请求正文中，提供 program 对象的 JSON [表示](../resources/program.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f9d1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f9d1-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2f9d1-141">C#</span><span class="sxs-lookup"><span data-stu-id="2f9d1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f9d1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f9d1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f9d1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f9d1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f9d1-144">Java</span><span class="sxs-lookup"><span data-stu-id="2f9d1-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f9d1-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f9d1-145">Response</span></span>
><span data-ttu-id="2f9d1-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2f9d1-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2f9d1-147">See also</span></span>

| <span data-ttu-id="2f9d1-148">方法</span><span class="sxs-lookup"><span data-stu-id="2f9d1-148">Method</span></span>           | <span data-ttu-id="2f9d1-149">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f9d1-149">Return Type</span></span>    |<span data-ttu-id="2f9d1-150">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d1-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f9d1-151">列出程序</span><span class="sxs-lookup"><span data-stu-id="2f9d1-151">List programs</span></span>](program-list.md) | <span data-ttu-id="2f9d1-152">[program](../resources/program.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f9d1-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="2f9d1-153">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="2f9d1-154">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="2f9d1-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="2f9d1-155">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f9d1-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="2f9d1-156">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="2f9d1-157">更新程序</span><span class="sxs-lookup"><span data-stu-id="2f9d1-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="2f9d1-158">程序</span><span class="sxs-lookup"><span data-stu-id="2f9d1-158">program</span></span>](../resources/program.md)| <span data-ttu-id="2f9d1-159">更新程序。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-159">Update a program.</span></span>|
|[<span data-ttu-id="2f9d1-160">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="2f9d1-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="2f9d1-161">programControl</span><span class="sxs-lookup"><span data-stu-id="2f9d1-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="2f9d1-162">将 programControl 添加到程序。</span><span class="sxs-lookup"><span data-stu-id="2f9d1-162">Add a programControl to a program.</span></span>|

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


