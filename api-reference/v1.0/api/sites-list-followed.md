---
author: learafa
description: 已登录用户的关注网站列表。
title: 关注网站列表
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: 4520d428511601ad2fa17c4d993a6ab373566eb0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473677"
---
# <a name="list-followed-sites"></a><span data-ttu-id="891f0-103">关注网站列表</span><span class="sxs-lookup"><span data-stu-id="891f0-103">List followed sites</span></span>

<span data-ttu-id="891f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="891f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="891f0-105">列出 [已](../resources/site.md) 登录用户关注的网站。</span><span class="sxs-lookup"><span data-stu-id="891f0-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="891f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="891f0-106">Permissions</span></span>

<span data-ttu-id="891f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="891f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="891f0-109">Permission type</span></span>      | <span data-ttu-id="891f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="891f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="891f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="891f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="891f0-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891f0-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="891f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="891f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="891f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="891f0-114">Not supported.</span></span>    |
|<span data-ttu-id="891f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="891f0-115">Application</span></span> | <span data-ttu-id="891f0-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891f0-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="891f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="891f0-117">HTTP request</span></span>

<span data-ttu-id="891f0-118">此方法只能通过 OneDrive for Business 访问。</span><span class="sxs-lookup"><span data-stu-id="891f0-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/followedSites
```
<span data-ttu-id="891f0-119">根据目标用户的 ID 获取网站列表。</span><span class="sxs-lookup"><span data-stu-id="891f0-119">Get a list of the sites followed by a target user, based on its ID.</span></span>

```http
GET /users/{user-id}/followedSites
```
<span data-ttu-id="891f0-120">**注意：** 若要访问其他目标用户的已关注网站列表，需要应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="891f0-120">**Note:** To access another targeted user's list of followed sites, you need application permissions.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="891f0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="891f0-121">Optional query parameters</span></span>
<span data-ttu-id="891f0-122">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="891f0-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="891f0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="891f0-123">Request headers</span></span>

| <span data-ttu-id="891f0-124">名称</span><span class="sxs-lookup"><span data-stu-id="891f0-124">Name</span></span>      |<span data-ttu-id="891f0-125">说明</span><span class="sxs-lookup"><span data-stu-id="891f0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="891f0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="891f0-126">Authorization</span></span>  | <span data-ttu-id="891f0-127">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="891f0-127">Bearer {code}.</span></span> <span data-ttu-id="891f0-128">必需。</span><span class="sxs-lookup"><span data-stu-id="891f0-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="891f0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="891f0-129">Request Body</span></span>

<span data-ttu-id="891f0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="891f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="891f0-131">响应</span><span class="sxs-lookup"><span data-stu-id="891f0-131">Response</span></span>

<span data-ttu-id="891f0-132">此方法返回用户 [正在](../resources/site.md) 跟踪的网站资源的集合。</span><span class="sxs-lookup"><span data-stu-id="891f0-132">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="891f0-133">如果未找到任何网站，则返回空集合。</span><span class="sxs-lookup"><span data-stu-id="891f0-133">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="891f0-134">示例</span><span class="sxs-lookup"><span data-stu-id="891f0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="891f0-135">请求</span><span class="sxs-lookup"><span data-stu-id="891f0-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="891f0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="891f0-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "sites-list-followed", "scopes": "sites.readwrite.all" } -->

```msgraph-interactive
GET /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="891f0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="891f0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sites-list-followed-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="891f0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="891f0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sites-list-followed-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="891f0-139">C#</span><span class="sxs-lookup"><span data-stu-id="891f0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sites-list-followed-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="891f0-140">Java</span><span class="sxs-lookup"><span data-stu-id="891f0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sites-list-followed-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="891f0-141">响应</span><span class="sxs-lookup"><span data-stu-id="891f0-141">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
            "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site",
            "webUrl": "https://contoso.sharepoint.com/teams/1drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "2C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/1drvteam",
                "webId": "2D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,1C712604-1370-44E7-A1F5-426573FDA80A,1D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site1",
            "webUrl": "https://contoso.sharepoint.com/teams/2drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "1C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/2drvteam",
                "webId": "1D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the sites a user is following.",
  "keywords": "site,onedrive.site,list followed sites, followedSites",
  "section": "documentation",
  "tocPath": "Sites/List followed sites",
  "suppressions": [
  ]
}
-->

