---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6c85ddecb5b40e103c7c5e0638f7879ac5595a9d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727962"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="baf8d-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="baf8d-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="baf8d-105">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="baf8d-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="baf8d-106">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="baf8d-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="baf8d-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="baf8d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="baf8d-108">权限</span><span class="sxs-lookup"><span data-stu-id="baf8d-108">Permissions</span></span>

<span data-ttu-id="baf8d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baf8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="baf8d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="baf8d-111">Permission type</span></span>                        | <span data-ttu-id="baf8d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baf8d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="baf8d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baf8d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="baf8d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baf8d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="baf8d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baf8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="baf8d-116">Not supported.</span></span>                           |
| <span data-ttu-id="baf8d-117">应用</span><span class="sxs-lookup"><span data-stu-id="baf8d-117">Application</span></span>                            | <span data-ttu-id="baf8d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baf8d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="baf8d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baf8d-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="baf8d-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="baf8d-120">Function parameters</span></span>

<span data-ttu-id="baf8d-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="baf8d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="baf8d-122">参数</span><span class="sxs-lookup"><span data-stu-id="baf8d-122">Parameter</span></span> | <span data-ttu-id="baf8d-123">类型</span><span class="sxs-lookup"><span data-stu-id="baf8d-123">Type</span></span>   | <span data-ttu-id="baf8d-124">说明</span><span class="sxs-lookup"><span data-stu-id="baf8d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="baf8d-125">period</span><span class="sxs-lookup"><span data-stu-id="baf8d-125">period</span></span>    | <span data-ttu-id="baf8d-126">string</span><span class="sxs-lookup"><span data-stu-id="baf8d-126">string</span></span> | <span data-ttu-id="baf8d-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="baf8d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="baf8d-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="baf8d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="baf8d-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="baf8d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="baf8d-130">必需。</span><span class="sxs-lookup"><span data-stu-id="baf8d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="baf8d-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="baf8d-131">Request headers</span></span>

| <span data-ttu-id="baf8d-132">名称</span><span class="sxs-lookup"><span data-stu-id="baf8d-132">Name</span></span>          | <span data-ttu-id="baf8d-133">说明</span><span class="sxs-lookup"><span data-stu-id="baf8d-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="baf8d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="baf8d-134">Authorization</span></span> | <span data-ttu-id="baf8d-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="baf8d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="baf8d-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="baf8d-137">If-None-Match</span></span> | <span data-ttu-id="baf8d-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="baf8d-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="baf8d-139">可选。</span><span class="sxs-lookup"><span data-stu-id="baf8d-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="baf8d-140">响应</span><span class="sxs-lookup"><span data-stu-id="baf8d-140">Response</span></span>

<span data-ttu-id="baf8d-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="baf8d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="baf8d-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="baf8d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="baf8d-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="baf8d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="baf8d-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="baf8d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="baf8d-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="baf8d-145">Report Refresh Date</span></span>
- <span data-ttu-id="baf8d-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="baf8d-146">Report Date</span></span>
- <span data-ttu-id="baf8d-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="baf8d-147">Report Period</span></span>
- <span data-ttu-id="baf8d-148">音频/视频</span><span class="sxs-lookup"><span data-stu-id="baf8d-148">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="baf8d-149">示例</span><span class="sxs-lookup"><span data-stu-id="baf8d-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="baf8d-150">请求</span><span class="sxs-lookup"><span data-stu-id="baf8d-150">Request</span></span>

<span data-ttu-id="baf8d-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="baf8d-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="baf8d-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="baf8d-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="baf8d-153">C#</span><span class="sxs-lookup"><span data-stu-id="baf8d-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baf8d-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="baf8d-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baf8d-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="baf8d-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="baf8d-156">Java</span><span class="sxs-lookup"><span data-stu-id="baf8d-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="baf8d-157">响应</span><span class="sxs-lookup"><span data-stu-id="baf8d-157">Response</span></span>

<span data-ttu-id="baf8d-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="baf8d-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="baf8d-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="baf8d-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
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
