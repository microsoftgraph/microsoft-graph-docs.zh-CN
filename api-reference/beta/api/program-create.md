---
title: 创建程序
description: 在 "Azure AD access 评论" 功能中, 创建一个新的程序对象。
localization_priority: Normal
ms.openlocfilehash: 0d2218031e924e7137378a63d932f5533620cc38
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267660"
---
# <a name="create-program"></a><span data-ttu-id="9c5dd-103">创建程序</span><span class="sxs-lookup"><span data-stu-id="9c5dd-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c5dd-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c5dd-105">权限</span><span class="sxs-lookup"><span data-stu-id="9c5dd-105">Permissions</span></span>
<span data-ttu-id="9c5dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c5dd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c5dd-108">Permission type</span></span>                        | <span data-ttu-id="9c5dd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c5dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c5dd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c5dd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c5dd-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c5dd-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="9c5dd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c5dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c5dd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-113">Not supported.</span></span> |
|<span data-ttu-id="9c5dd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c5dd-114">Application</span></span>                            | <span data-ttu-id="9c5dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-115">Not supported.</span></span> |

<span data-ttu-id="9c5dd-116">登录用户还必须位于允许他们创建程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="9c5dd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c5dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="9c5dd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c5dd-118">Request headers</span></span>
| <span data-ttu-id="9c5dd-119">名称</span><span class="sxs-lookup"><span data-stu-id="9c5dd-119">Name</span></span>         | <span data-ttu-id="9c5dd-120">类型</span><span class="sxs-lookup"><span data-stu-id="9c5dd-120">Type</span></span>        | <span data-ttu-id="9c5dd-121">说明</span><span class="sxs-lookup"><span data-stu-id="9c5dd-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9c5dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c5dd-122">Authorization</span></span> | <span data-ttu-id="9c5dd-123">string</span><span class="sxs-lookup"><span data-stu-id="9c5dd-123">string</span></span> | <span data-ttu-id="9c5dd-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c5dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c5dd-126">Request body</span></span>
<span data-ttu-id="9c5dd-127">在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="9c5dd-128">下表显示创建程序时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="9c5dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="9c5dd-129">Property</span></span>     | <span data-ttu-id="9c5dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="9c5dd-130">Type</span></span>        | <span data-ttu-id="9c5dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="9c5dd-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="9c5dd-132">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="9c5dd-133">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="9c5dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c5dd-134">Response</span></span>
<span data-ttu-id="9c5dd-135">如果成功, 此方法在响应`201, Created`正文中返回响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c5dd-136">示例</span><span class="sxs-lookup"><span data-stu-id="9c5dd-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c5dd-137">请求</span><span class="sxs-lookup"><span data-stu-id="9c5dd-137">Request</span></span>
<span data-ttu-id="9c5dd-138">在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="9c5dd-139">响应</span><span class="sxs-lookup"><span data-stu-id="9c5dd-139">Response</span></span>
><span data-ttu-id="9c5dd-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9c5dd-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9c5dd-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9c5dd-143">C#</span><span class="sxs-lookup"><span data-stu-id="9c5dd-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c5dd-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c5dd-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9c5dd-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="9c5dd-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="9c5dd-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9c5dd-146">See also</span></span>

| <span data-ttu-id="9c5dd-147">方法</span><span class="sxs-lookup"><span data-stu-id="9c5dd-147">Method</span></span>           | <span data-ttu-id="9c5dd-148">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c5dd-148">Return Type</span></span>    |<span data-ttu-id="9c5dd-149">说明</span><span class="sxs-lookup"><span data-stu-id="9c5dd-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c5dd-150">列出程序</span><span class="sxs-lookup"><span data-stu-id="9c5dd-150">List programs</span></span>](program-list.md) | <span data-ttu-id="9c5dd-151">[程序](../resources/program.md)集</span><span class="sxs-lookup"><span data-stu-id="9c5dd-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="9c5dd-152">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="9c5dd-153">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="9c5dd-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="9c5dd-154">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="9c5dd-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="9c5dd-155">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="9c5dd-156">更新程序</span><span class="sxs-lookup"><span data-stu-id="9c5dd-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="9c5dd-157">主程序</span><span class="sxs-lookup"><span data-stu-id="9c5dd-157">program</span></span>](../resources/program.md)| <span data-ttu-id="9c5dd-158">更新程序。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-158">Update a program.</span></span>|
|[<span data-ttu-id="9c5dd-159">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="9c5dd-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="9c5dd-160">programControl</span><span class="sxs-lookup"><span data-stu-id="9c5dd-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="9c5dd-161">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="9c5dd-161">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
