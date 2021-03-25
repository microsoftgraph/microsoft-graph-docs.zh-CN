---
title: channel： completeMigration
description: 通过从频道中删除迁移模式完成外部邮件的迁移。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 144ec67ef6e21e11716bec0e61f53c5e079d96cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200964"
---
# <a name="channel-completemigration"></a><span data-ttu-id="71769-103">channel： completeMigration</span><span class="sxs-lookup"><span data-stu-id="71769-103">channel: completeMigration</span></span>

<span data-ttu-id="71769-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71769-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71769-105">通过从团队中的频道删除来完成 `migration mode` 邮件迁移过程[](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="71769-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="71769-106">`Migration mode` 是一种在数据迁移过程中阻止某些操作（如发送邮件和添加成员）的特殊状态。</span><span class="sxs-lookup"><span data-stu-id="71769-106">`Migration mode` is a special state that prevents certain operations, like sending messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="71769-107">完成 **Migration 请求后** ，无法将其他消息导入团队。</span><span class="sxs-lookup"><span data-stu-id="71769-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="71769-108">在请求返回成功响应后，你可以向团队添加成员。</span><span class="sxs-lookup"><span data-stu-id="71769-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="71769-109">权限</span><span class="sxs-lookup"><span data-stu-id="71769-109">Permissions</span></span>

<span data-ttu-id="71769-110">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="71769-110">The following permission is required to call this API.</span></span> <span data-ttu-id="71769-111">若要了解更多信息，*请参阅*[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71769-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71769-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="71769-112">Permission type</span></span>      | <span data-ttu-id="71769-113">权限</span><span class="sxs-lookup"><span data-stu-id="71769-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="71769-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71769-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="71769-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71769-115">Not supported.</span></span>|
| <span data-ttu-id="71769-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71769-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71769-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71769-117">Not supported.</span></span> |
|<span data-ttu-id="71769-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="71769-118">Application</span></span> | <span data-ttu-id="71769-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="71769-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71769-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71769-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="71769-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="71769-121">Request headers</span></span>

| <span data-ttu-id="71769-122">标头</span><span class="sxs-lookup"><span data-stu-id="71769-122">Header</span></span>       | <span data-ttu-id="71769-123">值</span><span class="sxs-lookup"><span data-stu-id="71769-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71769-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71769-124">Authorization</span></span>  | <span data-ttu-id="71769-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71769-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71769-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71769-127">Request body</span></span>

<span data-ttu-id="71769-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71769-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71769-129">响应</span><span class="sxs-lookup"><span data-stu-id="71769-129">Response</span></span>

<span data-ttu-id="71769-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71769-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71769-132">示例</span><span class="sxs-lookup"><span data-stu-id="71769-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="71769-133">请求</span><span class="sxs-lookup"><span data-stu-id="71769-133">Request</span></span>

<span data-ttu-id="71769-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71769-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration
```

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="71769-135">响应</span><span class="sxs-lookup"><span data-stu-id="71769-135">Response</span></span>

<span data-ttu-id="71769-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71769-136">The following is an example of the response.</span></span>
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
