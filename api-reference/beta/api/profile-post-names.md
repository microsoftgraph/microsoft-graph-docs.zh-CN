---
title: 创建 Contact.personname
description: 使用此 API 在用户的配置文件中创建新的 Contact.personname。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a2523d72909946eed95b455e50b3e1fb1a1c51f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937684"
---
# <a name="create-personname"></a><span data-ttu-id="ba621-103">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="ba621-103">Create personName</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba621-104">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba621-104">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba621-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba621-105">Permissions</span></span>

<span data-ttu-id="ba621-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba621-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba621-108">Permission type</span></span>                        | <span data-ttu-id="ba621-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba621-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ba621-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba621-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba621-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="ba621-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba621-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba621-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba621-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="ba621-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba621-114">Application</span><span class="sxs-lookup"><span data-stu-id="ba621-114">Application</span></span>                            | <span data-ttu-id="ba621-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="ba621-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba621-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba621-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="ba621-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba621-117">Request headers</span></span>

| <span data-ttu-id="ba621-118">名称</span><span class="sxs-lookup"><span data-stu-id="ba621-118">Name</span></span>           |<span data-ttu-id="ba621-119">说明</span><span class="sxs-lookup"><span data-stu-id="ba621-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ba621-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba621-120">Authorization</span></span>  | <span data-ttu-id="ba621-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba621-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ba621-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba621-123">Content-Type</span></span>   | <span data-ttu-id="ba621-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ba621-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba621-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba621-126">Request body</span></span>

<span data-ttu-id="ba621-127">在请求正文中，提供[contact.personname](../resources/personname.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba621-127">In the request body, supply a JSON representation of [personName](../resources/personname.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ba621-128">响应</span><span class="sxs-lookup"><span data-stu-id="ba621-128">Response</span></span>

<span data-ttu-id="ba621-129">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba621-129">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba621-130">示例</span><span class="sxs-lookup"><span data-stu-id="ba621-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba621-131">请求</span><span class="sxs-lookup"><span data-stu-id="ba621-131">Request</span></span>

<span data-ttu-id="ba621-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba621-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

### <a name="response"></a><span data-ttu-id="ba621-133">响应</span><span class="sxs-lookup"><span data-stu-id="ba621-133">Response</span></span>

<span data-ttu-id="ba621-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba621-134">The following is an example of the response.</span></span>

> <span data-ttu-id="ba621-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba621-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->