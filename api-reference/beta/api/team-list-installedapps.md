---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 72393fb3c76c7d9b79aac80c3888bb42f4ccc3cc
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607564"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="54dde-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="54dde-103">List apps in team</span></span>

<span data-ttu-id="54dde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54dde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54dde-105">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="54dde-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="54dde-106">权限</span><span class="sxs-lookup"><span data-stu-id="54dde-106">Permissions</span></span>

<span data-ttu-id="54dde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54dde-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54dde-109">Permission type</span></span>      | <span data-ttu-id="54dde-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54dde-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54dde-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54dde-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54dde-112">TeamsAppInstallation、ReadForTeam、TeamsAppInstallation、、、、all、all、all 和 all。 all</span><span class="sxs-lookup"><span data-stu-id="54dde-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="54dde-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54dde-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54dde-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="54dde-114">Not supported.</span></span>    |
|<span data-ttu-id="54dde-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="54dde-115">Application</span></span> | <span data-ttu-id="54dde-116">TeamsAppInstallation \*、TeamsAppInstallation、ReadForTeam、group、group。 all、、、、all、all、all、all 和 all 的所有读写。</span><span class="sxs-lookup"><span data-stu-id="54dde-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="54dde-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="54dde-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="54dde-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54dde-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54dde-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54dde-119">Optional query parameters</span></span>

<span data-ttu-id="54dde-120">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54dde-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54dde-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54dde-121">Request headers</span></span>

| <span data-ttu-id="54dde-122">标头</span><span class="sxs-lookup"><span data-stu-id="54dde-122">Header</span></span>       | <span data-ttu-id="54dde-123">值</span><span class="sxs-lookup"><span data-stu-id="54dde-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54dde-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54dde-124">Authorization</span></span>  | <span data-ttu-id="54dde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54dde-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54dde-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54dde-127">Request body</span></span>

<span data-ttu-id="54dde-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54dde-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54dde-129">响应</span><span class="sxs-lookup"><span data-stu-id="54dde-129">Response</span></span>

<span data-ttu-id="54dde-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="54dde-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54dde-131">示例</span><span class="sxs-lookup"><span data-stu-id="54dde-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="54dde-132">示例1：列出已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="54dde-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="54dde-133">请求</span><span class="sxs-lookup"><span data-stu-id="54dde-133">Request</span></span>

<span data-ttu-id="54dde-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54dde-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```

#### <a name="response"></a><span data-ttu-id="54dde-135">响应</span><span class="sxs-lookup"><span data-stu-id="54dde-135">Response</span></span>

<span data-ttu-id="54dde-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54dde-136">The following is an example of the response.</span></span>
><span data-ttu-id="54dde-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54dde-137">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
        }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="54dde-138">示例2：获取已安装应用程序的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="54dde-138">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="54dde-139">请求</span><span class="sxs-lookup"><span data-stu-id="54dde-139">Request</span></span>

<span data-ttu-id="54dde-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54dde-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="54dde-141">响应</span><span class="sxs-lookup"><span data-stu-id="54dde-141">Response</span></span>

<span data-ttu-id="54dde-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54dde-142">The following is an example of the response.</span></span>

><span data-ttu-id="54dde-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54dde-143">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
            "teamsAppDefinition": {
                "id": "MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
                "teamsAppId": "00001016-de05-492e-9106-4828fc8a8687",
                "azureADAppId": "7df0a125-d3be-4c96-aa54-591f83ff541c",
                "displayName": "Power Automate Actions",
                "version": "1.0.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Be more productive with Microsoft Flow",
                "description": "Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
            "teamsAppDefinition": {
                "id": "MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
                "teamsAppId": "0ae35b36-0fd7-422e-805b-d53af1579093",
                "azureADAppId": "00000003-0000-0ff1-ce00-000000000000",
                "displayName": "SharePoint Pages",
                "version": "1.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Add a tab for a SharePoint news article or page.",
                "description": "This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
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
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="54dde-144">示例3：基于关联应用程序的清单 ID 获取应用程序安装资源</span><span class="sxs-lookup"><span data-stu-id="54dde-144">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="54dde-145">请求</span><span class="sxs-lookup"><span data-stu-id="54dde-145">Request</span></span>

<span data-ttu-id="54dde-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54dde-146">The following is an example of the request.</span></span> <span data-ttu-id="54dde-147">在此示例中，团队应用程序的清单 ID 为 `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee` 。</span><span class="sxs-lookup"><span data-stu-id="54dde-147">In the example, the manifest ID of the Teams app is `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee`.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```http
GET https://graph.microsoft.com/beta/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="54dde-148">响应</span><span class="sxs-lookup"><span data-stu-id="54dde-148">Response</span></span>

<span data-ttu-id="54dde-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54dde-149">The following is an example of the response.</span></span>

><span data-ttu-id="54dde-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54dde-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

