---
title: 团队： completeMigration
description: 通过从团队中删除迁移模式来完成外部邮件的迁移。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0594d7da3dce01285829e9ad4e59e8143c41bfdf
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903577"
---
# <a name="team-completemigration"></a><span data-ttu-id="f99c6-103">团队： completeMigration</span><span class="sxs-lookup"><span data-stu-id="f99c6-103">team: completeMigration</span></span>

<span data-ttu-id="f99c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f99c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f99c6-105">通过 `migration mode` 从 [团队](../resources/team.md)中删除来完成邮件迁移过程。</span><span class="sxs-lookup"><span data-stu-id="f99c6-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="f99c6-106">`Migration mode` 是一种特殊状态，在数据迁移过程中，某些操作是不带条的，如邮件投递和成员资格操作。</span><span class="sxs-lookup"><span data-stu-id="f99c6-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="f99c6-107">发出 **completeMigration** 请求后，不能将其他邮件导入到团队中。</span><span class="sxs-lookup"><span data-stu-id="f99c6-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="f99c6-108">在请求返回成功的响应之后，您可以向团队添加成员。</span><span class="sxs-lookup"><span data-stu-id="f99c6-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="f99c6-109">权限</span><span class="sxs-lookup"><span data-stu-id="f99c6-109">Permissions</span></span>

<span data-ttu-id="f99c6-110">若要调用此 API，需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="f99c6-110">The following permission is required to call this API.</span></span> <span data-ttu-id="f99c6-111">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f99c6-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99c6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f99c6-112">Permission type</span></span>      | <span data-ttu-id="f99c6-113">权限</span><span class="sxs-lookup"><span data-stu-id="f99c6-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="f99c6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f99c6-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="f99c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f99c6-115">Not supported.</span></span>|
| <span data-ttu-id="f99c6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f99c6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f99c6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f99c6-117">Not supported.</span></span> |
|<span data-ttu-id="f99c6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f99c6-118">Application</span></span> | <span data-ttu-id="f99c6-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="f99c6-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99c6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f99c6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="f99c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f99c6-121">Request headers</span></span>

| <span data-ttu-id="f99c6-122">标头</span><span class="sxs-lookup"><span data-stu-id="f99c6-122">Header</span></span>       | <span data-ttu-id="f99c6-123">值</span><span class="sxs-lookup"><span data-stu-id="f99c6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f99c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f99c6-124">Authorization</span></span>  | <span data-ttu-id="f99c6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f99c6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f99c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f99c6-127">Request body</span></span>

<span data-ttu-id="f99c6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f99c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f99c6-129">响应</span><span class="sxs-lookup"><span data-stu-id="f99c6-129">Response</span></span>

<span data-ttu-id="f99c6-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f99c6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99c6-132">示例</span><span class="sxs-lookup"><span data-stu-id="f99c6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f99c6-133">请求</span><span class="sxs-lookup"><span data-stu-id="f99c6-133">Request</span></span>

<span data-ttu-id="f99c6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f99c6-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


# <a name="http"></a>[<span data-ttu-id="f99c6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f99c6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="f99c6-136">C#</span><span class="sxs-lookup"><span data-stu-id="f99c6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f99c6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f99c6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f99c6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f99c6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f99c6-139">响应</span><span class="sxs-lookup"><span data-stu-id="f99c6-139">Response</span></span>

<span data-ttu-id="f99c6-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f99c6-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: d945a9a4-0e5b-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
