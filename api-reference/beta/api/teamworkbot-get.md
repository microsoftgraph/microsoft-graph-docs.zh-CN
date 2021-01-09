---
title: 获取 teamworkBot
description: 读取团队合作Bot 对象的属性和关系。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05cb2e8e4d6a41028a9f35b82561b4f5b5d80251
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790586"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="e9970-103">获取 teamworkBot</span><span class="sxs-lookup"><span data-stu-id="e9970-103">Get teamworkBot</span></span>

<span data-ttu-id="e9970-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9970-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9970-105">获取与[TeamsApp](../resources/teamsapp.md)的特定[定义](../resources/teamsappdefinition.md)相关联的机器人。</span><span class="sxs-lookup"><span data-stu-id="e9970-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9970-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9970-106">Permissions</span></span>
<span data-ttu-id="e9970-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9970-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9970-109">Permission type</span></span>|<span data-ttu-id="e9970-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e9970-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9970-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9970-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e9970-112">AppCatalog.Submit、AppCatalog.Read.All、AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9970-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="e9970-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9970-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e9970-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9970-114">Not supported.</span></span> |
|<span data-ttu-id="e9970-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9970-115">Application</span></span>| <span data-ttu-id="e9970-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9970-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9970-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9970-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9970-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9970-118">Optional query parameters</span></span>
<span data-ttu-id="e9970-119">此方法支持 `$select` [OData 查询参数](/graph/query-parameter) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9970-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9970-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9970-120">Request headers</span></span>
|<span data-ttu-id="e9970-121">名称</span><span class="sxs-lookup"><span data-stu-id="e9970-121">Name</span></span>|<span data-ttu-id="e9970-122">说明</span><span class="sxs-lookup"><span data-stu-id="e9970-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9970-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9970-123">Authorization</span></span>|<span data-ttu-id="e9970-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9970-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9970-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9970-126">Request body</span></span>
<span data-ttu-id="e9970-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9970-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9970-128">响应</span><span class="sxs-lookup"><span data-stu-id="e9970-128">Response</span></span>

<span data-ttu-id="e9970-129">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [团队合作Bot](../resources/teamworkbot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9970-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9970-130">示例</span><span class="sxs-lookup"><span data-stu-id="e9970-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9970-131">请求</span><span class="sxs-lookup"><span data-stu-id="e9970-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```


### <a name="response"></a><span data-ttu-id="e9970-132">响应</span><span class="sxs-lookup"><span data-stu-id="e9970-132">Response</span></span>
<span data-ttu-id="e9970-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9970-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkBot"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "1f81bb29-bb29-1f81-29bb-811f29bb811f"
}
```
## <a name="see-also"></a><span data-ttu-id="e9970-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e9970-134">See also</span></span>

- <span data-ttu-id="e9970-135">若要在团队中安装机器人，请参阅团队中的[列表应用中的示例 2。](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="e9970-135">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="e9970-136">若要在聊天中安装聊天机器人，请参阅聊天中的 [列表应用中的示例](chat-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="e9970-136">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="e9970-137">若要在用户的个人范围内安装机器人，请参阅为用户安装 [的列表应用中的示例](userteamwork-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="e9970-137">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


