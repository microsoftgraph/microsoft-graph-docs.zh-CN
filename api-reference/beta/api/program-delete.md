---
title: 删除程序
description: 在 "Azure AD access 评论" 功能中, 删除一个程序对象。
localization_priority: Normal
ms.openlocfilehash: 930367e6c61d354655e73fb7ece9c8776e15f34e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546396"
---
# <a name="delete-program"></a><span data-ttu-id="9cc12-103">删除程序</span><span class="sxs-lookup"><span data-stu-id="9cc12-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc12-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 删除一个[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9cc12-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="9cc12-105">请勿删除仍与它`programControl`链接的程序, 应首先从该程序中删除或取消这些访问审核, 并将其链接到其他程序。</span><span class="sxs-lookup"><span data-stu-id="9cc12-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="9cc12-106">此外, 请注意, 不能删除内置的默认程序。</span><span class="sxs-lookup"><span data-stu-id="9cc12-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="9cc12-107">权限</span><span class="sxs-lookup"><span data-stu-id="9cc12-107">Permissions</span></span>
<span data-ttu-id="9cc12-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cc12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc12-110">Permission type</span></span>                        | <span data-ttu-id="9cc12-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc12-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc12-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="9cc12-113"></span></span>  <span data-ttu-id="9cc12-114">登录用户还必须位于允许他们创建程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="9cc12-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="9cc12-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc12-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc12-116">Not supported.</span></span> |
|<span data-ttu-id="9cc12-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc12-117">Application</span></span>                            | <span data-ttu-id="9cc12-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc12-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc12-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc12-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="9cc12-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc12-120">Request headers</span></span>
| <span data-ttu-id="9cc12-121">名称</span><span class="sxs-lookup"><span data-stu-id="9cc12-121">Name</span></span>         | <span data-ttu-id="9cc12-122">类型</span><span class="sxs-lookup"><span data-stu-id="9cc12-122">Type</span></span>        | <span data-ttu-id="9cc12-123">说明</span><span class="sxs-lookup"><span data-stu-id="9cc12-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9cc12-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc12-124">Authorization</span></span> | <span data-ttu-id="9cc12-125">string</span><span class="sxs-lookup"><span data-stu-id="9cc12-125">string</span></span> | <span data-ttu-id="9cc12-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc12-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc12-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc12-128">Request body</span></span>
<span data-ttu-id="9cc12-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cc12-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9cc12-130">响应</span><span class="sxs-lookup"><span data-stu-id="9cc12-130">Response</span></span>
<span data-ttu-id="9cc12-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9cc12-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc12-133">示例</span><span class="sxs-lookup"><span data-stu-id="9cc12-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cc12-134">请求</span><span class="sxs-lookup"><span data-stu-id="9cc12-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="9cc12-135">响应</span><span class="sxs-lookup"><span data-stu-id="9cc12-135">Response</span></span>
><span data-ttu-id="9cc12-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc12-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
