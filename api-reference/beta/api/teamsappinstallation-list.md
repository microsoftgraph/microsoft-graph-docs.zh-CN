---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 98d0528950d2a9af79dfd5bf2b3423d71d1cce84
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637610"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="05257-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="05257-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05257-104">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="05257-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05257-105">权限</span><span class="sxs-lookup"><span data-stu-id="05257-105">Permissions</span></span>

<span data-ttu-id="05257-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05257-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="05257-108">Permission type</span></span>      | <span data-ttu-id="05257-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05257-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05257-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05257-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05257-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05257-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="05257-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05257-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05257-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="05257-113">Not supported.</span></span>    |
|<span data-ttu-id="05257-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="05257-114">Application</span></span> | <span data-ttu-id="05257-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05257-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="05257-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05257-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05257-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05257-117">Optional query parameters</span></span>

<span data-ttu-id="05257-118">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05257-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05257-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="05257-119">Request headers</span></span>

| <span data-ttu-id="05257-120">标头</span><span class="sxs-lookup"><span data-stu-id="05257-120">Header</span></span>       | <span data-ttu-id="05257-121">值</span><span class="sxs-lookup"><span data-stu-id="05257-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05257-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05257-122">Authorization</span></span>  | <span data-ttu-id="05257-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05257-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05257-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="05257-125">Request body</span></span>

<span data-ttu-id="05257-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05257-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05257-127">响应</span><span class="sxs-lookup"><span data-stu-id="05257-127">Response</span></span>

<span data-ttu-id="05257-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[teamsApp](../resources/teamsapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="05257-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05257-129">示例</span><span class="sxs-lookup"><span data-stu-id="05257-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="05257-130">请求</span><span class="sxs-lookup"><span data-stu-id="05257-130">Request</span></span>

<span data-ttu-id="05257-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05257-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="05257-132">响应</span><span class="sxs-lookup"><span data-stu-id="05257-132">Response</span></span>

<span data-ttu-id="05257-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="05257-133">The following is an example of the response.</span></span>
><span data-ttu-id="05257-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05257-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="05257-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05257-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="05257-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="05257-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="05257-137">语言</span><span class="sxs-lookup"><span data-stu-id="05257-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05257-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="05257-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="05257-139">示例--获取已安装应用程序的名称</span><span class="sxs-lookup"><span data-stu-id="05257-139">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="05257-140">请求</span><span class="sxs-lookup"><span data-stu-id="05257-140">Request</span></span>

<span data-ttu-id="05257-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05257-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="05257-142">响应</span><span class="sxs-lookup"><span data-stu-id="05257-142">Response</span></span>

<span data-ttu-id="05257-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="05257-143">The following is an example of the response.</span></span>

><span data-ttu-id="05257-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05257-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="05257-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05257-145">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="05257-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="05257-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="05257-147">语言</span><span class="sxs-lookup"><span data-stu-id="05257-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05257-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="05257-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
