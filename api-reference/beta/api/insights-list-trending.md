---
title: 列出趋势
description: 计算得出的见解，可返回用户常用的项目列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 83accede4b6af1f1bbc255f94e9e54fb4de4b90f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964633"
---
# <a name="list-trending"></a><span data-ttu-id="7f894-103">列出趋势</span><span class="sxs-lookup"><span data-stu-id="7f894-103">List trending</span></span>

<span data-ttu-id="7f894-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f894-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f894-105">计算的洞察力，包括围绕用户的文档趋势的列表。</span><span class="sxs-lookup"><span data-stu-id="7f894-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f894-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f894-106">Permissions</span></span>
<span data-ttu-id="7f894-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f894-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f894-109">Permission type</span></span>      | <span data-ttu-id="7f894-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f894-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f894-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f894-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f894-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f894-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f894-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f894-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f894-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f894-114">Not supported.</span></span>    |
|<span data-ttu-id="7f894-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f894-115">Application</span></span> | <span data-ttu-id="7f894-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f894-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f894-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f894-117">HTTP request</span></span>
<span data-ttu-id="7f894-118">获取围绕登录用户或指定用户的文档趋势的列表：</span><span class="sxs-lookup"><span data-stu-id="7f894-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="7f894-119">扩展 **趋势** 洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="7f894-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f894-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f894-120">Optional query parameters</span></span>
<span data-ttu-id="7f894-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f894-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="7f894-122">您可以使用 `$filter` 查询参数筛选趋势项。</span><span class="sxs-lookup"><span data-stu-id="7f894-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="7f894-123">例如，基于 **类型** ：</span><span class="sxs-lookup"><span data-stu-id="7f894-123">For example, based on **type** :</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="7f894-124">或基于 **containerType** ：</span><span class="sxs-lookup"><span data-stu-id="7f894-124">Or based on **containerType** :</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="7f894-125">请参阅可在 [resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="7f894-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="7f894-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f894-126">Request headers</span></span>
| <span data-ttu-id="7f894-127">标头</span><span class="sxs-lookup"><span data-stu-id="7f894-127">Header</span></span>       |  <span data-ttu-id="7f894-128">值</span><span class="sxs-lookup"><span data-stu-id="7f894-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="7f894-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f894-129">Authorization</span></span>  | <span data-ttu-id="7f894-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f894-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="7f894-132">接受</span><span class="sxs-lookup"><span data-stu-id="7f894-132">Accept</span></span>  | <span data-ttu-id="7f894-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7f894-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f894-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f894-134">Request body</span></span>
<span data-ttu-id="7f894-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f894-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f894-136">响应</span><span class="sxs-lookup"><span data-stu-id="7f894-136">Response</span></span>

<span data-ttu-id="7f894-137">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [趋势](../resources/insights-trending.md) 项列表。</span><span class="sxs-lookup"><span data-stu-id="7f894-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="7f894-138">每个项目都包含可视化属性，用于显示您的体验中的项目。</span><span class="sxs-lookup"><span data-stu-id="7f894-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="7f894-139">如果已禁用目标用户的项目见解，则此方法将返回， `403 Forbidden` 并出现以下错误：</span><span class="sxs-lookup"><span data-stu-id="7f894-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
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
<span data-ttu-id="7f894-140">有关详细信息，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy.md)。</span><span class="sxs-lookup"><span data-stu-id="7f894-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="7f894-141">示例</span><span class="sxs-lookup"><span data-stu-id="7f894-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f894-142">请求</span><span class="sxs-lookup"><span data-stu-id="7f894-142">Request</span></span>
<span data-ttu-id="7f894-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f894-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f894-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f894-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="7f894-145">C#</span><span class="sxs-lookup"><span data-stu-id="7f894-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f894-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f894-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f894-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f894-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f894-148">Java</span><span class="sxs-lookup"><span data-stu-id="7f894-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-trending-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7f894-149">响应</span><span class="sxs-lookup"><span data-stu-id="7f894-149">Response</span></span>
<span data-ttu-id="7f894-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7f894-150">Here is an example of the response.</span></span> <span data-ttu-id="7f894-151">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7f894-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7f894-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f894-152">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="7f894-153">请参阅页面底部的 "未截断的示例" 响应。</span><span class="sxs-lookup"><span data-stu-id="7f894-153">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```
