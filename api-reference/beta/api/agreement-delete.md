---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
ms.openlocfilehash: 2ebd62f9b367e48928c05b85e3a25c6d4b9bf285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809294"
---
# <a name="delete-agreement"></a><span data-ttu-id="b4821-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="b4821-103">Delete agreement</span></span>

> <span data-ttu-id="b4821-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b4821-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4821-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b4821-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4821-106">删除[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4821-106">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4821-107">权限</span><span class="sxs-lookup"><span data-stu-id="b4821-107">Permissions</span></span>
<span data-ttu-id="b4821-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4821-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4821-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4821-110">Permission type</span></span>                        | <span data-ttu-id="b4821-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4821-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4821-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4821-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4821-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4821-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="b4821-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4821-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4821-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4821-115">Not supported.</span></span> |
|<span data-ttu-id="b4821-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4821-116">Application</span></span>                            | <span data-ttu-id="b4821-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4821-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4821-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4821-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="b4821-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4821-119">Request headers</span></span>
| <span data-ttu-id="b4821-120">名称</span><span class="sxs-lookup"><span data-stu-id="b4821-120">Name</span></span>         | <span data-ttu-id="b4821-121">类型</span><span class="sxs-lookup"><span data-stu-id="b4821-121">Type</span></span>        | <span data-ttu-id="b4821-122">说明</span><span class="sxs-lookup"><span data-stu-id="b4821-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b4821-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4821-123">Authorization</span></span> | <span data-ttu-id="b4821-124">string</span><span class="sxs-lookup"><span data-stu-id="b4821-124">string</span></span> | <span data-ttu-id="b4821-125">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="b4821-125">Bearer \{token\}.</span></span> <span data-ttu-id="b4821-126">必填。</span><span class="sxs-lookup"><span data-stu-id="b4821-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4821-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4821-127">Request body</span></span>
<span data-ttu-id="b4821-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4821-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b4821-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4821-129">Response</span></span>
<span data-ttu-id="b4821-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4821-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4821-132">示例</span><span class="sxs-lookup"><span data-stu-id="b4821-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4821-133">请求</span><span class="sxs-lookup"><span data-stu-id="b4821-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="b4821-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4821-134">Response</span></span>
><span data-ttu-id="b4821-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4821-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
