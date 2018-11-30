---
title: 删除程序
description: 在 Azure AD 中访问审阅功能，删除程序对象。
ms.openlocfilehash: c09dcc36bfc4fbf279e7b6c49ea24bba9153c071
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047018"
---
# <a name="delete-program"></a><span data-ttu-id="3995a-103">删除程序</span><span class="sxs-lookup"><span data-stu-id="3995a-103">Delete program</span></span>

> <span data-ttu-id="3995a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3995a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3995a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3995a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3995a-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，删除[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3995a-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="3995a-107">请不要删除一个程序这仍有`programControl`链接到其，这些访问评论应该首先删除或取消链接从程序并链接到其他程序。</span><span class="sxs-lookup"><span data-stu-id="3995a-107">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="3995a-108">此外，请注意，不能删除内置的默认计划。</span><span class="sxs-lookup"><span data-stu-id="3995a-108">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="3995a-109">权限</span><span class="sxs-lookup"><span data-stu-id="3995a-109">Permissions</span></span>
<span data-ttu-id="3995a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3995a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3995a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3995a-112">Permission type</span></span>                        | <span data-ttu-id="3995a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3995a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3995a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3995a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3995a-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="3995a-115"></span></span>  <span data-ttu-id="3995a-116">登录的用户还必须在目录角色中允许他们创建的程序。</span><span class="sxs-lookup"><span data-stu-id="3995a-116">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="3995a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3995a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3995a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3995a-118">Not supported.</span></span> |
|<span data-ttu-id="3995a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3995a-119">Application</span></span>                            | <span data-ttu-id="3995a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="3995a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3995a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3995a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="3995a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3995a-122">Request headers</span></span>
| <span data-ttu-id="3995a-123">名称</span><span class="sxs-lookup"><span data-stu-id="3995a-123">Name</span></span>         | <span data-ttu-id="3995a-124">类型</span><span class="sxs-lookup"><span data-stu-id="3995a-124">Type</span></span>        | <span data-ttu-id="3995a-125">说明</span><span class="sxs-lookup"><span data-stu-id="3995a-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3995a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3995a-126">Authorization</span></span> | <span data-ttu-id="3995a-127">string</span><span class="sxs-lookup"><span data-stu-id="3995a-127">string</span></span> | <span data-ttu-id="3995a-128">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="3995a-128">Bearer \{token\}.</span></span> <span data-ttu-id="3995a-129">必需。</span><span class="sxs-lookup"><span data-stu-id="3995a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3995a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3995a-130">Request body</span></span>
<span data-ttu-id="3995a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3995a-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3995a-132">响应</span><span class="sxs-lookup"><span data-stu-id="3995a-132">Response</span></span>
<span data-ttu-id="3995a-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3995a-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3995a-135">示例</span><span class="sxs-lookup"><span data-stu-id="3995a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3995a-136">请求</span><span class="sxs-lookup"><span data-stu-id="3995a-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="3995a-137">响应</span><span class="sxs-lookup"><span data-stu-id="3995a-137">Response</span></span>
><span data-ttu-id="3995a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3995a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
