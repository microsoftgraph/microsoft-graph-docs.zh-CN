---
title: 列出团队中的应用
description: 检索指定团队中安装的应用列表。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09f278087073b70fc66fb052c8178f1fbbc37807
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962783"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="0ea72-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="0ea72-103">List apps in team</span></span>

<span data-ttu-id="0ea72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ea72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea72-105">检索指定 [团队中](../resources/teamsappinstallation.md) 安装的应用 [列表](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="0ea72-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea72-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ea72-106">Permissions</span></span>

<span data-ttu-id="0ea72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ea72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea72-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ea72-109">Permission type</span></span>      | <span data-ttu-id="0ea72-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ea72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea72-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea72-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea72-112">TeamsAppInstallation.ReadForTeam、TeamsAppInstallation.ReadWriteForTeam、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea72-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0ea72-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea72-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea72-114">Not supported.</span></span>    |
|<span data-ttu-id="0ea72-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ea72-115">Application</span></span> | <span data-ttu-id="0ea72-116">TeamsAppInstallation.Read.Group\*、TeamsAppInstallation.ReadForTeam.All、TeamsAppInstallation.ReadWriteForTeam.All、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea72-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0ea72-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="0ea72-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="0ea72-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ea72-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ea72-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ea72-119">Optional query parameters</span></span>

<span data-ttu-id="0ea72-120">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ea72-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea72-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ea72-121">Request headers</span></span>

| <span data-ttu-id="0ea72-122">标头</span><span class="sxs-lookup"><span data-stu-id="0ea72-122">Header</span></span>       | <span data-ttu-id="0ea72-123">值</span><span class="sxs-lookup"><span data-stu-id="0ea72-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ea72-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea72-124">Authorization</span></span>  | <span data-ttu-id="0ea72-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ea72-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ea72-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ea72-127">Request body</span></span>

<span data-ttu-id="0ea72-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ea72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea72-129">响应</span><span class="sxs-lookup"><span data-stu-id="0ea72-129">Response</span></span>

<span data-ttu-id="0ea72-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0ea72-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ea72-131">示例</span><span class="sxs-lookup"><span data-stu-id="0ea72-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="0ea72-132">示例 1：列出已安装的应用</span><span class="sxs-lookup"><span data-stu-id="0ea72-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="0ea72-133">请求</span><span class="sxs-lookup"><span data-stu-id="0ea72-133">Request</span></span>

<span data-ttu-id="0ea72-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ea72-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ea72-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea72-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="0ea72-136">C#</span><span class="sxs-lookup"><span data-stu-id="0ea72-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ea72-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea72-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ea72-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea72-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ea72-139">Java</span><span class="sxs-lookup"><span data-stu-id="0ea72-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ea72-140">响应</span><span class="sxs-lookup"><span data-stu-id="0ea72-140">Response</span></span>

<span data-ttu-id="0ea72-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ea72-141">The following is an example of the response.</span></span>
><span data-ttu-id="0ea72-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ea72-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
      }
   ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="0ea72-143">示例 2：获取已安装应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="0ea72-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="0ea72-144">请求</span><span class="sxs-lookup"><span data-stu-id="0ea72-144">Request</span></span>

<span data-ttu-id="0ea72-145">在下列示例中，如果已安装应用的实例有[机器人](../resources/teamworkbot.md)与它相联系，那么该机器人的详细信息也会被返回。</span><span class="sxs-lookup"><span data-stu-id="0ea72-145">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>


<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition($expand=bot)
```

#### <a name="response"></a><span data-ttu-id="0ea72-146">响应</span><span class="sxs-lookup"><span data-stu-id="0ea72-146">Response</span></span>

<span data-ttu-id="0ea72-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ea72-147">The following is an example of the response.</span></span>

><span data-ttu-id="0ea72-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ea72-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
         "teamsAppDefinition":{
            "id":"MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
            "teamsAppId":"00001016-de05-492e-9106-4828fc8a8687",
            "azureADAppId":"7df0a125-d3be-4c96-aa54-591f83ff541c",
            "displayName":"Power Automate Actions",
            "version":"1.0.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortdescription":"Be more productive with Microsoft Flow",
            "description":"Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
            "lastModifiedDateTime":null,
            "createdBy":null,
            "bot":{
               "id":"9a58a3ec-6b68-4818-ac11-844f1c326784"
            }
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
         "teamsAppDefinition":{
            "id":"MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
            "teamsAppId":"0ae35b36-0fd7-422e-805b-d53af1579093",
            "azureADAppId":"00000003-0000-0ff1-ce00-000000000000",
            "displayName":"SharePoint Pages",
            "version":"1.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortdescription":"Add a tab for a SharePoint news article or page.",
            "description":"This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
         "teamsAppDefinition":{
            "id":"MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
            "teamsAppId":"0d820ecd-def2-4297-adad-78056cde7c78",
            "azureADAppId":"2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
            "displayName":"OneNote",
            "version":"1.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortdescription":"Capture and share ideas, to-do lists and other notes with your team.",
            "description":"Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      }
   ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="0ea72-149">示例 3：基于关联应用的清单 ID 获取应用安装资源</span><span class="sxs-lookup"><span data-stu-id="0ea72-149">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="0ea72-150">请求</span><span class="sxs-lookup"><span data-stu-id="0ea72-150">Request</span></span>

<span data-ttu-id="0ea72-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ea72-151">The following is an example of the request.</span></span> <span data-ttu-id="0ea72-152">在示例中，Teams 应用的清单 ID 为 `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee` 。</span><span class="sxs-lookup"><span data-stu-id="0ea72-152">In the example, the manifest ID of the Teams app is `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee`.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ea72-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea72-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="0ea72-154">C#</span><span class="sxs-lookup"><span data-stu-id="0ea72-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ea72-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea72-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ea72-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea72-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ea72-157">Java</span><span class="sxs-lookup"><span data-stu-id="0ea72-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ea72-158">响应</span><span class="sxs-lookup"><span data-stu-id="0ea72-158">Response</span></span>

<span data-ttu-id="0ea72-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ea72-159">The following is an example of the response.</span></span>

><span data-ttu-id="0ea72-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ea72-160">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team_expand_filter_externalid",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.count":1,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
         "teamsApp":{
            "id":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "externalId":"cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName":"YPA",
            "distributionMethod":"sideloaded"
         },
         "teamsAppDefinition":{
            "id":"MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
            "teamsAppId":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "azureADAppId":"9fc97ea2-c417-4c76-a2db-197612067b28",
            "displayName":"YPA",
            "version":"6.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortdescription":"A conversational smart assistant from MSX that surfaces real-time insights.",
            "description":"For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

