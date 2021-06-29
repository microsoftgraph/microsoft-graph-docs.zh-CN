---
title: 聊天的列表权限权限
description: 检索聊天的权限权限。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 258bc1132f8a8f030a148b43a4ba04b1ebbba0eb
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162236"
---
# <a name="list-permissiongrants-of-a-chat"></a><span data-ttu-id="a06df-103">聊天的列表权限权限</span><span class="sxs-lookup"><span data-stu-id="a06df-103">List permissionGrants of a chat</span></span>

<span data-ttu-id="a06df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a06df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a06df-p101">列出 [聊天](../resources/chat.md) 的所有 [特定于资源的权限授予](../resources/resourcespecificpermissiongrant.md)。此列表指定有权访问 **聊天** 的 Azure AD 应用，以及每个应用具有的相应类型的特定于资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a06df-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [chat](../resources/chat.md). This list specifies the Azure AD apps that have access to the **chat**, along with the corresponding kind of resource-specific access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="a06df-107">权限</span><span class="sxs-lookup"><span data-stu-id="a06df-107">Permissions</span></span>

<span data-ttu-id="a06df-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a06df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a06df-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a06df-110">Permission Type</span></span>                        | <span data-ttu-id="a06df-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a06df-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                        |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a06df-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a06df-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a06df-113">ResourceSificPermissionGrant.ReadFor你、TeamsAppInstallation.ReadFor如果一、TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteFor一并</span><span class="sxs-lookup"><span data-stu-id="a06df-113">ResourceSpecificPermissionGrant.ReadForChat, TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span>                                    |
| <span data-ttu-id="a06df-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a06df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a06df-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a06df-115">Not supported.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="a06df-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a06df-116">Application</span></span>                            | <span data-ttu-id="a06df-117">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="a06df-117">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="a06df-118">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a06df-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="a06df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a06df-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a06df-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a06df-120">Optional query parameters</span></span>

<span data-ttu-id="a06df-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a06df-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a06df-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a06df-122">Request headers</span></span>

| <span data-ttu-id="a06df-123">标头</span><span class="sxs-lookup"><span data-stu-id="a06df-123">Header</span></span>           | <span data-ttu-id="a06df-124">值</span><span class="sxs-lookup"><span data-stu-id="a06df-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="a06df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a06df-125">Authorization</span></span>    | <span data-ttu-id="a06df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a06df-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a06df-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a06df-128">Request body</span></span>

<span data-ttu-id="a06df-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a06df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a06df-130">响应</span><span class="sxs-lookup"><span data-stu-id="a06df-130">Response</span></span>

<span data-ttu-id="a06df-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a06df-131">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a06df-132">示例</span><span class="sxs-lookup"><span data-stu-id="a06df-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a06df-133">请求</span><span class="sxs-lookup"><span data-stu-id="a06df-133">Request</span></span>

<span data-ttu-id="a06df-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a06df-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a06df-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a06df-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="a06df-136">C#</span><span class="sxs-lookup"><span data-stu-id="a06df-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a06df-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a06df-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a06df-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a06df-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a06df-139">Java</span><span class="sxs-lookup"><span data-stu-id="a06df-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="a06df-140">响应</span><span class="sxs-lookup"><span data-stu-id="a06df-140">Response</span></span>

<span data-ttu-id="a06df-141">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a06df-141">The following example shows the response.</span></span>

><span data-ttu-id="a06df-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a06df-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#permissionGrants",
   "value":[
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"ChatSettings.ReadWrite.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsAppInstallation.Read.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc1RhYi5EZWxldGUuQ2hhdCMjQXBwbGljYXRpb24=",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsTab.Delete.Chat"
      },
      {
         "id":"ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
         "clientAppId":"69024002-35ae-4574-a219-f261183580b4",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"74c92190-dc0e-485a-81c6-fdffd4aadfd8",
         "permissionType":"Application",
         "permission":"ChatSettings.Read.Chat"
      }
   ]
}
```

## <a name="see-also"></a><span data-ttu-id="a06df-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a06df-143">See also</span></span>
- [<span data-ttu-id="a06df-144">列出团队的权限授予</span><span class="sxs-lookup"><span data-stu-id="a06df-144">List permission grants of a team</span></span>](team-list-permissionGrants.md)
- [<span data-ttu-id="a06df-145">组的列表权限管理</span><span class="sxs-lookup"><span data-stu-id="a06df-145">List permission grants of a group</span></span>](group-list-permissionGrants.md)