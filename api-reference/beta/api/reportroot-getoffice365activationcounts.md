---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f71a38c9c3d2264a0414bf03041d7a9132bfccb9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869149"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="22f31-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="22f31-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22f31-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="22f31-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="22f31-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="22f31-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="22f31-106">权限</span><span class="sxs-lookup"><span data-stu-id="22f31-106">Permissions</span></span>

<span data-ttu-id="22f31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22f31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22f31-109">Permission type</span></span>                        | <span data-ttu-id="22f31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22f31-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="22f31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22f31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22f31-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f31-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="22f31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22f31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22f31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22f31-114">Not supported.</span></span>                           |
| <span data-ttu-id="22f31-115">应用</span><span class="sxs-lookup"><span data-stu-id="22f31-115">Application</span></span>                            | <span data-ttu-id="22f31-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f31-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="22f31-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="22f31-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="22f31-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="22f31-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="22f31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22f31-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="22f31-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="22f31-120">Query parameters</span></span>

<span data-ttu-id="22f31-121">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22f31-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="22f31-122">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="22f31-122">The default output type is text/csv.</span></span> <span data-ttu-id="22f31-123">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="22f31-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22f31-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="22f31-124">Request headers</span></span>

| <span data-ttu-id="22f31-125">名称</span><span class="sxs-lookup"><span data-stu-id="22f31-125">Name</span></span>          | <span data-ttu-id="22f31-126">说明</span><span class="sxs-lookup"><span data-stu-id="22f31-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="22f31-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f31-127">Authorization</span></span> | <span data-ttu-id="22f31-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22f31-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="22f31-130">响应</span><span class="sxs-lookup"><span data-stu-id="22f31-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="22f31-131">CSV</span><span class="sxs-lookup"><span data-stu-id="22f31-131">CSV</span></span>

<span data-ttu-id="22f31-132">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="22f31-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="22f31-133">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="22f31-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="22f31-134">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="22f31-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="22f31-135">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="22f31-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="22f31-136">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="22f31-136">Report Refresh Date</span></span>
- <span data-ttu-id="22f31-137">产品类型</span><span class="sxs-lookup"><span data-stu-id="22f31-137">Product Type</span></span>
- <span data-ttu-id="22f31-138">Windows</span><span class="sxs-lookup"><span data-stu-id="22f31-138">Windows</span></span>
- <span data-ttu-id="22f31-139">Mac</span><span class="sxs-lookup"><span data-stu-id="22f31-139">Mac</span></span>
- <span data-ttu-id="22f31-140">Android</span><span class="sxs-lookup"><span data-stu-id="22f31-140">Android</span></span>
- <span data-ttu-id="22f31-141">iOS</span><span class="sxs-lookup"><span data-stu-id="22f31-141">iOS</span></span>
- <span data-ttu-id="22f31-142">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="22f31-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="22f31-143">JSON</span><span class="sxs-lookup"><span data-stu-id="22f31-143">JSON</span></span>

<span data-ttu-id="22f31-144">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="22f31-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f31-145">示例</span><span class="sxs-lookup"><span data-stu-id="22f31-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="22f31-146">CSV</span><span class="sxs-lookup"><span data-stu-id="22f31-146">CSV</span></span>

<span data-ttu-id="22f31-147">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="22f31-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="22f31-148">请求</span><span class="sxs-lookup"><span data-stu-id="22f31-148">Request</span></span>

<span data-ttu-id="22f31-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22f31-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="22f31-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="22f31-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22f31-151">C#</span><span class="sxs-lookup"><span data-stu-id="22f31-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22f31-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22f31-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22f31-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22f31-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22f31-154">响应</span><span class="sxs-lookup"><span data-stu-id="22f31-154">Response</span></span>

<span data-ttu-id="22f31-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22f31-155">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="22f31-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="22f31-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="22f31-157">JSON</span><span class="sxs-lookup"><span data-stu-id="22f31-157">JSON</span></span>

<span data-ttu-id="22f31-158">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="22f31-158">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="22f31-159">请求</span><span class="sxs-lookup"><span data-stu-id="22f31-159">Request</span></span>

<span data-ttu-id="22f31-160">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="22f31-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="22f31-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="22f31-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22f31-162">C#</span><span class="sxs-lookup"><span data-stu-id="22f31-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22f31-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22f31-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22f31-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22f31-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22f31-165">响应</span><span class="sxs-lookup"><span data-stu-id="22f31-165">Response</span></span>

<span data-ttu-id="22f31-166">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="22f31-166">The following example shows the response.</span></span>

> <span data-ttu-id="22f31-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22f31-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
