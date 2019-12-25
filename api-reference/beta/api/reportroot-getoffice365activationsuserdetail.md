---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bdab2bdfe628f8a1b9bffef59806969ad1d6c03a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869162"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="72b61-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="72b61-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b61-104">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="72b61-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="72b61-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="72b61-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="72b61-106">权限</span><span class="sxs-lookup"><span data-stu-id="72b61-106">Permissions</span></span>

<span data-ttu-id="72b61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72b61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72b61-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72b61-109">Permission type</span></span>                        | <span data-ttu-id="72b61-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72b61-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="72b61-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72b61-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72b61-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72b61-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="72b61-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72b61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b61-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72b61-114">Not supported.</span></span>                           |
| <span data-ttu-id="72b61-115">应用</span><span class="sxs-lookup"><span data-stu-id="72b61-115">Application</span></span>                            | <span data-ttu-id="72b61-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72b61-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="72b61-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="72b61-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="72b61-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="72b61-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="72b61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72b61-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="72b61-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="72b61-120">Query parameters</span></span>

<span data-ttu-id="72b61-121">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72b61-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="72b61-122">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="72b61-122">The default output type is text/csv.</span></span> <span data-ttu-id="72b61-123">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="72b61-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72b61-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="72b61-124">Request headers</span></span>

| <span data-ttu-id="72b61-125">名称</span><span class="sxs-lookup"><span data-stu-id="72b61-125">Name</span></span>          | <span data-ttu-id="72b61-126">说明</span><span class="sxs-lookup"><span data-stu-id="72b61-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="72b61-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="72b61-127">Authorization</span></span> | <span data-ttu-id="72b61-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72b61-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="72b61-130">响应</span><span class="sxs-lookup"><span data-stu-id="72b61-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="72b61-131">CSV</span><span class="sxs-lookup"><span data-stu-id="72b61-131">CSV</span></span>

<span data-ttu-id="72b61-132">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="72b61-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="72b61-133">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="72b61-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="72b61-134">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="72b61-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="72b61-135">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="72b61-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="72b61-136">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="72b61-136">Report Refresh Date</span></span>
- <span data-ttu-id="72b61-137">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="72b61-137">User Principal Name</span></span>
- <span data-ttu-id="72b61-138">显示名称</span><span class="sxs-lookup"><span data-stu-id="72b61-138">Display Name</span></span>
- <span data-ttu-id="72b61-139">产品类型</span><span class="sxs-lookup"><span data-stu-id="72b61-139">Product Type</span></span>
- <span data-ttu-id="72b61-140">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="72b61-140">Last Activated Date</span></span>
- <span data-ttu-id="72b61-141">Windows</span><span class="sxs-lookup"><span data-stu-id="72b61-141">Windows</span></span>
- <span data-ttu-id="72b61-142">Mac</span><span class="sxs-lookup"><span data-stu-id="72b61-142">Mac</span></span>
- <span data-ttu-id="72b61-143">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="72b61-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="72b61-144">iOS</span><span class="sxs-lookup"><span data-stu-id="72b61-144">iOS</span></span>
- <span data-ttu-id="72b61-145">Android</span><span class="sxs-lookup"><span data-stu-id="72b61-145">Android</span></span>
- <span data-ttu-id="72b61-146">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="72b61-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="72b61-147">JSON</span><span class="sxs-lookup"><span data-stu-id="72b61-147">JSON</span></span>

<span data-ttu-id="72b61-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="72b61-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="72b61-149">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="72b61-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="72b61-150">示例</span><span class="sxs-lookup"><span data-stu-id="72b61-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="72b61-151">CSV</span><span class="sxs-lookup"><span data-stu-id="72b61-151">CSV</span></span>

<span data-ttu-id="72b61-152">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="72b61-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="72b61-153">请求</span><span class="sxs-lookup"><span data-stu-id="72b61-153">Request</span></span>

<span data-ttu-id="72b61-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72b61-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72b61-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="72b61-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72b61-156">C#</span><span class="sxs-lookup"><span data-stu-id="72b61-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72b61-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72b61-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72b61-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72b61-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72b61-159">响应</span><span class="sxs-lookup"><span data-stu-id="72b61-159">Response</span></span>

<span data-ttu-id="72b61-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72b61-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="72b61-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="72b61-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="72b61-162">JSON</span><span class="sxs-lookup"><span data-stu-id="72b61-162">JSON</span></span>

<span data-ttu-id="72b61-163">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="72b61-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="72b61-164">请求</span><span class="sxs-lookup"><span data-stu-id="72b61-164">Request</span></span>

<span data-ttu-id="72b61-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72b61-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72b61-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="72b61-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72b61-167">C#</span><span class="sxs-lookup"><span data-stu-id="72b61-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72b61-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72b61-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72b61-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72b61-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72b61-170">响应</span><span class="sxs-lookup"><span data-stu-id="72b61-170">Response</span></span>

<span data-ttu-id="72b61-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="72b61-171">The following is an example of the response.</span></span>

> <span data-ttu-id="72b61-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72b61-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
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
