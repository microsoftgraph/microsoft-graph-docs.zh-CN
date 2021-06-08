---
title: 获取 teamworkHostedContent
description: 检索 teamsAppIcon 中的托管内容。
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6317cac369ad8d7bb29ed83c7e2c5ce9a0ca5f5f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788001"
---
# <a name="get-teamworkhostedcontent"></a><span data-ttu-id="e6f70-103">获取 teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="e6f70-103">Get teamworkHostedContent</span></span>

<span data-ttu-id="e6f70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f70-105">在 [应用的图标](../resources/teamworkhostedcontent.md) 中检索 [托管的内容](../resources/teamsappicon.md)。</span><span class="sxs-lookup"><span data-stu-id="e6f70-105">Retrieve the [hosted content](../resources/teamworkhostedcontent.md) in an [app's icon](../resources/teamsappicon.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f70-106">权限</span><span class="sxs-lookup"><span data-stu-id="e6f70-106">Permissions</span></span>

<span data-ttu-id="e6f70-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6f70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-app-icon-in-app-catalog"></a><span data-ttu-id="e6f70-109">应用程序目录中应用程序图标的权限</span><span class="sxs-lookup"><span data-stu-id="e6f70-109">Permissions for app icon in app catalog</span></span>
| <span data-ttu-id="e6f70-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6f70-110">Permission Type</span></span>                        | <span data-ttu-id="e6f70-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6f70-111">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e6f70-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f70-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6f70-113">AppCatalog.Read.All、AppCatalog.ReadWrite.All、AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="e6f70-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="e6f70-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6f70-115">Not supported.</span></span>                                                   |
| <span data-ttu-id="e6f70-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6f70-116">Application</span></span>                            | <span data-ttu-id="e6f70-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6f70-117">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="e6f70-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6f70-118">HTTP request</span></span>

<span data-ttu-id="e6f70-119">**获取应用程序目录中应用程序图标中的托管内容**</span><span class="sxs-lookup"><span data-stu-id="e6f70-119">**Get hosted content in app icon in app catalog**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6f70-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e6f70-120">Optional query parameters</span></span>

<span data-ttu-id="e6f70-121">此操作支持使用 `$select` [OData 查询参数](/graph/query-parameter) 自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6f70-121">This operation supports the `$select` [OData query parameters](/graph/query-parameter) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6f70-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6f70-122">Request headers</span></span>

| <span data-ttu-id="e6f70-123">标头</span><span class="sxs-lookup"><span data-stu-id="e6f70-123">Header</span></span>           | <span data-ttu-id="e6f70-124">值</span><span class="sxs-lookup"><span data-stu-id="e6f70-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="e6f70-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6f70-125">Authorization</span></span>    | <span data-ttu-id="e6f70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6f70-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6f70-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6f70-128">Request body</span></span>

<span data-ttu-id="e6f70-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6f70-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6f70-130">响应</span><span class="sxs-lookup"><span data-stu-id="e6f70-130">Response</span></span>

<span data-ttu-id="e6f70-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamworkHostedContent](../resources/teamworkhostedcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6f70-131">If successful, this method returns a `200 OK` response code and a [teamworkHostedContent](../resources/teamworkhostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6f70-132">示例</span><span class="sxs-lookup"><span data-stu-id="e6f70-132">Examples</span></span>

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="e6f70-133">示例 1：获取目录中应用程序颜色图标Teams内容的字节数</span><span class="sxs-lookup"><span data-stu-id="e6f70-133">Example 1: Get the bytes of the hosted content of the color icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="e6f70-134">请求</span><span class="sxs-lookup"><span data-stu-id="e6f70-134">Request</span></span>

<span data-ttu-id="e6f70-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6f70-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6f70-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f70-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```
# <a name="c"></a>[<span data-ttu-id="e6f70-137">C#</span><span class="sxs-lookup"><span data-stu-id="e6f70-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontent-coloricon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6f70-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6f70-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontent-coloricon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6f70-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6f70-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontent-coloricon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6f70-140">Java</span><span class="sxs-lookup"><span data-stu-id="e6f70-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontent-coloricon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e6f70-141">响应</span><span class="sxs-lookup"><span data-stu-id="e6f70-141">Response</span></span>

<span data-ttu-id="e6f70-142">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="e6f70-142">The following example shows the response.</span></span>

> <span data-ttu-id="e6f70-143">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="e6f70-143">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="e6f70-144">示例 2：获取目录中应用程序大纲图标Teams内容的字节数</span><span class="sxs-lookup"><span data-stu-id="e6f70-144">Example 2: Get the bytes of the hosted content of the outline icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="e6f70-145">请求</span><span class="sxs-lookup"><span data-stu-id="e6f70-145">Request</span></span>

<span data-ttu-id="e6f70-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6f70-146">The following is an example of the request.</span></span>

> <span data-ttu-id="e6f70-147">**注意：** 对原始值的请求不支持 [使用 OData 查询参数](/graph/query-parameters) 自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6f70-147">**Note:** Requests for the raw value does not support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6f70-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f70-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```
# <a name="c"></a>[<span data-ttu-id="e6f70-149">C#</span><span class="sxs-lookup"><span data-stu-id="e6f70-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontentbytes-outlineicon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6f70-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6f70-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontentbytes-outlineicon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6f70-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6f70-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontentbytes-outlineicon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6f70-152">Java</span><span class="sxs-lookup"><span data-stu-id="e6f70-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontentbytes-outlineicon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e6f70-153">响应</span><span class="sxs-lookup"><span data-stu-id="e6f70-153">Response</span></span>

<span data-ttu-id="e6f70-154">响应包含正文中托管内容的字节。</span><span class="sxs-lookup"><span data-stu-id="e6f70-154">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="e6f70-155">`content-type` header 指定托管内容类型。</span><span class="sxs-lookup"><span data-stu-id="e6f70-155">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a><span data-ttu-id="e6f70-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e6f70-156">See also</span></span>

- [<span data-ttu-id="e6f70-157">获取应用Teams图标</span><span class="sxs-lookup"><span data-stu-id="e6f70-157">Get icons of a Teams app</span></span>](teamsappicon-get.md)
- [<span data-ttu-id="e6f70-158">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="e6f70-158">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
