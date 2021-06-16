---
title: 在团队中获取已安装的应用
description: 在团队中安装应用。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2f27cff7f0f3006fa7704628fdd6b66f944de641
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971396"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="720e5-103">在团队中获取已安装的应用</span><span class="sxs-lookup"><span data-stu-id="720e5-103">Get installed app in team</span></span>

<span data-ttu-id="720e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="720e5-105">检索 [指定](../resources/teamsappinstallation.md) 团队中安装 [的应用](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="720e5-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="720e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="720e5-106">Permissions</span></span>

<span data-ttu-id="720e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="720e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="720e5-109">Permission type</span></span>      | <span data-ttu-id="720e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="720e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="720e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="720e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="720e5-112">TeamsAppInstallation.ReadWriteSelfForTeam、TeamsAppInstallation.ReadForUser、TeamsAppInstallation.ReadForTeam、TeamsAppInstallation.ReadWriteForTeam、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="720e5-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="720e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="720e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="720e5-114">Not supported.</span></span>    |
|<span data-ttu-id="720e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="720e5-115">Application</span></span> | <span data-ttu-id="720e5-116">TeamsAppInstallation.Read.Group\*、TeamsAppInstallation.ReadWriteSelfForTeam、TeamsAppInstallation.ReadForTeam.All、TeamsAppInstallation.ReadWriteForTeam.All、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="720e5-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="720e5-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="720e5-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="720e5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="720e5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="720e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="720e5-119">Request headers</span></span>

| <span data-ttu-id="720e5-120">标头</span><span class="sxs-lookup"><span data-stu-id="720e5-120">Header</span></span>       | <span data-ttu-id="720e5-121">值</span><span class="sxs-lookup"><span data-stu-id="720e5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="720e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="720e5-122">Authorization</span></span>  | <span data-ttu-id="720e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="720e5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="720e5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="720e5-125">Request body</span></span>

<span data-ttu-id="720e5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="720e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="720e5-127">响应</span><span class="sxs-lookup"><span data-stu-id="720e5-127">Response</span></span>

<span data-ttu-id="720e5-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamsAppInstallation](../resources/teamsappinstallation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="720e5-128">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="720e5-129">示例</span><span class="sxs-lookup"><span data-stu-id="720e5-129">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="720e5-130">示例 1：获取已安装的应用</span><span class="sxs-lookup"><span data-stu-id="720e5-130">Example 1: Get the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="720e5-131">请求</span><span class="sxs-lookup"><span data-stu-id="720e5-131">Request</span></span>

<span data-ttu-id="720e5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="720e5-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="720e5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="720e5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="720e5-134">C#</span><span class="sxs-lookup"><span data-stu-id="720e5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="720e5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="720e5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="720e5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="720e5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="720e5-137">Java</span><span class="sxs-lookup"><span data-stu-id="720e5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="720e5-138">响应</span><span class="sxs-lookup"><span data-stu-id="720e5-138">Response</span></span>

<span data-ttu-id="720e5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="720e5-139">The following is an example of the response.</span></span>
><span data-ttu-id="720e5-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="720e5-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="720e5-141">示例 2：获取已安装应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="720e5-141">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="requests"></a><span data-ttu-id="720e5-142">请求</span><span class="sxs-lookup"><span data-stu-id="720e5-142">Requests</span></span>

<span data-ttu-id="720e5-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="720e5-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="720e5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="720e5-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="720e5-145">C#</span><span class="sxs-lookup"><span data-stu-id="720e5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="720e5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="720e5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="720e5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="720e5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="720e5-148">Java</span><span class="sxs-lookup"><span data-stu-id="720e5-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="720e5-149">响应</span><span class="sxs-lookup"><span data-stu-id="720e5-149">Response</span></span>

<span data-ttu-id="720e5-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="720e5-150">The following is an example of the response.</span></span>

><span data-ttu-id="720e5-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="720e5-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
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
