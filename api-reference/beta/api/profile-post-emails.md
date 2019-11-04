---
title: 创建 itemEmail
description: 创建新的 itemEmail。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 25f81760c4d4320474027d0f3d7f5113007ae94d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937705"
---
# <a name="create-itememail"></a><span data-ttu-id="2f921-103">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="2f921-103">Create itemEmail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f921-104">创建新的[itemEmail](../resources/itememail.md)。</span><span class="sxs-lookup"><span data-stu-id="2f921-104">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f921-105">权限</span><span class="sxs-lookup"><span data-stu-id="2f921-105">Permissions</span></span>

<span data-ttu-id="2f921-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f921-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f921-108">Permission type</span></span>                        | <span data-ttu-id="2f921-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f921-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f921-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f921-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f921-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2f921-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2f921-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f921-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f921-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2f921-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2f921-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f921-114">Application</span></span>                            | <span data-ttu-id="2f921-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f921-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f921-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f921-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="2f921-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f921-117">Request headers</span></span>

| <span data-ttu-id="2f921-118">名称</span><span class="sxs-lookup"><span data-stu-id="2f921-118">Name</span></span>      |<span data-ttu-id="2f921-119">说明</span><span class="sxs-lookup"><span data-stu-id="2f921-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f921-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f921-120">Authorization</span></span>  | <span data-ttu-id="2f921-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f921-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2f921-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f921-123">Content-Type</span></span>   | <span data-ttu-id="2f921-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2f921-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f921-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f921-126">Request body</span></span>

<span data-ttu-id="2f921-127">在请求正文中，提供[itemEmail](../resources/itememail.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f921-127">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f921-128">响应</span><span class="sxs-lookup"><span data-stu-id="2f921-128">Response</span></span>

<span data-ttu-id="2f921-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f921-129">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f921-130">示例</span><span class="sxs-lookup"><span data-stu-id="2f921-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f921-131">请求</span><span class="sxs-lookup"><span data-stu-id="2f921-131">Request</span></span>

<span data-ttu-id="2f921-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f921-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/user/profile/emails
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

### <a name="response"></a><span data-ttu-id="2f921-133">响应</span><span class="sxs-lookup"><span data-stu-id="2f921-133">Response</span></span>

<span data-ttu-id="2f921-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f921-134">The following is an example of the response.</span></span>

> <span data-ttu-id="2f921-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2f921-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
