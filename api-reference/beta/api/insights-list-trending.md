---
title: 列出趋势
description: 计算得出的见解，可返回用户常用的项目列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5a790c23a0e3cee09079beb5b51151610f309dad
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040243"
---
# <a name="list-trending"></a><span data-ttu-id="c1389-103">列出趋势</span><span class="sxs-lookup"><span data-stu-id="c1389-103">List trending</span></span>

<span data-ttu-id="c1389-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1389-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1389-105">计算得出的见解，其中包括围绕用户趋势的文档列表。</span><span class="sxs-lookup"><span data-stu-id="c1389-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1389-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1389-106">Permissions</span></span>
<span data-ttu-id="c1389-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c1389-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1389-109">Permission type</span></span>      | <span data-ttu-id="c1389-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1389-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1389-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1389-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1389-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1389-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1389-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1389-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1389-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1389-114">Not supported.</span></span>    |
|<span data-ttu-id="c1389-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1389-115">Application</span></span> | <span data-ttu-id="c1389-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1389-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1389-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1389-117">HTTP request</span></span>
<span data-ttu-id="c1389-118">获取登录用户或指定用户周围的文档列表：</span><span class="sxs-lookup"><span data-stu-id="c1389-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="c1389-119">展开趋势见解 **所引用的资源** ：</span><span class="sxs-lookup"><span data-stu-id="c1389-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1389-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1389-120">Optional query parameters</span></span>
<span data-ttu-id="c1389-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1389-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="c1389-122">可以使用查询 `$filter` 参数筛选趋势项目。</span><span class="sxs-lookup"><span data-stu-id="c1389-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="c1389-123">例如，根据 **类型**：</span><span class="sxs-lookup"><span data-stu-id="c1389-123">For example, based on **type**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="c1389-124">或基于 **containerType：**</span><span class="sxs-lookup"><span data-stu-id="c1389-124">Or based on **containerType**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="c1389-125">请参阅 [resourceVisualization](../resources/insights-resourcevisualization.md)中可以按筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="c1389-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="c1389-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1389-126">Request headers</span></span>
| <span data-ttu-id="c1389-127">标头</span><span class="sxs-lookup"><span data-stu-id="c1389-127">Header</span></span>       |  <span data-ttu-id="c1389-128">值</span><span class="sxs-lookup"><span data-stu-id="c1389-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="c1389-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1389-129">Authorization</span></span>  | <span data-ttu-id="c1389-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1389-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c1389-132">接受</span><span class="sxs-lookup"><span data-stu-id="c1389-132">Accept</span></span>  | <span data-ttu-id="c1389-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c1389-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1389-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1389-134">Request body</span></span>
<span data-ttu-id="c1389-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1389-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1389-136">响应</span><span class="sxs-lookup"><span data-stu-id="c1389-136">Response</span></span>

<span data-ttu-id="c1389-137">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/insights-trending.md)趋势项列表。</span><span class="sxs-lookup"><span data-stu-id="c1389-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="c1389-138">每个项目都包含用于在你的体验中显示该项目的可视化属性。</span><span class="sxs-lookup"><span data-stu-id="c1389-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="c1389-139">如果已禁用目标用户的项目见解，此方法将返回 `403 Forbidden` 并出现以下错误：</span><span class="sxs-lookup"><span data-stu-id="c1389-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
<!-- { "blockType": "ignored" } -->

```
{
  "error": {
    "code": "ItemInsightsDisabled",
    "message": " The access to the requested resource is denied because item insights are disabled.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```
<span data-ttu-id="c1389-140">有关详细信息，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy.md)。</span><span class="sxs-lookup"><span data-stu-id="c1389-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="c1389-141">示例</span><span class="sxs-lookup"><span data-stu-id="c1389-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c1389-142">请求</span><span class="sxs-lookup"><span data-stu-id="c1389-142">Request</span></span>
<span data-ttu-id="c1389-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1389-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1389-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1389-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="c1389-145">C#</span><span class="sxs-lookup"><span data-stu-id="c1389-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1389-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1389-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1389-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1389-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1389-148">Java</span><span class="sxs-lookup"><span data-stu-id="c1389-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-trending-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c1389-149">响应</span><span class="sxs-lookup"><span data-stu-id="c1389-149">Response</span></span>
<span data-ttu-id="c1389-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1389-150">Here is an example of the response.</span></span> <span data-ttu-id="c1389-151">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1389-151">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1389-152">请参阅页面底部的未截断响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1389-152">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AWMiSOpKHlJCpP_ZoVJQXi9ees4wFhDQQqF55Pm5DlaMzvtd2zra4UWSTEvpTldvb6EhQ289G4BAsxnrajQyjW1jIkjqSh5SQqT_2aFSUF4vBQ",
      "weight": "0.1583399742569597",
      "resourceVisualization": {
        "title": "LiveCaptions",
        "type": "Image",
        "mediaType": "application/octet-stream",
        "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN/thumbnails/0/small/thumbnailContent",
        "previewText": "",
        "containerWebUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared Documents/Go to Market Plan",
        "containerDisplayName": "Mark 8 Project Team",
        "containerType": "Site"
      },
      "resourceReference": {
        "webUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared%20Documents/Go%20to%20Market%20Plan/LiveCaptions.gif",
        "id": "drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN",
        "type": "microsoft.graph.driveItem"
      }
    }
  ]
}
```
