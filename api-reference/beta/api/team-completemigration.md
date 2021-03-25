---
title: team： completeMigration
description: 通过从团队中删除迁移模式完成外部邮件的迁移。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6edd393475eecba7da736fe0c72571ffc244b73e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200757"
---
# <a name="team-completemigration"></a><span data-ttu-id="6066a-103">team： completeMigration</span><span class="sxs-lookup"><span data-stu-id="6066a-103">team: completeMigration</span></span>

<span data-ttu-id="6066a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6066a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6066a-105">通过从团队 中删除 完成 `migration mode` 邮件迁移 [过程](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="6066a-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="6066a-106">`Migration mode` 是禁止某些操作的特殊状态，如数据迁移过程中的邮件 POST 和成员资格操作。</span><span class="sxs-lookup"><span data-stu-id="6066a-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="6066a-107">完成 **Migration 请求后** ，无法将其他消息导入团队。</span><span class="sxs-lookup"><span data-stu-id="6066a-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="6066a-108">在请求返回成功响应后，你可以向团队添加成员。</span><span class="sxs-lookup"><span data-stu-id="6066a-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="6066a-109">权限</span><span class="sxs-lookup"><span data-stu-id="6066a-109">Permissions</span></span>

<span data-ttu-id="6066a-110">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="6066a-110">The following permission is required to call this API.</span></span> <span data-ttu-id="6066a-111">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6066a-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6066a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6066a-112">Permission type</span></span>      | <span data-ttu-id="6066a-113">权限</span><span class="sxs-lookup"><span data-stu-id="6066a-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="6066a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6066a-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="6066a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6066a-115">Not supported.</span></span>|
| <span data-ttu-id="6066a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6066a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6066a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6066a-117">Not supported.</span></span> |
|<span data-ttu-id="6066a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6066a-118">Application</span></span> | <span data-ttu-id="6066a-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="6066a-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6066a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6066a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="6066a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6066a-121">Request headers</span></span>

| <span data-ttu-id="6066a-122">标头</span><span class="sxs-lookup"><span data-stu-id="6066a-122">Header</span></span>       | <span data-ttu-id="6066a-123">值</span><span class="sxs-lookup"><span data-stu-id="6066a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6066a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6066a-124">Authorization</span></span>  | <span data-ttu-id="6066a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6066a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6066a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6066a-127">Request body</span></span>

<span data-ttu-id="6066a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6066a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6066a-129">响应</span><span class="sxs-lookup"><span data-stu-id="6066a-129">Response</span></span>

<span data-ttu-id="6066a-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6066a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6066a-132">示例</span><span class="sxs-lookup"><span data-stu-id="6066a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6066a-133">请求</span><span class="sxs-lookup"><span data-stu-id="6066a-133">Request</span></span>

<span data-ttu-id="6066a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6066a-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration
```


<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="6066a-135">响应</span><span class="sxs-lookup"><span data-stu-id="6066a-135">Response</span></span>

<span data-ttu-id="6066a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6066a-136">The following is an example of the response.</span></span>
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
