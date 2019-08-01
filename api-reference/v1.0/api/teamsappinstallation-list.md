---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee92c3e0235f220e2aeb1bf60806c03df8351085
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027291"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="8e7f4-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="8e7f4-103">List apps in team</span></span>

<span data-ttu-id="8e7f4-104">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e7f4-105">权限</span><span class="sxs-lookup"><span data-stu-id="8e7f4-105">Permissions</span></span>

<span data-ttu-id="8e7f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e7f4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e7f4-108">Permission type</span></span>      | <span data-ttu-id="8e7f4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e7f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e7f4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e7f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e7f4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e7f4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e7f4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e7f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e7f4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-113">Not supported.</span></span>    |
|<span data-ttu-id="8e7f4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e7f4-114">Application</span></span> | <span data-ttu-id="8e7f4-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e7f4-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="8e7f4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e7f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e7f4-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8e7f4-117">Optional query parameters</span></span>

<span data-ttu-id="8e7f4-118">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e7f4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e7f4-119">Request headers</span></span>

| <span data-ttu-id="8e7f4-120">标头</span><span class="sxs-lookup"><span data-stu-id="8e7f4-120">Header</span></span>       | <span data-ttu-id="8e7f4-121">值</span><span class="sxs-lookup"><span data-stu-id="8e7f4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e7f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e7f4-122">Authorization</span></span>  | <span data-ttu-id="8e7f4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e7f4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e7f4-125">Request body</span></span>

<span data-ttu-id="8e7f4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e7f4-127">响应</span><span class="sxs-lookup"><span data-stu-id="8e7f4-127">Response</span></span>

<span data-ttu-id="8e7f4-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[teamsAppInstallation](../resources/teamsappinstallation.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-128">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e7f4-129">示例</span><span class="sxs-lookup"><span data-stu-id="8e7f4-129">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="8e7f4-130">示例 1: 列出已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="8e7f4-130">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="8e7f4-131">请求</span><span class="sxs-lookup"><span data-stu-id="8e7f4-131">Request</span></span>

<span data-ttu-id="8e7f4-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e7f4-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e7f4-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```http
GET /teams/{id}/installedApps
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e7f4-134">C#</span><span class="sxs-lookup"><span data-stu-id="8e7f4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e7f4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e7f4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e7f4-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e7f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e7f4-137">Java</span><span class="sxs-lookup"><span data-stu-id="8e7f4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e7f4-138">响应</span><span class="sxs-lookup"><span data-stu-id="8e7f4-138">Response</span></span>

<span data-ttu-id="8e7f4-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-139">The following is an example of the response.</span></span>
><span data-ttu-id="8e7f4-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e7f4-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-141">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="8e7f4-142">示例 2: 获取已安装应用程序的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="8e7f4-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="8e7f4-143">请求</span><span class="sxs-lookup"><span data-stu-id="8e7f4-143">Request</span></span>

<span data-ttu-id="8e7f4-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e7f4-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e7f4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e7f4-146">C#</span><span class="sxs-lookup"><span data-stu-id="8e7f4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e7f4-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e7f4-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e7f4-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e7f4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e7f4-149">Java</span><span class="sxs-lookup"><span data-stu-id="8e7f4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e7f4-150">响应</span><span class="sxs-lookup"><span data-stu-id="8e7f4-150">Response</span></span>

<span data-ttu-id="8e7f4-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-151">The following is an example of the response.</span></span>

><span data-ttu-id="8e7f4-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e7f4-153">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e7f4-153">All the properties will be returned from an actual call.</span></span>
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
