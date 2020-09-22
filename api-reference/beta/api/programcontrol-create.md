---
title: 创建 programControl
description: 在 "Azure AD access 评论" 功能中，创建一个新的 programControl 对象。  这会将访问审核链接到某个程序。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: f27094a28423137eb6c8e9661b42449f9cf7ac6c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986229"
---
# <a name="create-programcontrol"></a><span data-ttu-id="dad08-104">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="dad08-104">Create programControl</span></span>

<span data-ttu-id="dad08-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad08-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dad08-106">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，创建一个新的 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dad08-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="dad08-107">这会将访问审核链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="dad08-107">This links an access review to a program.</span></span>

<span data-ttu-id="dad08-108">在发出此请求之前，呼叫者必须先</span><span class="sxs-lookup"><span data-stu-id="dad08-108">Prior to making this request, the caller must have previously</span></span>

- <span data-ttu-id="dad08-109">[创建了一个程序](program-create.md) 或 [检索了一个程序](program-list.md)，以使 `programId` 其值包含在请求中，</span><span class="sxs-lookup"><span data-stu-id="dad08-109">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
- <span data-ttu-id="dad08-110">[创建了访问](accessreview-create.md) 审核或 [检索到访问审核](accessreview-get.md)，以 `controlId` 在请求中包含的值，以及</span><span class="sxs-lookup"><span data-stu-id="dad08-110">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
- <span data-ttu-id="dad08-111">[检索了程序控制类型的列表](programcontroltype-list.md)，以将值 `controlTypeId` 包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="dad08-111">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="dad08-112">权限</span><span class="sxs-lookup"><span data-stu-id="dad08-112">Permissions</span></span>
<span data-ttu-id="dad08-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dad08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad08-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="dad08-115">Permission type</span></span>                        | <span data-ttu-id="dad08-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dad08-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dad08-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dad08-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="dad08-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad08-118">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="dad08-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dad08-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dad08-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="dad08-120">Not supported.</span></span> |
|<span data-ttu-id="dad08-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="dad08-121">Application</span></span>                            |  <span data-ttu-id="dad08-122">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad08-122">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="dad08-123">登录用户还必须位于允许他们创建 **programControl**的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="dad08-123">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="dad08-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dad08-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="dad08-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="dad08-125">Request headers</span></span>
| <span data-ttu-id="dad08-126">名称</span><span class="sxs-lookup"><span data-stu-id="dad08-126">Name</span></span>         | <span data-ttu-id="dad08-127">类型</span><span class="sxs-lookup"><span data-stu-id="dad08-127">Type</span></span>        | <span data-ttu-id="dad08-128">说明</span><span class="sxs-lookup"><span data-stu-id="dad08-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dad08-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="dad08-129">Authorization</span></span> | <span data-ttu-id="dad08-130">string</span><span class="sxs-lookup"><span data-stu-id="dad08-130">string</span></span> | <span data-ttu-id="dad08-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="dad08-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dad08-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="dad08-133">Request body</span></span>
<span data-ttu-id="dad08-134">在请求正文中，提供 [programControl](../resources/programcontrol.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dad08-134">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="dad08-135">下表显示创建程序控件时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dad08-135">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="dad08-136">属性</span><span class="sxs-lookup"><span data-stu-id="dad08-136">Property</span></span>     | <span data-ttu-id="dad08-137">类型</span><span class="sxs-lookup"><span data-stu-id="dad08-137">Type</span></span>        | <span data-ttu-id="dad08-138">说明</span><span class="sxs-lookup"><span data-stu-id="dad08-138">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="dad08-139">此控件将要成为的程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="dad08-139">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="dad08-140">控件的 controlId，特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="dad08-140">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="dad08-141">ProgramControlType 标识程序控制的类型-例如，链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="dad08-141">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="dad08-142">响应</span><span class="sxs-lookup"><span data-stu-id="dad08-142">Response</span></span>
<span data-ttu-id="dad08-143">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dad08-143">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="dad08-144">示例</span><span class="sxs-lookup"><span data-stu-id="dad08-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dad08-145">请求</span><span class="sxs-lookup"><span data-stu-id="dad08-145">Request</span></span>
<span data-ttu-id="dad08-146">在请求正文中，提供 [programControl](../resources/programcontrol.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dad08-146">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="dad08-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dad08-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dad08-148">C#</span><span class="sxs-lookup"><span data-stu-id="dad08-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dad08-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dad08-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dad08-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dad08-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dad08-151">响应</span><span class="sxs-lookup"><span data-stu-id="dad08-151">Response</span></span>
><span data-ttu-id="dad08-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dad08-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dad08-154">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dad08-154">See also</span></span>

| <span data-ttu-id="dad08-155">方法</span><span class="sxs-lookup"><span data-stu-id="dad08-155">Method</span></span>           | <span data-ttu-id="dad08-156">返回类型</span><span class="sxs-lookup"><span data-stu-id="dad08-156">Return Type</span></span>    |<span data-ttu-id="dad08-157">说明</span><span class="sxs-lookup"><span data-stu-id="dad08-157">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dad08-158">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="dad08-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="dad08-159">[programControlType](../resources/programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dad08-159">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="dad08-160">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="dad08-160">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


