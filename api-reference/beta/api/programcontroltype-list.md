---
title: 列出 programControlTypes
description: 在 "Azure AD access 评论" 功能中，列出所有 programControlType 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 93cf528b1fec7f857057ea469ae5c313dee6c07c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896425"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="9e8bf-103">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="9e8bf-103">List programControlTypes</span></span>

<span data-ttu-id="9e8bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e8bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e8bf-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，列出所有[programControlType](../resources/programcontroltype.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e8bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="9e8bf-106">Permissions</span></span>
<span data-ttu-id="9e8bf-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9e8bf-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9e8bf-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e8bf-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e8bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e8bf-109">Permission type</span></span>                        | <span data-ttu-id="9e8bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e8bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e8bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e8bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e8bf-112">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="9e8bf-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="9e8bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e8bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e8bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-114">Not supported.</span></span> |
|<span data-ttu-id="9e8bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e8bf-115">Application</span></span>                            | <span data-ttu-id="9e8bf-116">ProgramControl "、ProgramControl 的所有</span><span class="sxs-lookup"><span data-stu-id="9e8bf-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="9e8bf-117">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="9e8bf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e8bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="9e8bf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e8bf-119">Request headers</span></span>
| <span data-ttu-id="9e8bf-120">名称</span><span class="sxs-lookup"><span data-stu-id="9e8bf-120">Name</span></span>         | <span data-ttu-id="9e8bf-121">类型</span><span class="sxs-lookup"><span data-stu-id="9e8bf-121">Type</span></span>        | <span data-ttu-id="9e8bf-122">说明</span><span class="sxs-lookup"><span data-stu-id="9e8bf-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9e8bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e8bf-123">Authorization</span></span> | <span data-ttu-id="9e8bf-124">string</span><span class="sxs-lookup"><span data-stu-id="9e8bf-124">string</span></span> | <span data-ttu-id="9e8bf-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="9e8bf-125">Bearer \{token\}.</span></span> <span data-ttu-id="9e8bf-126">Required.</span><span class="sxs-lookup"><span data-stu-id="9e8bf-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e8bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e8bf-127">Request body</span></span>
<span data-ttu-id="9e8bf-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="9e8bf-129">响应</span><span class="sxs-lookup"><span data-stu-id="9e8bf-129">Response</span></span>
<span data-ttu-id="9e8bf-130">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和[programControlType](../resources/programcontroltype.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e8bf-131">示例</span><span class="sxs-lookup"><span data-stu-id="9e8bf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e8bf-132">请求</span><span class="sxs-lookup"><span data-stu-id="9e8bf-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9e8bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e8bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="9e8bf-134">C#</span><span class="sxs-lookup"><span data-stu-id="9e8bf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e8bf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e8bf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e8bf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e8bf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e8bf-137">响应</span><span class="sxs-lookup"><span data-stu-id="9e8bf-137">Response</span></span>
><span data-ttu-id="9e8bf-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="9e8bf-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9e8bf-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9e8bf-139">All the properties will be returned from an actual call.</span></span>
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
            "displayName": "Access Reviews for Microsoft 365 groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="9e8bf-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9e8bf-140">See also</span></span>

| <span data-ttu-id="9e8bf-141">方法</span><span class="sxs-lookup"><span data-stu-id="9e8bf-141">Method</span></span>           | <span data-ttu-id="9e8bf-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e8bf-142">Return Type</span></span>    |<span data-ttu-id="9e8bf-143">说明</span><span class="sxs-lookup"><span data-stu-id="9e8bf-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e8bf-144">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="9e8bf-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="9e8bf-145">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e8bf-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="9e8bf-146">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="9e8bf-146">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
