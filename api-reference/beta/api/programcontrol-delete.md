---
title: 删除 programControl
description: 在 Azure AD 中访问审阅功能，删除 programControl 对象。  这将取消链接从某个程序访问审阅。
ms.openlocfilehash: a7f21cd4c18ecda2ce15a6dd76d87322f75e4af0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044005"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="646c0-104">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="646c0-104">Delete programControl</span></span>

> <span data-ttu-id="646c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="646c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="646c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="646c0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="646c0-107">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，删除[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="646c0-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="646c0-108">这将取消链接从某个程序访问审阅。</span><span class="sxs-lookup"><span data-stu-id="646c0-108">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="646c0-109">权限</span><span class="sxs-lookup"><span data-stu-id="646c0-109">Permissions</span></span>
<span data-ttu-id="646c0-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="646c0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="646c0-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="646c0-112">Permission type</span></span>                        | <span data-ttu-id="646c0-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="646c0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="646c0-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="646c0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="646c0-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="646c0-115"></span></span>  <span data-ttu-id="646c0-116">登录的用户必须同时是允许他们删除 programControl 目录角色中。</span><span class="sxs-lookup"><span data-stu-id="646c0-116">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="646c0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="646c0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="646c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="646c0-118">Not supported.</span></span> |
|<span data-ttu-id="646c0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="646c0-119">Application</span></span>                            | <span data-ttu-id="646c0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="646c0-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="646c0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="646c0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="646c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="646c0-122">Request headers</span></span>
| <span data-ttu-id="646c0-123">名称</span><span class="sxs-lookup"><span data-stu-id="646c0-123">Name</span></span>         | <span data-ttu-id="646c0-124">类型</span><span class="sxs-lookup"><span data-stu-id="646c0-124">Type</span></span>        | <span data-ttu-id="646c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="646c0-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="646c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="646c0-126">Authorization</span></span> | <span data-ttu-id="646c0-127">string</span><span class="sxs-lookup"><span data-stu-id="646c0-127">string</span></span> | <span data-ttu-id="646c0-128">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="646c0-128">Bearer \{token\}.</span></span> <span data-ttu-id="646c0-129">必需。</span><span class="sxs-lookup"><span data-stu-id="646c0-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="646c0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="646c0-130">Request body</span></span>
<span data-ttu-id="646c0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="646c0-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="646c0-132">响应</span><span class="sxs-lookup"><span data-stu-id="646c0-132">Response</span></span>
<span data-ttu-id="646c0-p107">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="646c0-p107">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="646c0-135">示例</span><span class="sxs-lookup"><span data-stu-id="646c0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="646c0-136">请求</span><span class="sxs-lookup"><span data-stu-id="646c0-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="646c0-137">响应</span><span class="sxs-lookup"><span data-stu-id="646c0-137">Response</span></span>
><span data-ttu-id="646c0-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="646c0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
