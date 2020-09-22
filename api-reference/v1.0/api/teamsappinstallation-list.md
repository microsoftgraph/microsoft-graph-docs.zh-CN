---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dfe6d2748fa3fd148292e005a9f600a0568627fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978375"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="c4e67-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="c4e67-103">List apps in team</span></span>

<span data-ttu-id="c4e67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4e67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4e67-105">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="c4e67-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4e67-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4e67-106">Permissions</span></span>

<span data-ttu-id="c4e67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4e67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4e67-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4e67-109">Permission type</span></span>      | <span data-ttu-id="c4e67-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4e67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4e67-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4e67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4e67-112">TeamsAppInstallation、ReadForTeam、TeamsAppInstallation、、、、all、all、all 和 all。 all</span><span class="sxs-lookup"><span data-stu-id="c4e67-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c4e67-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4e67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4e67-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4e67-114">Not supported.</span></span>    |
|<span data-ttu-id="c4e67-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4e67-115">Application</span></span> | <span data-ttu-id="c4e67-116">TeamsAppInstallation、TeamsAppInstallation、ReadForTeam、、、、、all、all、all、all 和 All。</span><span class="sxs-lookup"><span data-stu-id="c4e67-116">TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4e67-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4e67-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4e67-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4e67-118">Optional query parameters</span></span>

<span data-ttu-id="c4e67-119">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4e67-119">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4e67-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4e67-120">Request headers</span></span>

| <span data-ttu-id="c4e67-121">标头</span><span class="sxs-lookup"><span data-stu-id="c4e67-121">Header</span></span>       | <span data-ttu-id="c4e67-122">值</span><span class="sxs-lookup"><span data-stu-id="c4e67-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4e67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4e67-123">Authorization</span></span>  | <span data-ttu-id="c4e67-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4e67-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4e67-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4e67-126">Request body</span></span>

<span data-ttu-id="c4e67-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4e67-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4e67-128">响应</span><span class="sxs-lookup"><span data-stu-id="c4e67-128">Response</span></span>

<span data-ttu-id="c4e67-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4e67-129">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4e67-130">示例</span><span class="sxs-lookup"><span data-stu-id="c4e67-130">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="c4e67-131">示例1：列出已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="c4e67-131">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="c4e67-132">请求</span><span class="sxs-lookup"><span data-stu-id="c4e67-132">Request</span></span>

<span data-ttu-id="c4e67-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4e67-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4e67-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4e67-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps
```
# <a name="c"></a>[<span data-ttu-id="c4e67-135">C#</span><span class="sxs-lookup"><span data-stu-id="c4e67-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4e67-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4e67-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4e67-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4e67-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4e67-138">Java</span><span class="sxs-lookup"><span data-stu-id="c4e67-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c4e67-139">响应</span><span class="sxs-lookup"><span data-stu-id="c4e67-139">Response</span></span>

<span data-ttu-id="c4e67-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4e67-140">The following is an example of the response.</span></span>
><span data-ttu-id="c4e67-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4e67-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4e67-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4e67-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
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
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="c4e67-143">示例2：获取已安装应用程序的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="c4e67-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="c4e67-144">请求</span><span class="sxs-lookup"><span data-stu-id="c4e67-144">Request</span></span>

<span data-ttu-id="c4e67-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4e67-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4e67-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4e67-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="c4e67-147">C#</span><span class="sxs-lookup"><span data-stu-id="c4e67-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4e67-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4e67-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4e67-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4e67-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4e67-150">Java</span><span class="sxs-lookup"><span data-stu-id="c4e67-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c4e67-151">响应</span><span class="sxs-lookup"><span data-stu-id="c4e67-151">Response</span></span>

<span data-ttu-id="c4e67-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4e67-152">The following is an example of the response.</span></span>

><span data-ttu-id="c4e67-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4e67-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4e67-154">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4e67-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
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
                "version": "1.7"
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

