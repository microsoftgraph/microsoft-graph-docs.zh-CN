---
title: 列出为用户安装的应用
description: 检索在指定用户的个人范围内安装的应用列表。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d16d2611abd34b0131efb15872e687d6bad227b4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052549"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="0306d-103">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="0306d-103">List apps installed for user</span></span>

<span data-ttu-id="0306d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0306d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0306d-105">检索指定 [用户的个人](../resources/teamsappinstallation.md) 范围内安装的应用 [列表](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="0306d-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

> [!NOTE]
> <span data-ttu-id="0306d-106">**teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。</span><span class="sxs-lookup"><span data-stu-id="0306d-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0306d-107">权限</span><span class="sxs-lookup"><span data-stu-id="0306d-107">Permissions</span></span>

<span data-ttu-id="0306d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0306d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0306d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0306d-110">Permission type</span></span>      | <span data-ttu-id="0306d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0306d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0306d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0306d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0306d-113">TeamsAppInstallation.ReadForUser、TeamsAppInstallation.ReadWriteSelfForUser、TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="0306d-113">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="0306d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0306d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0306d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0306d-115">Not supported.</span></span>    |
|<span data-ttu-id="0306d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0306d-116">Application</span></span> | <span data-ttu-id="0306d-117">TeamsAppInstallation.ReadForUser.All、TeamsAppInstallation.ReadWriteSelfForUser.All、TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="0306d-117">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0306d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0306d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0306d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0306d-119">Optional query parameters</span></span>

<span data-ttu-id="0306d-120">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0306d-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0306d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0306d-121">Request headers</span></span>

| <span data-ttu-id="0306d-122">标头</span><span class="sxs-lookup"><span data-stu-id="0306d-122">Header</span></span>       | <span data-ttu-id="0306d-123">值</span><span class="sxs-lookup"><span data-stu-id="0306d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0306d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0306d-124">Authorization</span></span>  | <span data-ttu-id="0306d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0306d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0306d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0306d-127">Request body</span></span>

<span data-ttu-id="0306d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0306d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0306d-129">响应</span><span class="sxs-lookup"><span data-stu-id="0306d-129">Response</span></span>

<span data-ttu-id="0306d-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0306d-130">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0306d-131">示例</span><span class="sxs-lookup"><span data-stu-id="0306d-131">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="0306d-132">示例 1：列出为指定用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="0306d-132">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="0306d-133">请求</span><span class="sxs-lookup"><span data-stu-id="0306d-133">Request</span></span>

<span data-ttu-id="0306d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0306d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0306d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0306d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
```
# <a name="c"></a>[<span data-ttu-id="0306d-136">C#</span><span class="sxs-lookup"><span data-stu-id="0306d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0306d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0306d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0306d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0306d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0306d-139">Java</span><span class="sxs-lookup"><span data-stu-id="0306d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0306d-140">响应</span><span class="sxs-lookup"><span data-stu-id="0306d-140">Response</span></span>

<span data-ttu-id="0306d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0306d-141">The following is an example of the response.</span></span>
><span data-ttu-id="0306d-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0306d-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
    },
    {
      "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk="
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="0306d-143">示例 2：获取为用户安装的应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="0306d-143">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="0306d-144">请求</span><span class="sxs-lookup"><span data-stu-id="0306d-144">Request</span></span>

<span data-ttu-id="0306d-145">在下列示例中，如果已安装应用的实例有[机器人](../resources/teamworkbot.md)与它相联系，那么该机器人的详细信息也会被返回。</span><span class="sxs-lookup"><span data-stu-id="0306d-145">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps?$expand=teamsAppDefinition($expand=bot)
```

#### <a name="response"></a><span data-ttu-id="0306d-146">响应</span><span class="sxs-lookup"><span data-stu-id="0306d-146">Response</span></span>

<span data-ttu-id="0306d-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0306d-147">The following is an example of the response.</span></span>

><span data-ttu-id="0306d-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0306d-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7",
                "bot": {
                    "id":"793a57f9-a795-4264-bf8d-3d90585a4d1f"
                }
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```
### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="0306d-149">示例 3：基于关联应用的清单 ID 获取应用安装资源</span><span class="sxs-lookup"><span data-stu-id="0306d-149">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="0306d-150">请求</span><span class="sxs-lookup"><span data-stu-id="0306d-150">Request</span></span>

<span data-ttu-id="0306d-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0306d-151">The following is an example of the request.</span></span> <span data-ttu-id="0306d-152">在此示例中，Teams 应用的清单 ID 为“cf1ba4c7-f94e-4d80-ba90-5594b641a8ee”。</span><span class="sxs-lookup"><span data-stu-id="0306d-152">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="0306d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0306d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="0306d-154">C#</span><span class="sxs-lookup"><span data-stu-id="0306d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-details-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0306d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0306d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-details-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0306d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0306d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-details-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0306d-157">Java</span><span class="sxs-lookup"><span data-stu-id="0306d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-details-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0306d-158">响应</span><span class="sxs-lookup"><span data-stu-id="0306d-158">Response</span></span>

<span data-ttu-id="0306d-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0306d-159">The following is an example of the response.</span></span>

><span data-ttu-id="0306d-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0306d-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details_filter",
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
## <a name="see-also"></a><span data-ttu-id="0306d-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0306d-161">See also</span></span>
- [<span data-ttu-id="0306d-162">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="0306d-162">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


