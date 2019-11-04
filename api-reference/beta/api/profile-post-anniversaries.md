---
title: 创建 personAnniversary
description: 使用此 API 创建新的 personAnniversary。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e6e73919913f710bee6721ec1710847cc742ba4d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937719"
---
# <a name="create-personanniversary"></a><span data-ttu-id="3048b-103">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="3048b-103">Create personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3048b-104">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3048b-104">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3048b-105">权限</span><span class="sxs-lookup"><span data-stu-id="3048b-105">Permissions</span></span>

<span data-ttu-id="3048b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3048b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3048b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3048b-108">Permission type</span></span>                        | <span data-ttu-id="3048b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3048b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3048b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3048b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3048b-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="3048b-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3048b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3048b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3048b-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="3048b-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3048b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3048b-114">Application</span></span>                            | <span data-ttu-id="3048b-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3048b-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3048b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3048b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries 
```

## <a name="request-headers"></a><span data-ttu-id="3048b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3048b-117">Request headers</span></span>

| <span data-ttu-id="3048b-118">名称</span><span class="sxs-lookup"><span data-stu-id="3048b-118">Name</span></span>      |<span data-ttu-id="3048b-119">说明</span><span class="sxs-lookup"><span data-stu-id="3048b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3048b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3048b-120">Authorization</span></span>  | <span data-ttu-id="3048b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3048b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3048b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3048b-123">Content-Type</span></span>   | <span data-ttu-id="3048b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3048b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3048b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3048b-126">Request body</span></span>

<span data-ttu-id="3048b-127">在请求正文中，提供[personAnniversary](../resources/personanniversary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3048b-127">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3048b-128">响应</span><span class="sxs-lookup"><span data-stu-id="3048b-128">Response</span></span>

<span data-ttu-id="3048b-129">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3048b-129">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3048b-130">示例</span><span class="sxs-lookup"><span data-stu-id="3048b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3048b-131">请求</span><span class="sxs-lookup"><span data-stu-id="3048b-131">Request</span></span>

<span data-ttu-id="3048b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3048b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="3048b-133">响应</span><span class="sxs-lookup"><span data-stu-id="3048b-133">Response</span></span>

<span data-ttu-id="3048b-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3048b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="3048b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3048b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->