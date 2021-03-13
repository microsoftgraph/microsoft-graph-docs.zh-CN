---
title: 列出聊天中的应用
description: 列出聊天中安装的应用。
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e2d05bdcb34a22170264d3858d07dbf8509f226
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777557"
---
# <a name="list-apps-in-chat"></a><span data-ttu-id="1378a-103">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="1378a-103">List apps in chat</span></span>

<span data-ttu-id="1378a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1378a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1378a-105">列出[聊天](../resources/chat.md)中的所有[应用安装](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="1378a-105">List all [app installations](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="1378a-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md)实例关联，则实际上，将列出安装在会议中的 **teamsApp。**</span><span class="sxs-lookup"><span data-stu-id="1378a-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** s installed in the meeting will be listed.</span></span>

> [!NOTE]
> <span data-ttu-id="1378a-107">**teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。</span><span class="sxs-lookup"><span data-stu-id="1378a-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>


## <a name="permissions"></a><span data-ttu-id="1378a-108">权限</span><span class="sxs-lookup"><span data-stu-id="1378a-108">Permissions</span></span>

<span data-ttu-id="1378a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1378a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1378a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1378a-111">Permission type</span></span>      | <span data-ttu-id="1378a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1378a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1378a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1378a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1378a-114">TeamsAppInstallation.ReadForChat、TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="1378a-114">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="1378a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1378a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1378a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1378a-116">Not supported.</span></span>    |
|<span data-ttu-id="1378a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1378a-117">Application</span></span> | <span data-ttu-id="1378a-118">TeamsAppInstallation.ReadForChat.All、TeamsAppInstallation.ReadWriteSelfForChat.All、TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="1378a-118">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1378a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1378a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{chat-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1378a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1378a-120">Optional query parameters</span></span>

<span data-ttu-id="1378a-121">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1378a-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1378a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1378a-122">Request headers</span></span>

| <span data-ttu-id="1378a-123">标头</span><span class="sxs-lookup"><span data-stu-id="1378a-123">Header</span></span>       | <span data-ttu-id="1378a-124">值</span><span class="sxs-lookup"><span data-stu-id="1378a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1378a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1378a-125">Authorization</span></span>  | <span data-ttu-id="1378a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1378a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1378a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1378a-128">Request body</span></span>

<span data-ttu-id="1378a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1378a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1378a-130">响应</span><span class="sxs-lookup"><span data-stu-id="1378a-130">Response</span></span>

<span data-ttu-id="1378a-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1378a-131">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1378a-132">示例</span><span class="sxs-lookup"><span data-stu-id="1378a-132">Examples</span></span>

### <a name="example-1-get-all-the-apps-installed-in-the-specified-chat"></a><span data-ttu-id="1378a-133">示例 1：获取在指定聊天中安装的所有应用</span><span class="sxs-lookup"><span data-stu-id="1378a-133">Example 1: Get all the apps installed in the specified chat</span></span>

#### <a name="request"></a><span data-ttu-id="1378a-134">请求</span><span class="sxs-lookup"><span data-stu-id="1378a-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps
```


#### <a name="response"></a><span data-ttu-id="1378a-135">响应</span><span class="sxs-lookup"><span data-stu-id="1378a-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsAppInstallation)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps",
    "value": [
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMxYzQzNDBkZS0yYTg1LTQwZTUtOGViMC00ZjI5NTM2ODk3OGI="
        }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-in-the-specified-chat"></a><span data-ttu-id="1378a-136">示例 2：获取在指定聊天中安装的应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="1378a-136">Example 2: Get the names and other details of apps installed in the specified chat</span></span>

<span data-ttu-id="1378a-137">在下列示例中，如果已安装应用的实例有[机器人](../resources/teamworkbot.md)与它相联系，那么该机器人的详细信息也会被返回。</span><span class="sxs-lookup"><span data-stu-id="1378a-137">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>

#### <a name="request"></a><span data-ttu-id="1378a-138">请求</span><span class="sxs-lookup"><span data-stu-id="1378a-138">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsAppDefinition($expand=bot)
```

#### <a name="response"></a><span data-ttu-id="1378a-139">响应</span><span class="sxs-lookup"><span data-stu-id="1378a-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsAppInstallation)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps(teamsAppDefinition())",
    "value": [
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
            "teamsAppDefinition": {
                "id": "MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMiMjUHVibGlzaGVk",
                "teamsAppId": "00001016-de05-492e-9106-4828fc8a8687",
                "azureADAppId": "7df0a125-d3be-4c96-aa54-591f83ff541c",
                "displayName": "Power Automate Actions",
                "version": "1.0.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Be more productive with Microsoft Flow",
                "description": "Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
                "lastModifiedDateTime": null,
                "createdBy": null,
                "bot": {
                    "id":"9a58a3ec-6b68-4818-ac11-844f1c326784"
                }
            }
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMCMjUHVibGlzaGVk",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "azureADAppId": "2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
                "displayName": "OneNote",
                "version": "1.0.0",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Capture and share ideas, to-do lists and other notes with your team.",
                "description": "Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMxYzQzNDBkZS0yYTg1LTQwZTUtOGViMC00ZjI5NTM2ODk3OGI=",
            "teamsAppDefinition": {
                "id": "MWM0MzQwZGUtMmE4NS00MGU1LThlYjAtNGYyOTUzNjg5NzhiIyMxLjMjI1B1Ymxpc2hlZA==",
                "teamsAppId": "1c4340de-2a85-40e5-8eb0-4f295368978b",
                "azureADAppId": null,
                "displayName": "Power BI",
                "version": "1.3",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Easily see and chat about Power BI reports",
                "description": "Pin Power BI reports to your channel to start a conversation about your data. With reports and chats in the same place, everyone stays on the same page.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="1378a-140">示例 3：基于关联应用的清单 id 获取应用安装资源</span><span class="sxs-lookup"><span data-stu-id="1378a-140">Example 3: Get the app installation resource based on the manifest id of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="1378a-141">请求</span><span class="sxs-lookup"><span data-stu-id="1378a-141">Request</span></span>

<span data-ttu-id="1378a-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1378a-142">The following is an example of the request.</span></span> <span data-ttu-id="1378a-143">在此示例中，Teams 应用的清单 ID 为“cf1ba4c7-f94e-4d80-ba90-5594b641a8ee”。</span><span class="sxs-lookup"><span data-stu-id="1378a-143">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```


#### <a name="response"></a><span data-ttu-id="1378a-144">响应</span><span class="sxs-lookup"><span data-stu-id="1378a-144">Response</span></span>

<span data-ttu-id="1378a-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1378a-145">The following is an example of the response.</span></span>

><span data-ttu-id="1378a-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1378a-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_chat_expand_filter",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
            "teamsApp": {
                "id": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
                "displayName": "YPA",
                "distributionMethod": "sideloaded"
            },
            "teamsAppDefinition": {
                "id": "MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
                "teamsAppId": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "azureADAppId": "9fc97ea2-c417-4c76-a2db-197612067b28",
                "displayName": "YPA",
                "version": "6.0.0",
                "requiredResourceSpecificApplicationPermissions": [
                ],
                "publishingState": "published",
                "shortdescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="1378a-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1378a-147">See also</span></span>
- [<span data-ttu-id="1378a-148">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="1378a-148">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat list installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
