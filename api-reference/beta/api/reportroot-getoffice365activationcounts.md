---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 080a5bf3694d5134338b4eb321eb38eaf00785bc
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639451"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="6a32d-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="6a32d-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a32d-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="6a32d-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="6a32d-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="6a32d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a32d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6a32d-106">Permissions</span></span>

<span data-ttu-id="6a32d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a32d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a32d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a32d-109">Permission type</span></span>                        | <span data-ttu-id="6a32d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a32d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6a32d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a32d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a32d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a32d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6a32d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a32d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a32d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a32d-114">Not supported.</span></span>                           |
| <span data-ttu-id="6a32d-115">应用</span><span class="sxs-lookup"><span data-stu-id="6a32d-115">Application</span></span>                            | <span data-ttu-id="6a32d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a32d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6a32d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a32d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="6a32d-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="6a32d-118">Query parameters</span></span>

<span data-ttu-id="6a32d-119">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6a32d-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6a32d-120">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="6a32d-120">The default output type is text/csv.</span></span> <span data-ttu-id="6a32d-121">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="6a32d-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a32d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a32d-122">Request headers</span></span>

| <span data-ttu-id="6a32d-123">名称</span><span class="sxs-lookup"><span data-stu-id="6a32d-123">Name</span></span>          | <span data-ttu-id="6a32d-124">说明</span><span class="sxs-lookup"><span data-stu-id="6a32d-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6a32d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a32d-125">Authorization</span></span> | <span data-ttu-id="6a32d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a32d-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6a32d-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a32d-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6a32d-129">CSV</span><span class="sxs-lookup"><span data-stu-id="6a32d-129">CSV</span></span>

<span data-ttu-id="6a32d-130">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6a32d-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6a32d-131">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6a32d-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6a32d-132">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6a32d-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6a32d-133">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6a32d-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6a32d-134">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6a32d-134">Report Refresh Date</span></span>
- <span data-ttu-id="6a32d-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="6a32d-135">Product Type</span></span>
- <span data-ttu-id="6a32d-136">Windows</span><span class="sxs-lookup"><span data-stu-id="6a32d-136">Windows</span></span>
- <span data-ttu-id="6a32d-137">Mac</span><span class="sxs-lookup"><span data-stu-id="6a32d-137">Mac</span></span>
- <span data-ttu-id="6a32d-138">Android</span><span class="sxs-lookup"><span data-stu-id="6a32d-138">Android</span></span>
- <span data-ttu-id="6a32d-139">iOS</span><span class="sxs-lookup"><span data-stu-id="6a32d-139">iOS</span></span>
- <span data-ttu-id="6a32d-140">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="6a32d-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="6a32d-141">JSON</span><span class="sxs-lookup"><span data-stu-id="6a32d-141">JSON</span></span>

<span data-ttu-id="6a32d-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6a32d-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a32d-143">示例</span><span class="sxs-lookup"><span data-stu-id="6a32d-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6a32d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="6a32d-144">CSV</span></span>

<span data-ttu-id="6a32d-145">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="6a32d-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6a32d-146">请求</span><span class="sxs-lookup"><span data-stu-id="6a32d-146">Request</span></span>

<span data-ttu-id="6a32d-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6a32d-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6a32d-148">响应</span><span class="sxs-lookup"><span data-stu-id="6a32d-148">Response</span></span>

<span data-ttu-id="6a32d-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a32d-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a32d-150">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6a32d-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a32d-151">语言</span><span class="sxs-lookup"><span data-stu-id="6a32d-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a32d-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a32d-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6a32d-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6a32d-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="6a32d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="6a32d-154">JSON</span></span>

<span data-ttu-id="6a32d-155">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6a32d-155">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6a32d-156">请求</span><span class="sxs-lookup"><span data-stu-id="6a32d-156">Request</span></span>

<span data-ttu-id="6a32d-157">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a32d-157">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6a32d-158">响应</span><span class="sxs-lookup"><span data-stu-id="6a32d-158">Response</span></span>

<span data-ttu-id="6a32d-159">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="6a32d-159">The following example shows the response.</span></span>

> <span data-ttu-id="6a32d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6a32d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a32d-162">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6a32d-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a32d-163">语言</span><span class="sxs-lookup"><span data-stu-id="6a32d-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a32d-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a32d-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
