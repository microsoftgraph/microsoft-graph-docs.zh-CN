---
title: 删除 programControl
description: 在 Azure AD 中访问审阅功能，删除 programControl 对象。  这将取消链接从某个程序访问审阅。
localization_priority: Normal
ms.openlocfilehash: 782cc8f336e84f82d937e3180d7de6af69e67e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843916"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="e8d42-104">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="e8d42-104">Delete programControl</span></span>

> <span data-ttu-id="e8d42-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8d42-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8d42-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8d42-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8d42-107">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，删除[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8d42-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="e8d42-108">这将取消链接从某个程序访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e8d42-108">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8d42-109">权限</span><span class="sxs-lookup"><span data-stu-id="e8d42-109">Permissions</span></span>
<span data-ttu-id="e8d42-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8d42-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d42-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8d42-112">Permission type</span></span>                        | <span data-ttu-id="e8d42-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8d42-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d42-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8d42-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8d42-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e8d42-115"></span></span>  <span data-ttu-id="e8d42-116">登录的用户必须同时是允许他们删除 programControl 目录角色中。</span><span class="sxs-lookup"><span data-stu-id="e8d42-116">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="e8d42-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8d42-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d42-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8d42-118">Not supported.</span></span> |
|<span data-ttu-id="e8d42-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8d42-119">Application</span></span>                            | <span data-ttu-id="e8d42-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8d42-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d42-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8d42-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="e8d42-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8d42-122">Request headers</span></span>
| <span data-ttu-id="e8d42-123">名称</span><span class="sxs-lookup"><span data-stu-id="e8d42-123">Name</span></span>         | <span data-ttu-id="e8d42-124">类型</span><span class="sxs-lookup"><span data-stu-id="e8d42-124">Type</span></span>        | <span data-ttu-id="e8d42-125">说明</span><span class="sxs-lookup"><span data-stu-id="e8d42-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e8d42-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8d42-126">Authorization</span></span> | <span data-ttu-id="e8d42-127">string</span><span class="sxs-lookup"><span data-stu-id="e8d42-127">string</span></span> | <span data-ttu-id="e8d42-128">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="e8d42-128">Bearer \{token\}.</span></span> <span data-ttu-id="e8d42-129">必填。</span><span class="sxs-lookup"><span data-stu-id="e8d42-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8d42-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8d42-130">Request body</span></span>
<span data-ttu-id="e8d42-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8d42-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e8d42-132">响应</span><span class="sxs-lookup"><span data-stu-id="e8d42-132">Response</span></span>
<span data-ttu-id="e8d42-p107">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e8d42-p107">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8d42-135">示例</span><span class="sxs-lookup"><span data-stu-id="e8d42-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8d42-136">请求</span><span class="sxs-lookup"><span data-stu-id="e8d42-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="e8d42-137">响应</span><span class="sxs-lookup"><span data-stu-id="e8d42-137">Response</span></span>
><span data-ttu-id="e8d42-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e8d42-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
