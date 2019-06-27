---
title: 创建 programControl
description: 在 "Azure AD access 评论" 功能中, 创建一个新的 programControl 对象。  这会将访问审核链接到某个程序。
localization_priority: Normal
ms.openlocfilehash: 822b9c58651eb1a997b00553f34f40e1d7b9886d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268017"
---
# <a name="create-programcontrol"></a><span data-ttu-id="c026c-104">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="c026c-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c026c-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c026c-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="c026c-106">这会将访问审核链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="c026c-106">This links an access review to a program.</span></span>

<span data-ttu-id="c026c-107">在发出此请求之前, 呼叫者必须先</span><span class="sxs-lookup"><span data-stu-id="c026c-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="c026c-108">[创建了一个程序](program-create.md)或[检索了一个程序](program-list.md), 以使`programId`其值包含在请求中,</span><span class="sxs-lookup"><span data-stu-id="c026c-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="c026c-109">[创建了访问](accessreview-create.md)审核或[检索到访问审核](accessreview-get.md), 以在请求中包含`controlId`的值, 以及</span><span class="sxs-lookup"><span data-stu-id="c026c-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="c026c-110">[检索了程序控制类型的列表](programcontroltype-list.md), 以将值`controlTypeId`包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="c026c-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="c026c-111">权限</span><span class="sxs-lookup"><span data-stu-id="c026c-111">Permissions</span></span>
<span data-ttu-id="c026c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c026c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c026c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c026c-114">Permission type</span></span>                        | <span data-ttu-id="c026c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c026c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c026c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c026c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c026c-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c026c-117">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="c026c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c026c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c026c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c026c-119">Not supported.</span></span> |
|<span data-ttu-id="c026c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c026c-120">Application</span></span>                            |  <span data-ttu-id="c026c-121">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c026c-121">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="c026c-122">登录用户还必须位于允许他们创建**programControl**的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="c026c-122">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="c026c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c026c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="c026c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c026c-124">Request headers</span></span>
| <span data-ttu-id="c026c-125">名称</span><span class="sxs-lookup"><span data-stu-id="c026c-125">Name</span></span>         | <span data-ttu-id="c026c-126">类型</span><span class="sxs-lookup"><span data-stu-id="c026c-126">Type</span></span>        | <span data-ttu-id="c026c-127">说明</span><span class="sxs-lookup"><span data-stu-id="c026c-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c026c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c026c-128">Authorization</span></span> | <span data-ttu-id="c026c-129">string</span><span class="sxs-lookup"><span data-stu-id="c026c-129">string</span></span> | <span data-ttu-id="c026c-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c026c-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c026c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c026c-132">Request body</span></span>
<span data-ttu-id="c026c-133">在请求正文中, 提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c026c-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="c026c-134">下表显示创建程序控件时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c026c-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="c026c-135">属性</span><span class="sxs-lookup"><span data-stu-id="c026c-135">Property</span></span>     | <span data-ttu-id="c026c-136">类型</span><span class="sxs-lookup"><span data-stu-id="c026c-136">Type</span></span>        | <span data-ttu-id="c026c-137">说明</span><span class="sxs-lookup"><span data-stu-id="c026c-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="c026c-138">此控件将要成为的程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="c026c-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="c026c-139">控件的 controlId, 特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="c026c-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="c026c-140">ProgramControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="c026c-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="c026c-141">响应</span><span class="sxs-lookup"><span data-stu-id="c026c-141">Response</span></span>
<span data-ttu-id="c026c-142">如果成功, 此方法在响应`201, Created`正文中返回响应代码和[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c026c-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c026c-143">示例</span><span class="sxs-lookup"><span data-stu-id="c026c-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c026c-144">请求</span><span class="sxs-lookup"><span data-stu-id="c026c-144">Request</span></span>
<span data-ttu-id="c026c-145">在请求正文中, 提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c026c-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="c026c-146">响应</span><span class="sxs-lookup"><span data-stu-id="c026c-146">Response</span></span>
><span data-ttu-id="c026c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c026c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c026c-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c026c-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c026c-150">C#</span><span class="sxs-lookup"><span data-stu-id="c026c-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c026c-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="c026c-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c026c-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="c026c-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="c026c-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c026c-153">See also</span></span>

| <span data-ttu-id="c026c-154">方法</span><span class="sxs-lookup"><span data-stu-id="c026c-154">Method</span></span>           | <span data-ttu-id="c026c-155">返回类型</span><span class="sxs-lookup"><span data-stu-id="c026c-155">Return Type</span></span>    |<span data-ttu-id="c026c-156">说明</span><span class="sxs-lookup"><span data-stu-id="c026c-156">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c026c-157">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="c026c-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="c026c-158">[programControlType](../resources/programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="c026c-158">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="c026c-159">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="c026c-159">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
