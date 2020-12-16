---
title: 'conversationMember: add'
description: 批量添加成员到团队。
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ffc3d9d36c0f4d22653a961ebe5af4769f286d7d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658330"
---
# <a name="conversationmember-add"></a><span data-ttu-id="1e796-103">conversationMember: add</span><span class="sxs-lookup"><span data-stu-id="1e796-103">conversationMember: add</span></span>

<span data-ttu-id="1e796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e796-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e796-105">在单个请求中将多个成员添加到[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="1e796-105">Add multiple members in a single request to a [team](../resources/team.md).</span></span> <span data-ttu-id="1e796-106">响应提供了有关能够和不能创建哪些成员资格的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1e796-106">The response provides details about which memberships could and could not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e796-107">权限</span><span class="sxs-lookup"><span data-stu-id="1e796-107">Permissions</span></span>

<span data-ttu-id="1e796-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e796-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e796-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e796-110">Permission type</span></span>      | <span data-ttu-id="1e796-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e796-111">Permissions (from least to most privileged)</span></span> | 
|:--------------------|:--------------------------|
| <span data-ttu-id="1e796-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e796-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e796-113">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e796-113">TeamMember.ReadWrite.All</span></span>  |
| <span data-ttu-id="1e796-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e796-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e796-115">不支持</span><span class="sxs-lookup"><span data-stu-id="1e796-115">Not supported</span></span> |
| <span data-ttu-id="1e796-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e796-116">Application</span></span> | <span data-ttu-id="1e796-117">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e796-117">TeamMember.ReadWrite.All</span></span>   |


## <a name="http-request"></a><span data-ttu-id="1e796-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e796-118">HTTP Request</span></span>

<span data-ttu-id="1e796-119">这是在单个请求中将多个元素添加至 **conversationMember** 的绑定操作。</span><span class="sxs-lookup"><span data-stu-id="1e796-119">This is a bound action for adding multiple elements to a **conversationMember** collection in a single request.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a><span data-ttu-id="1e796-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e796-120">Request headers</span></span>

| <span data-ttu-id="1e796-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e796-121">Header</span></span>        | <span data-ttu-id="1e796-122">值</span><span class="sxs-lookup"><span data-stu-id="1e796-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1e796-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e796-123">Authorization</span></span> | <span data-ttu-id="1e796-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e796-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e796-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e796-126">Request body</span></span>
<span data-ttu-id="1e796-127">在请求正文中，提供需要添加到团队的 `conversationMember` 派生对象列表的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e796-127">In the request body, supply the JSON representation of the list of `conversationMember` derivatives that need to be added to the team.</span></span>

<span data-ttu-id="1e796-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1e796-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1e796-129">参数</span><span class="sxs-lookup"><span data-stu-id="1e796-129">Parameter</span></span>|<span data-ttu-id="1e796-130">类型</span><span class="sxs-lookup"><span data-stu-id="1e796-130">Type</span></span>|<span data-ttu-id="1e796-131">说明</span><span class="sxs-lookup"><span data-stu-id="1e796-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e796-132">值</span><span class="sxs-lookup"><span data-stu-id="1e796-132">values</span></span>|<span data-ttu-id="1e796-133">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e796-133">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="1e796-134">应该添加的对话成员列表。</span><span class="sxs-lookup"><span data-stu-id="1e796-134">List of conversation members that should be added.</span></span>|


## <a name="response"></a><span data-ttu-id="1e796-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e796-135">Response</span></span>

<span data-ttu-id="1e796-136">如果成功，此操作将在响应正文中返回 `200 OK` 响应代码和 [actionResultPart ](../resources/actionresultpart.md)的派生对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e796-136">If successful, this action returns a `200 OK` response code and a collection of derivatives of [actionResultPart](../resources/actionresultpart.md) in the response body.</span></span>

<span data-ttu-id="1e796-137">此 API 返回一个 `200` 响应，指示将所有提供的成员添加到团队中，或者返回一个 `207` 响应，指示仅将一些提供的成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="1e796-137">This API returns a `200` response indicating all members supplied were added to the team or a `207` response indicating that only some of the supplied members were added to the team.</span></span> <span data-ttu-id="1e796-138">调用方应检查响应有效负载，以确定哪些成员添加失败。</span><span class="sxs-lookup"><span data-stu-id="1e796-138">The caller should inspect the response payload to determine which member additions failed.</span></span> <span data-ttu-id="1e796-139">响应正文是 [actionResultPart](../resources/actionresultpart.md) 资源的派生对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e796-139">The response body is a collection of derivatives of the [actionResultPart](../resources/actionresultpart.md) resource.</span></span>

## <a name="examples"></a><span data-ttu-id="1e796-140">示例</span><span class="sxs-lookup"><span data-stu-id="1e796-140">Examples</span></span>

### <a name="example-1-add-members-in-bulk-to-a-team"></a><span data-ttu-id="1e796-141">示例 1：将成员批量添加到团队</span><span class="sxs-lookup"><span data-stu-id="1e796-141">Example 1: Add members in bulk to a team</span></span>

#### <a name="request"></a><span data-ttu-id="1e796-142">请求</span><span class="sxs-lookup"><span data-stu-id="1e796-142">Request</span></span>

<span data-ttu-id="1e796-143">以下示例显示了将多个成员添加到团队的请求。</span><span class="sxs-lookup"><span data-stu-id="1e796-143">The following example shows a request to add multiple members to a team.</span></span>
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="1e796-144">响应</span><span class="sxs-lookup"><span data-stu-id="1e796-144">Response</span></span>

<span data-ttu-id="1e796-145">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="1e796-145">The following is the response.</span></span>

> <span data-ttu-id="1e796-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e796-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.aadUserConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": null
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a><span data-ttu-id="1e796-147">示例 2：批量添加成员并遇到遇到部分失败</span><span class="sxs-lookup"><span data-stu-id="1e796-147">Example 2: Add members in bulk and encounter partial failure</span></span>

#### <a name="request"></a><span data-ttu-id="1e796-148">请求</span><span class="sxs-lookup"><span data-stu-id="1e796-148">Request</span></span>

<span data-ttu-id="1e796-149">以下示例显示了将多个成员添加到团队并会导致部分部分失败的请求。</span><span class="sxs-lookup"><span data-stu-id="1e796-149">The following example shows a request to add multiple members to a team that results in a partial failure.</span></span>

<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team_partial_failure"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="1e796-150">响应</span><span class="sxs-lookup"><span data-stu-id="1e796-150">Response</span></span>

<span data-ttu-id="1e796-151">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="1e796-151">The following is the response.</span></span>

> <span data-ttu-id="1e796-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e796-152">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 207 MULTI-STATUS
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.addConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": {
                "code": "NotFound",
                "message": ""
            }
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="1e796-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1e796-153">See also</span></span>

- [<span data-ttu-id="1e796-154">添加成员至团队</span><span class="sxs-lookup"><span data-stu-id="1e796-154">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add members to team in bulk",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
