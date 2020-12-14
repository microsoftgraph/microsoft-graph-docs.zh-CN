---
title: 在团队中获取已安装的应用
description: 在团队中安装应用。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3a46a661dd324331a15e334548825af8af0180f2
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659553"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="94ad2-103">在团队中获取已安装的应用</span><span class="sxs-lookup"><span data-stu-id="94ad2-103">Get installed app in team</span></span>

<span data-ttu-id="94ad2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ad2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94ad2-105">检索 [指定](../resources/teamsappinstallation.md) 团队中安装 [的应用](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="94ad2-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94ad2-106">权限</span><span class="sxs-lookup"><span data-stu-id="94ad2-106">Permissions</span></span>

<span data-ttu-id="94ad2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94ad2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94ad2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94ad2-109">Permission type</span></span>      | <span data-ttu-id="94ad2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94ad2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94ad2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94ad2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94ad2-112">TeamsAppInstallation.ReadWriteSelfForTeam、TeamsAppInstallation.ReadForUser、TeamsAppInstallation.ReadForTeam、TeamsAppInstallation.ReadWriteForTeam、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ad2-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="94ad2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94ad2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ad2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="94ad2-114">Not supported.</span></span>    |
|<span data-ttu-id="94ad2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="94ad2-115">Application</span></span> | <span data-ttu-id="94ad2-116">TeamsAppInstallation.ReadWriteSelfForTeam、TeamsAppInstallation.ReadForTeam.All、TeamsAppInstallation.ReadWriteForTeam.All、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ad2-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94ad2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94ad2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94ad2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="94ad2-118">Request headers</span></span>

| <span data-ttu-id="94ad2-119">标头</span><span class="sxs-lookup"><span data-stu-id="94ad2-119">Header</span></span>       | <span data-ttu-id="94ad2-120">值</span><span class="sxs-lookup"><span data-stu-id="94ad2-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94ad2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94ad2-121">Authorization</span></span>  | <span data-ttu-id="94ad2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94ad2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94ad2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="94ad2-124">Request body</span></span>

<span data-ttu-id="94ad2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94ad2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94ad2-126">响应</span><span class="sxs-lookup"><span data-stu-id="94ad2-126">Response</span></span>

<span data-ttu-id="94ad2-127">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [teamsAppInstallation](../resources/teamsappinstallation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94ad2-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94ad2-128">示例</span><span class="sxs-lookup"><span data-stu-id="94ad2-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="94ad2-129">示例 1：获取已安装的应用</span><span class="sxs-lookup"><span data-stu-id="94ad2-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="94ad2-130">请求</span><span class="sxs-lookup"><span data-stu-id="94ad2-130">Request</span></span>

<span data-ttu-id="94ad2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94ad2-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94ad2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ad2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="94ad2-133">C#</span><span class="sxs-lookup"><span data-stu-id="94ad2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ad2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ad2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ad2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ad2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ad2-136">Java</span><span class="sxs-lookup"><span data-stu-id="94ad2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="94ad2-137">响应</span><span class="sxs-lookup"><span data-stu-id="94ad2-137">Response</span></span>

<span data-ttu-id="94ad2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94ad2-138">The following is an example of the response.</span></span>
><span data-ttu-id="94ad2-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94ad2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="94ad2-141">示例 2：获取已安装应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="94ad2-141">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="94ad2-142">请求</span><span class="sxs-lookup"><span data-stu-id="94ad2-142">Request</span></span>

<span data-ttu-id="94ad2-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94ad2-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94ad2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ad2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="94ad2-145">C#</span><span class="sxs-lookup"><span data-stu-id="94ad2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ad2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ad2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ad2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ad2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ad2-148">Java</span><span class="sxs-lookup"><span data-stu-id="94ad2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="94ad2-149">响应</span><span class="sxs-lookup"><span data-stu-id="94ad2-149">Response</span></span>

<span data-ttu-id="94ad2-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94ad2-150">The following is an example of the response.</span></span>

><span data-ttu-id="94ad2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94ad2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
                "version": "beta"
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

