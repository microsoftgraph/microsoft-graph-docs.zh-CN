---
title: 通道： completeMigration
description: 通过从通道中删除迁移模式来完成外部邮件的迁移。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 632aa4b1bdcf949951598f083fec1376ce9417cc
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903966"
---
# <a name="channel-completemigration"></a><span data-ttu-id="776ce-103">通道： completeMigration</span><span class="sxs-lookup"><span data-stu-id="776ce-103">channel: completeMigration</span></span>

<span data-ttu-id="776ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="776ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="776ce-105">通过 `migration mode` 从团队中的 [通道](../resources/channel.md) 中删除来完成邮件迁移过程。</span><span class="sxs-lookup"><span data-stu-id="776ce-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="776ce-106">`Migration mode` 是一种特殊状态，可防止在数据迁移过程中执行某些操作（如发送邮件和添加成员）。</span><span class="sxs-lookup"><span data-stu-id="776ce-106">`Migration mode` is a special state that prevents certain operations, like sending messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="776ce-107">发出 **completeMigration** 请求后，不能将其他邮件导入到团队中。</span><span class="sxs-lookup"><span data-stu-id="776ce-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="776ce-108">在请求返回成功的响应之后，您可以向团队添加成员。</span><span class="sxs-lookup"><span data-stu-id="776ce-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="776ce-109">权限</span><span class="sxs-lookup"><span data-stu-id="776ce-109">Permissions</span></span>

<span data-ttu-id="776ce-110">若要调用此 API，需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="776ce-110">The following permission is required to call this API.</span></span> <span data-ttu-id="776ce-111">若要了解详细信息， *请参阅*[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="776ce-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="776ce-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="776ce-112">Permission type</span></span>      | <span data-ttu-id="776ce-113">权限</span><span class="sxs-lookup"><span data-stu-id="776ce-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="776ce-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="776ce-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="776ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="776ce-115">Not supported.</span></span>|
| <span data-ttu-id="776ce-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="776ce-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="776ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="776ce-117">Not supported.</span></span> |
|<span data-ttu-id="776ce-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="776ce-118">Application</span></span> | <span data-ttu-id="776ce-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="776ce-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="776ce-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="776ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="776ce-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="776ce-121">Request headers</span></span>

| <span data-ttu-id="776ce-122">标头</span><span class="sxs-lookup"><span data-stu-id="776ce-122">Header</span></span>       | <span data-ttu-id="776ce-123">值</span><span class="sxs-lookup"><span data-stu-id="776ce-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="776ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="776ce-124">Authorization</span></span>  | <span data-ttu-id="776ce-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="776ce-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="776ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="776ce-127">Request body</span></span>

<span data-ttu-id="776ce-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="776ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="776ce-129">响应</span><span class="sxs-lookup"><span data-stu-id="776ce-129">Response</span></span>

<span data-ttu-id="776ce-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="776ce-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="776ce-132">示例</span><span class="sxs-lookup"><span data-stu-id="776ce-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="776ce-133">请求</span><span class="sxs-lookup"><span data-stu-id="776ce-133">Request</span></span>

<span data-ttu-id="776ce-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="776ce-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


# <a name="http"></a>[<span data-ttu-id="776ce-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="776ce-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="776ce-136">C#</span><span class="sxs-lookup"><span data-stu-id="776ce-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="776ce-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="776ce-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="776ce-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="776ce-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="776ce-139">响应</span><span class="sxs-lookup"><span data-stu-id="776ce-139">Response</span></span>

<span data-ttu-id="776ce-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="776ce-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
