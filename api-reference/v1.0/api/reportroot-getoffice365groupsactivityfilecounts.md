---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: 获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2560472cec0d26099875c9e9950a5bfcf86e1159
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728158"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="20aa8-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="20aa8-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="20aa8-104">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="20aa8-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="20aa8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="20aa8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="20aa8-106">权限</span><span class="sxs-lookup"><span data-stu-id="20aa8-106">Permissions</span></span>

<span data-ttu-id="20aa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20aa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20aa8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20aa8-109">Permission type</span></span>                        | <span data-ttu-id="20aa8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20aa8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="20aa8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20aa8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20aa8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="20aa8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="20aa8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20aa8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20aa8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20aa8-114">Not supported.</span></span>                           |
| <span data-ttu-id="20aa8-115">应用</span><span class="sxs-lookup"><span data-stu-id="20aa8-115">Application</span></span>                            | <span data-ttu-id="20aa8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="20aa8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="20aa8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20aa8-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="20aa8-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="20aa8-118">Function parameters</span></span>

<span data-ttu-id="20aa8-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="20aa8-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="20aa8-120">参数</span><span class="sxs-lookup"><span data-stu-id="20aa8-120">Parameter</span></span> | <span data-ttu-id="20aa8-121">类型</span><span class="sxs-lookup"><span data-stu-id="20aa8-121">Type</span></span>   | <span data-ttu-id="20aa8-122">说明</span><span class="sxs-lookup"><span data-stu-id="20aa8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="20aa8-123">period</span><span class="sxs-lookup"><span data-stu-id="20aa8-123">period</span></span>    | <span data-ttu-id="20aa8-124">string</span><span class="sxs-lookup"><span data-stu-id="20aa8-124">string</span></span> | <span data-ttu-id="20aa8-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="20aa8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="20aa8-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="20aa8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="20aa8-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="20aa8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="20aa8-128">必需。</span><span class="sxs-lookup"><span data-stu-id="20aa8-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="20aa8-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="20aa8-129">Request headers</span></span>

| <span data-ttu-id="20aa8-130">名称</span><span class="sxs-lookup"><span data-stu-id="20aa8-130">Name</span></span>          | <span data-ttu-id="20aa8-131">说明</span><span class="sxs-lookup"><span data-stu-id="20aa8-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="20aa8-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="20aa8-132">Authorization</span></span> | <span data-ttu-id="20aa8-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="20aa8-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="20aa8-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="20aa8-135">If-None-Match</span></span> | <span data-ttu-id="20aa8-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="20aa8-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="20aa8-137">可选。</span><span class="sxs-lookup"><span data-stu-id="20aa8-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="20aa8-138">响应</span><span class="sxs-lookup"><span data-stu-id="20aa8-138">Response</span></span>

<span data-ttu-id="20aa8-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="20aa8-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="20aa8-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="20aa8-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="20aa8-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="20aa8-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="20aa8-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="20aa8-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="20aa8-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="20aa8-143">Report Refresh Date</span></span>
- <span data-ttu-id="20aa8-144">总计</span><span class="sxs-lookup"><span data-stu-id="20aa8-144">Total</span></span>
- <span data-ttu-id="20aa8-145">活跃</span><span class="sxs-lookup"><span data-stu-id="20aa8-145">Active</span></span>
- <span data-ttu-id="20aa8-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="20aa8-146">Report Date</span></span>
- <span data-ttu-id="20aa8-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="20aa8-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="20aa8-148">示例</span><span class="sxs-lookup"><span data-stu-id="20aa8-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="20aa8-149">请求</span><span class="sxs-lookup"><span data-stu-id="20aa8-149">Request</span></span>

<span data-ttu-id="20aa8-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20aa8-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="20aa8-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="20aa8-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20aa8-152">C#</span><span class="sxs-lookup"><span data-stu-id="20aa8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20aa8-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20aa8-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20aa8-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="20aa8-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="20aa8-155">Java</span><span class="sxs-lookup"><span data-stu-id="20aa8-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="20aa8-156">响应</span><span class="sxs-lookup"><span data-stu-id="20aa8-156">Response</span></span>

<span data-ttu-id="20aa8-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="20aa8-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="20aa8-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="20aa8-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
