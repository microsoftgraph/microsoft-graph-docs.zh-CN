---
title: 列出团队中的应用
description: 检索指定团队中安装的应用列表。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 24c3de7479de6f4d380b50a5c917f99b5495f9bb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470702"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="e4c4f-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="e4c4f-103">List apps in team</span></span>

<span data-ttu-id="e4c4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4c4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4c4f-105">检索指定 [团队中安装](../resources/teamsappinstallation.md) 的应用 [列表](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-105">Retrieve a list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>


> [!NOTE]
> <span data-ttu-id="e4c4f-106">**teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4c4f-107">权限</span><span class="sxs-lookup"><span data-stu-id="e4c4f-107">Permissions</span></span>

<span data-ttu-id="e4c4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4c4f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4c4f-110">Permission type</span></span>      | <span data-ttu-id="e4c4f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4c4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4c4f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4c4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4c4f-113">TeamsAppInstallation.ReadForTeam、TeamsAppInstallation.ReadWriteForTeam、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4c4f-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e4c4f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4c4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4c4f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-115">Not supported.</span></span>    |
|<span data-ttu-id="e4c4f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4c4f-116">Application</span></span> | <span data-ttu-id="e4c4f-117">TeamsAppInstallation.Read.Group\*、TeamsAppInstallation.ReadForTeam.All、TeamsAppInstallation.ReadWriteForTeam.All、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4c4f-117">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e4c4f-118">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="e4c4f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4c4f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4c4f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e4c4f-120">Optional query parameters</span></span>

<span data-ttu-id="e4c4f-121">此方法支持 `$filter` ， `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-121">This method supports the `$filter`, `$select`, and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4c4f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4c4f-122">Request headers</span></span>

| <span data-ttu-id="e4c4f-123">标头</span><span class="sxs-lookup"><span data-stu-id="e4c4f-123">Header</span></span>       | <span data-ttu-id="e4c4f-124">值</span><span class="sxs-lookup"><span data-stu-id="e4c4f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4c4f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4c4f-125">Authorization</span></span>  | <span data-ttu-id="e4c4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4c4f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4c4f-128">Request body</span></span>

<span data-ttu-id="e4c4f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4c4f-130">响应</span><span class="sxs-lookup"><span data-stu-id="e4c4f-130">Response</span></span>

<span data-ttu-id="e4c4f-131">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-131">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4c4f-132">示例</span><span class="sxs-lookup"><span data-stu-id="e4c4f-132">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="e4c4f-133">示例 1：列出已安装的应用</span><span class="sxs-lookup"><span data-stu-id="e4c4f-133">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="e4c4f-134">请求</span><span class="sxs-lookup"><span data-stu-id="e4c4f-134">Request</span></span>

<span data-ttu-id="e4c4f-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4c4f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c4f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="e4c4f-137">C#</span><span class="sxs-lookup"><span data-stu-id="e4c4f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4c4f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4c4f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4c4f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4c4f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4c4f-140">Java</span><span class="sxs-lookup"><span data-stu-id="e4c4f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4c4f-141">响应</span><span class="sxs-lookup"><span data-stu-id="e4c4f-141">Response</span></span>

<span data-ttu-id="e4c4f-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-142">The following is an example of the response.</span></span>
><span data-ttu-id="e4c4f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="e4c4f-145">示例 2：获取已安装应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="e4c4f-145">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="e4c4f-146">请求</span><span class="sxs-lookup"><span data-stu-id="e4c4f-146">Request</span></span>

<span data-ttu-id="e4c4f-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4c4f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c4f-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="e4c4f-149">C#</span><span class="sxs-lookup"><span data-stu-id="e4c4f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4c4f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4c4f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4c4f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4c4f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4c4f-152">Java</span><span class="sxs-lookup"><span data-stu-id="e4c4f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4c4f-153">响应</span><span class="sxs-lookup"><span data-stu-id="e4c4f-153">Response</span></span>

<span data-ttu-id="e4c4f-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-154">The following is an example of the response.</span></span>

><span data-ttu-id="e4c4f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
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
                "shortDescription": "Be more productive with Microsoft Flow",
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
                "shortDescription": "Add a tab for a SharePoint news article or page.",
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
                "shortDescription": "Capture and share ideas, to-do lists and other notes with your team.",
                "description": "Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="e4c4f-157">示例 3：基于关联应用的清单 ID 获取应用安装资源</span><span class="sxs-lookup"><span data-stu-id="e4c4f-157">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="e4c4f-158">请求</span><span class="sxs-lookup"><span data-stu-id="e4c4f-158">Request</span></span>

<span data-ttu-id="e4c4f-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-159">The following is an example of the request.</span></span> <span data-ttu-id="e4c4f-160">在此示例中，Teams 应用的清单 ID 为“cf1ba4c7-f94e-4d80-ba90-5594b641a8ee”。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-160">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4c4f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4c4f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="e4c4f-162">C#</span><span class="sxs-lookup"><span data-stu-id="e4c4f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4c4f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4c4f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4c4f-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4c4f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4c4f-165">Java</span><span class="sxs-lookup"><span data-stu-id="e4c4f-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4c4f-166">响应</span><span class="sxs-lookup"><span data-stu-id="e4c4f-166">Response</span></span>

<span data-ttu-id="e4c4f-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-167">The following is an example of the response.</span></span>

><span data-ttu-id="e4c4f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e4c4f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
                "shortDescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
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

## <a name="see-also"></a><span data-ttu-id="e4c4f-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e4c4f-170">See also</span></span>
- [<span data-ttu-id="e4c4f-171">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="e4c4f-171">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
