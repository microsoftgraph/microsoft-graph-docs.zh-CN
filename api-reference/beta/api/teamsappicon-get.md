---
title: 获取 teamsAppIcon
description: 检索与 Teams 应用的特定定义相关联的图标。
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e80b20f0802fbfa084c02b9103e7362be9ca159
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921759"
---
# <a name="get-teamsappicon"></a><span data-ttu-id="2f861-103">获取 teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="2f861-103">Get teamsAppIcon</span></span>

<span data-ttu-id="2f861-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f861-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f861-105">检索与 [应用](../resources/teamsappicon.md) 的特定 [定义相关联的](../resources/teamsappdefinition.md) Teams 应用 [图标](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="2f861-105">Retrieve a [Teams app icon](../resources/teamsappicon.md) associated with a specific [definition](../resources/teamsappdefinition.md) of an [app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f861-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f861-106">Permissions</span></span>

<span data-ttu-id="2f861-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f861-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f861-109">Permission Type</span></span>                        | <span data-ttu-id="2f861-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f861-110">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="2f861-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f861-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f861-112">AppCatalog.Read.All、AppCatalog.ReadWrite.All、AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="2f861-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="2f861-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f861-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f861-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f861-114">Not supported.</span></span>                                                   |
| <span data-ttu-id="2f861-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f861-115">Application</span></span>                            | <span data-ttu-id="2f861-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f861-116">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="2f861-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f861-117">HTTP request</span></span>

<span data-ttu-id="2f861-118">**获取 Teams 应用定义的颜色图标**</span><span class="sxs-lookup"><span data-stu-id="2f861-118">**Get color icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon
```

<span data-ttu-id="2f861-119">**获取 Teams 应用定义的大纲图标**</span><span class="sxs-lookup"><span data-stu-id="2f861-119">**Get outline icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f861-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2f861-120">Optional query parameters</span></span>

<span data-ttu-id="2f861-121">此操作支持 `$select` 使用 `$expand` [和 OData 查询参数](/graph/query-parameters) 自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2f861-121">This operation supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f861-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f861-122">Request headers</span></span>

| <span data-ttu-id="2f861-123">标头</span><span class="sxs-lookup"><span data-stu-id="2f861-123">Header</span></span>           | <span data-ttu-id="2f861-124">值</span><span class="sxs-lookup"><span data-stu-id="2f861-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="2f861-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f861-125">Authorization</span></span>    | <span data-ttu-id="2f861-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f861-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f861-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f861-128">Request body</span></span>

<span data-ttu-id="2f861-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f861-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f861-130">响应</span><span class="sxs-lookup"><span data-stu-id="2f861-130">Response</span></span>

<span data-ttu-id="2f861-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamsAppIcon](../resources/teamsappicon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f861-131">If successful, this method returns a `200 OK` response code and a [teamsAppIcon](../resources/teamsappicon.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f861-132">示例</span><span class="sxs-lookup"><span data-stu-id="2f861-132">Examples</span></span>

### <a name="example-1-get-color-icon-of-a-custom-teams-app"></a><span data-ttu-id="2f861-133">示例 1：获取自定义 *Teams* 应用的颜色图标</span><span class="sxs-lookup"><span data-stu-id="2f861-133">Example 1: Get color icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2f861-134">请求</span><span class="sxs-lookup"><span data-stu-id="2f861-134">Request</span></span>

<span data-ttu-id="2f861-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f861-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f861-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f861-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_coloricon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon
```
# <a name="c"></a>[<span data-ttu-id="2f861-137">C#</span><span class="sxs-lookup"><span data-stu-id="2f861-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-coloricon-customapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f861-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f861-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-coloricon-customapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f861-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f861-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-coloricon-customapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f861-140">Java</span><span class="sxs-lookup"><span data-stu-id="2f861-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-coloricon-customapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f861-141">响应</span><span class="sxs-lookup"><span data-stu-id="2f861-141">Response</span></span>

<span data-ttu-id="2f861-142">以下示例显示组织应用的响应。</span><span class="sxs-lookup"><span data-stu-id="2f861-142">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="2f861-143">**注意**：若要访问自定义应用图标的实际 [图像](teamworkhostedcontent-get.md) ，需要在请求上设置 Microsoft Graph 令牌。</span><span class="sxs-lookup"><span data-stu-id="2f861-143">**Note**: Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/$value"
}
```

### <a name="example-2-get-outline-icon-of-a-custom-teams-app"></a><span data-ttu-id="2f861-144">示例 2：获取自定义 *Teams* 应用的大纲图标</span><span class="sxs-lookup"><span data-stu-id="2f861-144">Example 2: Get outline icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2f861-145">请求</span><span class="sxs-lookup"><span data-stu-id="2f861-145">Request</span></span>

<span data-ttu-id="2f861-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f861-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f861-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f861-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon
```
# <a name="c"></a>[<span data-ttu-id="2f861-148">C#</span><span class="sxs-lookup"><span data-stu-id="2f861-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-customapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f861-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f861-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-customapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f861-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f861-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-customapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f861-151">Java</span><span class="sxs-lookup"><span data-stu-id="2f861-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-customapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f861-152">响应</span><span class="sxs-lookup"><span data-stu-id="2f861-152">Response</span></span>

<span data-ttu-id="2f861-153">以下示例显示组织应用的响应。</span><span class="sxs-lookup"><span data-stu-id="2f861-153">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="2f861-154">**注意**：若要访问自定义应用图标的实际 [图像](teamworkhostedcontent-get.md) ，需要在请求上设置 Microsoft Graph 令牌。</span><span class="sxs-lookup"><span data-stu-id="2f861-154">**Note**:  Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWIxYzU0Mzg0NGE5ZmFjY2Y2YWI4NDdkNWY0NTU0ZGU0L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value"
}
```


### <a name="example-3-get-color-icon-of-a-store-teams-app"></a><span data-ttu-id="2f861-155">示例 3：获取应用商店 *Teams* 应用的颜色图标</span><span class="sxs-lookup"><span data-stu-id="2f861-155">Example 3: Get color icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2f861-156">请求</span><span class="sxs-lookup"><span data-stu-id="2f861-156">Request</span></span>

<span data-ttu-id="2f861-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f861-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f861-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f861-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/colorIcon/
```
# <a name="c"></a>[<span data-ttu-id="2f861-159">C#</span><span class="sxs-lookup"><span data-stu-id="2f861-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-publicapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f861-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f861-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-publicapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f861-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f861-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-publicapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f861-162">Java</span><span class="sxs-lookup"><span data-stu-id="2f861-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-publicapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2f861-163">响应</span><span class="sxs-lookup"><span data-stu-id="2f861-163">Response</span></span>

<span data-ttu-id="2f861-164">以下示例显示了应用商店应用的响应。</span><span class="sxs-lookup"><span data-stu-id="2f861-164">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetateamsgraphdev/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfbGFyZ2VJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_largeImage.png?v=1.0.5"
}
```

### <a name="example-4-get-outline-icon-of-a-store-teams-app"></a><span data-ttu-id="2f861-165">示例 4：获取应用商店 *Teams* 应用的大纲图标</span><span class="sxs-lookup"><span data-stu-id="2f861-165">Example 4: Get outline icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2f861-166">请求</span><span class="sxs-lookup"><span data-stu-id="2f861-166">Request</span></span>

<span data-ttu-id="2f861-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f861-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f861-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f861-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/outlineIcon/
```
# <a name="c"></a>[<span data-ttu-id="2f861-169">C#</span><span class="sxs-lookup"><span data-stu-id="2f861-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-publicapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f861-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f861-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-publicapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f861-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f861-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-publicapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f861-172">Java</span><span class="sxs-lookup"><span data-stu-id="2f861-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-publicapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2f861-173">响应</span><span class="sxs-lookup"><span data-stu-id="2f861-173">Response</span></span>

<span data-ttu-id="2f861-174">以下示例显示了应用商店应用的响应。</span><span class="sxs-lookup"><span data-stu-id="2f861-174">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfc21hbGxJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_smallImage.png?v=1.0.5"
}
```

## <a name="see-also"></a><span data-ttu-id="2f861-175">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2f861-175">See also</span></span>

- [<span data-ttu-id="2f861-176">获取应用图标中的托管内容</span><span class="sxs-lookup"><span data-stu-id="2f861-176">Get hosted content in app's icon</span></span>](teamworkhostedcontent-get.md)
- [<span data-ttu-id="2f861-177">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="2f861-177">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
