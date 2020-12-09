---
title: 在用户和 teamsApp 之间获取聊天
description: 检索指定用户与团队应用程序之间的一对一聊天。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cc0be0eb80b35c17b2f0ea6ba38b4dbf1673ac37
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607208"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="dccd4-103">在用户和 teamsApp 之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="dccd4-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="dccd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dccd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dccd4-105">检索指定[用户](../resources/user.md)和[团队应用程序](../resources/teamsapp.md)的[聊天](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="dccd4-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dccd4-106">权限</span><span class="sxs-lookup"><span data-stu-id="dccd4-106">Permissions</span></span>

<span data-ttu-id="dccd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dccd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dccd4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dccd4-109">Permission type</span></span>      | <span data-ttu-id="dccd4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dccd4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dccd4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dccd4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dccd4-112">ReadForUser、TeamsAppInstallation、TeamsAppInstallation TeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="dccd4-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="dccd4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dccd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dccd4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dccd4-114">Not supported.</span></span>    |
|<span data-ttu-id="dccd4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dccd4-115">Application</span></span> | <span data-ttu-id="dccd4-116">TeamsAppInstallation、TeamsAppInstallation、ReadWriteSelfForUser、TeamsAppInstallation。 all</span><span class="sxs-lookup"><span data-stu-id="dccd4-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dccd4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dccd4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dccd4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dccd4-118">Optional query parameters</span></span>

<span data-ttu-id="dccd4-119">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dccd4-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dccd4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dccd4-120">Request headers</span></span>

| <span data-ttu-id="dccd4-121">标头</span><span class="sxs-lookup"><span data-stu-id="dccd4-121">Header</span></span>       | <span data-ttu-id="dccd4-122">值</span><span class="sxs-lookup"><span data-stu-id="dccd4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dccd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dccd4-123">Authorization</span></span>  | <span data-ttu-id="dccd4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dccd4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dccd4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dccd4-126">Request body</span></span>

<span data-ttu-id="dccd4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dccd4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dccd4-128">响应</span><span class="sxs-lookup"><span data-stu-id="dccd4-128">Response</span></span>

<span data-ttu-id="dccd4-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [chat](../resources/chat.md) 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="dccd4-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dccd4-130">示例</span><span class="sxs-lookup"><span data-stu-id="dccd4-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="dccd4-131">示例1：在指定的用户与团队应用程序之间列出一对一聊天</span><span class="sxs-lookup"><span data-stu-id="dccd4-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="dccd4-132">请求</span><span class="sxs-lookup"><span data-stu-id="dccd4-132">Request</span></span>

<span data-ttu-id="dccd4-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dccd4-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```

#### <a name="response"></a><span data-ttu-id="dccd4-134">响应</span><span class="sxs-lookup"><span data-stu-id="dccd4-134">Response</span></span>

<span data-ttu-id="dccd4-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dccd4-135">The following is an example of the response.</span></span>
><span data-ttu-id="dccd4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dccd4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
