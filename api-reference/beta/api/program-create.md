---
title: 创建程序
description: 在 "Azure AD access 评论" 功能中, 创建一个新的程序对象。
localization_priority: Normal
ms.openlocfilehash: 87f766917499e6e9d1896ccf64f8fbae2bef813b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593659"
---
# <a name="create-program"></a><span data-ttu-id="b705e-103">创建程序</span><span class="sxs-lookup"><span data-stu-id="b705e-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b705e-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b705e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b705e-105">权限</span><span class="sxs-lookup"><span data-stu-id="b705e-105">Permissions</span></span>
<span data-ttu-id="b705e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b705e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b705e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b705e-108">Permission type</span></span>                        | <span data-ttu-id="b705e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b705e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b705e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b705e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b705e-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b705e-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="b705e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b705e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b705e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b705e-113">Not supported.</span></span> |
|<span data-ttu-id="b705e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b705e-114">Application</span></span>                            | <span data-ttu-id="b705e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b705e-115">Not supported.</span></span> |

<span data-ttu-id="b705e-116">登录用户还必须位于允许他们创建程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="b705e-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="b705e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b705e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="b705e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b705e-118">Request headers</span></span>
| <span data-ttu-id="b705e-119">名称</span><span class="sxs-lookup"><span data-stu-id="b705e-119">Name</span></span>         | <span data-ttu-id="b705e-120">类型</span><span class="sxs-lookup"><span data-stu-id="b705e-120">Type</span></span>        | <span data-ttu-id="b705e-121">说明</span><span class="sxs-lookup"><span data-stu-id="b705e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b705e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b705e-122">Authorization</span></span> | <span data-ttu-id="b705e-123">string</span><span class="sxs-lookup"><span data-stu-id="b705e-123">string</span></span> | <span data-ttu-id="b705e-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="b705e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b705e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b705e-126">Request body</span></span>
<span data-ttu-id="b705e-127">在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b705e-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="b705e-128">下表显示创建程序时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b705e-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="b705e-129">属性</span><span class="sxs-lookup"><span data-stu-id="b705e-129">Property</span></span>     | <span data-ttu-id="b705e-130">类型</span><span class="sxs-lookup"><span data-stu-id="b705e-130">Type</span></span>        | <span data-ttu-id="b705e-131">说明</span><span class="sxs-lookup"><span data-stu-id="b705e-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="b705e-132">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="b705e-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="b705e-133">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="b705e-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="b705e-134">响应</span><span class="sxs-lookup"><span data-stu-id="b705e-134">Response</span></span>
<span data-ttu-id="b705e-135">如果成功, 此方法在响应`201, Created`正文中返回响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b705e-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b705e-136">示例</span><span class="sxs-lookup"><span data-stu-id="b705e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b705e-137">请求</span><span class="sxs-lookup"><span data-stu-id="b705e-137">Request</span></span>
<span data-ttu-id="b705e-138">在请求正文中, 提供[程序](../resources/program.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b705e-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b705e-139">响应</span><span class="sxs-lookup"><span data-stu-id="b705e-139">Response</span></span>
><span data-ttu-id="b705e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b705e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b705e-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b705e-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b705e-143">语言</span><span class="sxs-lookup"><span data-stu-id="b705e-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b705e-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b705e-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="b705e-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b705e-145">See also</span></span>

| <span data-ttu-id="b705e-146">方法</span><span class="sxs-lookup"><span data-stu-id="b705e-146">Method</span></span>           | <span data-ttu-id="b705e-147">返回类型</span><span class="sxs-lookup"><span data-stu-id="b705e-147">Return Type</span></span>    |<span data-ttu-id="b705e-148">说明</span><span class="sxs-lookup"><span data-stu-id="b705e-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b705e-149">列出程序</span><span class="sxs-lookup"><span data-stu-id="b705e-149">List programs</span></span>](program-list.md) | <span data-ttu-id="b705e-150">[程序](../resources/program.md)集</span><span class="sxs-lookup"><span data-stu-id="b705e-150">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="b705e-151">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="b705e-151">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b705e-152">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="b705e-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b705e-153">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="b705e-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b705e-154">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="b705e-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b705e-155">更新程序</span><span class="sxs-lookup"><span data-stu-id="b705e-155">Update program</span></span>](program-update.md) |  [<span data-ttu-id="b705e-156">主程序</span><span class="sxs-lookup"><span data-stu-id="b705e-156">program</span></span>](../resources/program.md)| <span data-ttu-id="b705e-157">更新程序。</span><span class="sxs-lookup"><span data-stu-id="b705e-157">Update a program.</span></span>|
|[<span data-ttu-id="b705e-158">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="b705e-158">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="b705e-159">programControl</span><span class="sxs-lookup"><span data-stu-id="b705e-159">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="b705e-160">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="b705e-160">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
