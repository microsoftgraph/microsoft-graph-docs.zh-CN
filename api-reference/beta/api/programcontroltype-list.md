---
title: 列出 programControlTypes
description: 在 "Azure AD access 评论" 功能中, 列出所有 programControlType 对象。
localization_priority: Normal
ms.openlocfilehash: 2a2767a0dc55e5d2d046e897ec0ac6cde10af945
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264076"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="a3826-103">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="a3826-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3826-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 列出所有[programControlType](../resources/programcontroltype.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a3826-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3826-105">权限</span><span class="sxs-lookup"><span data-stu-id="a3826-105">Permissions</span></span>
<span data-ttu-id="a3826-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3826-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3826-108">Permission type</span></span>                        | <span data-ttu-id="a3826-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3826-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3826-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3826-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3826-111">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="a3826-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="a3826-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3826-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3826-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3826-113">Not supported.</span></span> |
|<span data-ttu-id="a3826-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3826-114">Application</span></span>                            | <span data-ttu-id="a3826-115">ProgramControl "、ProgramControl 的所有</span><span class="sxs-lookup"><span data-stu-id="a3826-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="a3826-116">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="a3826-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3826-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3826-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="a3826-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3826-118">Request headers</span></span>
| <span data-ttu-id="a3826-119">名称</span><span class="sxs-lookup"><span data-stu-id="a3826-119">Name</span></span>         | <span data-ttu-id="a3826-120">类型</span><span class="sxs-lookup"><span data-stu-id="a3826-120">Type</span></span>        | <span data-ttu-id="a3826-121">说明</span><span class="sxs-lookup"><span data-stu-id="a3826-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a3826-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3826-122">Authorization</span></span> | <span data-ttu-id="a3826-123">string</span><span class="sxs-lookup"><span data-stu-id="a3826-123">string</span></span> | <span data-ttu-id="a3826-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3826-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3826-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3826-126">Request body</span></span>
<span data-ttu-id="a3826-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3826-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a3826-128">响应</span><span class="sxs-lookup"><span data-stu-id="a3826-128">Response</span></span>
<span data-ttu-id="a3826-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[programControlType](../resources/programcontroltype.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="a3826-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3826-130">示例</span><span class="sxs-lookup"><span data-stu-id="a3826-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3826-131">请求</span><span class="sxs-lookup"><span data-stu-id="a3826-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="a3826-132">响应</span><span class="sxs-lookup"><span data-stu-id="a3826-132">Response</span></span>
><span data-ttu-id="a3826-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3826-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3826-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a3826-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3826-136">C#</span><span class="sxs-lookup"><span data-stu-id="a3826-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3826-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3826-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a3826-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="a3826-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="a3826-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a3826-139">See also</span></span>

| <span data-ttu-id="a3826-140">方法</span><span class="sxs-lookup"><span data-stu-id="a3826-140">Method</span></span>           | <span data-ttu-id="a3826-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3826-141">Return Type</span></span>    |<span data-ttu-id="a3826-142">说明</span><span class="sxs-lookup"><span data-stu-id="a3826-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3826-143">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="a3826-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="a3826-144">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3826-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="a3826-145">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="a3826-145">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
