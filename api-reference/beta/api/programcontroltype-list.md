---
title: 列出 programControlTypes
description: 在 "Azure AD access 评论" 功能中, 列出所有 programControlType 对象。
localization_priority: Normal
ms.openlocfilehash: fd9317b5a40c9587b91f0fdd4a9e1a9cfd8f2933
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610633"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="bfc41-103">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="bfc41-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfc41-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[programControlType](../resources/programcontroltype.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfc41-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfc41-105">权限</span><span class="sxs-lookup"><span data-stu-id="bfc41-105">Permissions</span></span>
<span data-ttu-id="bfc41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfc41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfc41-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfc41-108">Permission type</span></span>                        | <span data-ttu-id="bfc41-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfc41-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc41-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc41-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfc41-111">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="bfc41-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="bfc41-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc41-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfc41-113">Not supported.</span></span> |
|<span data-ttu-id="bfc41-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfc41-114">Application</span></span>                            | <span data-ttu-id="bfc41-115">ProgramControl "、ProgramControl 的所有</span><span class="sxs-lookup"><span data-stu-id="bfc41-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="bfc41-116">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="bfc41-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="bfc41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfc41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="bfc41-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfc41-118">Request headers</span></span>
| <span data-ttu-id="bfc41-119">名称</span><span class="sxs-lookup"><span data-stu-id="bfc41-119">Name</span></span>         | <span data-ttu-id="bfc41-120">类型</span><span class="sxs-lookup"><span data-stu-id="bfc41-120">Type</span></span>        | <span data-ttu-id="bfc41-121">说明</span><span class="sxs-lookup"><span data-stu-id="bfc41-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bfc41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc41-122">Authorization</span></span> | <span data-ttu-id="bfc41-123">string</span><span class="sxs-lookup"><span data-stu-id="bfc41-123">string</span></span> | <span data-ttu-id="bfc41-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfc41-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfc41-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfc41-126">Request body</span></span>
<span data-ttu-id="bfc41-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfc41-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bfc41-128">响应</span><span class="sxs-lookup"><span data-stu-id="bfc41-128">Response</span></span>
<span data-ttu-id="bfc41-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[programControlType](../resources/programcontroltype.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="bfc41-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfc41-130">示例</span><span class="sxs-lookup"><span data-stu-id="bfc41-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfc41-131">请求</span><span class="sxs-lookup"><span data-stu-id="bfc41-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="bfc41-132">响应</span><span class="sxs-lookup"><span data-stu-id="bfc41-132">Response</span></span>
><span data-ttu-id="bfc41-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bfc41-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bfc41-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bfc41-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bfc41-136">语言</span><span class="sxs-lookup"><span data-stu-id="bfc41-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfc41-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfc41-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="bfc41-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bfc41-138">See also</span></span>

| <span data-ttu-id="bfc41-139">方法</span><span class="sxs-lookup"><span data-stu-id="bfc41-139">Method</span></span>           | <span data-ttu-id="bfc41-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="bfc41-140">Return Type</span></span>    |<span data-ttu-id="bfc41-141">说明</span><span class="sxs-lookup"><span data-stu-id="bfc41-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfc41-142">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="bfc41-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="bfc41-143">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="bfc41-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="bfc41-144">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="bfc41-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
