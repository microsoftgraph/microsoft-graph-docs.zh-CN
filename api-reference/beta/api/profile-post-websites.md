---
title: 创建 personWebsite
description: 创建新的 personWebsite。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5fb4d4a427229c0bf727596b46520cf767cbd29f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937642"
---
# <a name="create-personwebsite"></a><span data-ttu-id="91708-103">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="91708-103">Create personWebsite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91708-104">在用户的[配置文件](../resources/profile.md)中创建新的[personWebsite](../resources/personwebsite.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91708-104">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91708-105">权限</span><span class="sxs-lookup"><span data-stu-id="91708-105">Permissions</span></span>

<span data-ttu-id="91708-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91708-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="91708-108">Permission type</span></span>                        | <span data-ttu-id="91708-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91708-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91708-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91708-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91708-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="91708-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="91708-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91708-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91708-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="91708-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="91708-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="91708-114">Application</span></span>                            | <span data-ttu-id="91708-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91708-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91708-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91708-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="91708-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="91708-117">Request headers</span></span>

| <span data-ttu-id="91708-118">名称</span><span class="sxs-lookup"><span data-stu-id="91708-118">Name</span></span>      |<span data-ttu-id="91708-119">说明</span><span class="sxs-lookup"><span data-stu-id="91708-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91708-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91708-120">Authorization</span></span>  | <span data-ttu-id="91708-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91708-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="91708-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91708-123">Content-Type</span></span>   | <span data-ttu-id="91708-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="91708-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91708-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91708-126">Request body</span></span>

<span data-ttu-id="91708-127">在请求正文中，提供[personWebsite](../resources/personwebsite.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91708-127">In the request body, supply a JSON representation of [personWebsite](../resources/personwebsite.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="91708-128">响应</span><span class="sxs-lookup"><span data-stu-id="91708-128">Response</span></span>

<span data-ttu-id="91708-129">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[personWebsite](../resources/personwebsite.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91708-129">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91708-130">示例</span><span class="sxs-lookup"><span data-stu-id="91708-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91708-131">请求</span><span class="sxs-lookup"><span data-stu-id="91708-131">Request</span></span>

<span data-ttu-id="91708-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91708-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="91708-133">响应</span><span class="sxs-lookup"><span data-stu-id="91708-133">Response</span></span>

<span data-ttu-id="91708-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91708-134">The following is an example of the response.</span></span>

> <span data-ttu-id="91708-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91708-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
