---
title: 创建 itemEmail
description: 创建新的 itemEmail。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c273e7c826d8222596521948c91f48d939657575
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455107"
---
# <a name="create-itememail"></a><span data-ttu-id="35ba6-103">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="35ba6-103">Create itemEmail</span></span>

<span data-ttu-id="35ba6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="35ba6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35ba6-105">创建新的[itemEmail](../resources/itememail.md)。</span><span class="sxs-lookup"><span data-stu-id="35ba6-105">Create a new [itemEmail](../resources/itememail.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35ba6-106">权限</span><span class="sxs-lookup"><span data-stu-id="35ba6-106">Permissions</span></span>

<span data-ttu-id="35ba6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35ba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35ba6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="35ba6-109">Permission type</span></span>                        | <span data-ttu-id="35ba6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35ba6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35ba6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35ba6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35ba6-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="35ba6-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="35ba6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35ba6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35ba6-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="35ba6-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="35ba6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="35ba6-115">Application</span></span>                            | <span data-ttu-id="35ba6-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ba6-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35ba6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35ba6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="35ba6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="35ba6-118">Request headers</span></span>

| <span data-ttu-id="35ba6-119">名称</span><span class="sxs-lookup"><span data-stu-id="35ba6-119">Name</span></span>      |<span data-ttu-id="35ba6-120">说明</span><span class="sxs-lookup"><span data-stu-id="35ba6-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35ba6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35ba6-121">Authorization</span></span>  | <span data-ttu-id="35ba6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35ba6-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="35ba6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35ba6-124">Content-Type</span></span>   | <span data-ttu-id="35ba6-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="35ba6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35ba6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35ba6-127">Request body</span></span>

<span data-ttu-id="35ba6-128">在请求正文中，提供[itemEmail](../resources/itememail.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35ba6-128">In the request body, supply a JSON representation of an [itemEmail](../resources/itememail.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="35ba6-129">响应</span><span class="sxs-lookup"><span data-stu-id="35ba6-129">Response</span></span>

<span data-ttu-id="35ba6-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35ba6-130">If successful, this method returns a `201 Created` response code and a new [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35ba6-131">示例</span><span class="sxs-lookup"><span data-stu-id="35ba6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35ba6-132">请求</span><span class="sxs-lookup"><span data-stu-id="35ba6-132">Request</span></span>

<span data-ttu-id="35ba6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="35ba6-133">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35ba6-134">响应</span><span class="sxs-lookup"><span data-stu-id="35ba6-134">Response</span></span>

<span data-ttu-id="35ba6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="35ba6-135">The following is an example of the response.</span></span>

> <span data-ttu-id="35ba6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35ba6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
