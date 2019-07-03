---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 30e729b2418ab93b35d33739459b3c75a6705c51
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451470"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="d15ab-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="d15ab-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d15ab-104">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="d15ab-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d15ab-105">权限</span><span class="sxs-lookup"><span data-stu-id="d15ab-105">Permissions</span></span>

<span data-ttu-id="d15ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d15ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d15ab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d15ab-108">Permission type</span></span>      | <span data-ttu-id="d15ab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d15ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d15ab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d15ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d15ab-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15ab-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d15ab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d15ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d15ab-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d15ab-113">Not supported.</span></span>    |
|<span data-ttu-id="d15ab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d15ab-114">Application</span></span> | <span data-ttu-id="d15ab-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15ab-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d15ab-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d15ab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d15ab-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d15ab-117">Optional query parameters</span></span>

<span data-ttu-id="d15ab-118">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d15ab-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d15ab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d15ab-119">Request headers</span></span>

| <span data-ttu-id="d15ab-120">标头</span><span class="sxs-lookup"><span data-stu-id="d15ab-120">Header</span></span>       | <span data-ttu-id="d15ab-121">值</span><span class="sxs-lookup"><span data-stu-id="d15ab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d15ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d15ab-122">Authorization</span></span>  | <span data-ttu-id="d15ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d15ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d15ab-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d15ab-125">Request body</span></span>

<span data-ttu-id="d15ab-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d15ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d15ab-127">响应</span><span class="sxs-lookup"><span data-stu-id="d15ab-127">Response</span></span>

<span data-ttu-id="d15ab-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[teamsApp](../resources/teamsapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d15ab-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d15ab-129">示例</span><span class="sxs-lookup"><span data-stu-id="d15ab-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d15ab-130">请求</span><span class="sxs-lookup"><span data-stu-id="d15ab-130">Request</span></span>

<span data-ttu-id="d15ab-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d15ab-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d15ab-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d15ab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d15ab-133">C#</span><span class="sxs-lookup"><span data-stu-id="d15ab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d15ab-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d15ab-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d15ab-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="d15ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d15ab-136">响应</span><span class="sxs-lookup"><span data-stu-id="d15ab-136">Response</span></span>

<span data-ttu-id="d15ab-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d15ab-137">The following is an example of the response.</span></span>
><span data-ttu-id="d15ab-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d15ab-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d15ab-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d15ab-139">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="d15ab-140">示例--获取已安装应用程序的名称</span><span class="sxs-lookup"><span data-stu-id="d15ab-140">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="d15ab-141">请求</span><span class="sxs-lookup"><span data-stu-id="d15ab-141">Request</span></span>

<span data-ttu-id="d15ab-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d15ab-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d15ab-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d15ab-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d15ab-144">C#</span><span class="sxs-lookup"><span data-stu-id="d15ab-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d15ab-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="d15ab-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d15ab-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="d15ab-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d15ab-147">响应</span><span class="sxs-lookup"><span data-stu-id="d15ab-147">Response</span></span>

<span data-ttu-id="d15ab-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d15ab-148">The following is an example of the response.</span></span>

><span data-ttu-id="d15ab-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d15ab-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d15ab-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d15ab-150">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
