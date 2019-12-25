---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fbd35e1eddae4b6d3a492cfcdc2a207e487e0531
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865293"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="051eb-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="051eb-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="051eb-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="051eb-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="051eb-106">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="051eb-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="051eb-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="051eb-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="051eb-108">权限</span><span class="sxs-lookup"><span data-stu-id="051eb-108">Permissions</span></span>

<span data-ttu-id="051eb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="051eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="051eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="051eb-111">Permission type</span></span>                        | <span data-ttu-id="051eb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="051eb-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="051eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="051eb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="051eb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="051eb-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="051eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="051eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="051eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="051eb-116">Not supported.</span></span>                           |
| <span data-ttu-id="051eb-117">应用</span><span class="sxs-lookup"><span data-stu-id="051eb-117">Application</span></span>                            | <span data-ttu-id="051eb-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="051eb-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="051eb-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="051eb-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="051eb-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="051eb-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="051eb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="051eb-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="051eb-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="051eb-122">Function parameters</span></span>

<span data-ttu-id="051eb-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="051eb-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="051eb-124">参数</span><span class="sxs-lookup"><span data-stu-id="051eb-124">Parameter</span></span> | <span data-ttu-id="051eb-125">类型</span><span class="sxs-lookup"><span data-stu-id="051eb-125">Type</span></span>   | <span data-ttu-id="051eb-126">说明</span><span class="sxs-lookup"><span data-stu-id="051eb-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="051eb-127">period</span><span class="sxs-lookup"><span data-stu-id="051eb-127">period</span></span>    | <span data-ttu-id="051eb-128">string</span><span class="sxs-lookup"><span data-stu-id="051eb-128">string</span></span> | <span data-ttu-id="051eb-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="051eb-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="051eb-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="051eb-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="051eb-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="051eb-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="051eb-132">必需。</span><span class="sxs-lookup"><span data-stu-id="051eb-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="051eb-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="051eb-133">Request headers</span></span>

| <span data-ttu-id="051eb-134">名称</span><span class="sxs-lookup"><span data-stu-id="051eb-134">Name</span></span>          | <span data-ttu-id="051eb-135">说明</span><span class="sxs-lookup"><span data-stu-id="051eb-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="051eb-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="051eb-136">Authorization</span></span> | <span data-ttu-id="051eb-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="051eb-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="051eb-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="051eb-139">If-None-Match</span></span> | <span data-ttu-id="051eb-140">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="051eb-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="051eb-141">可选。</span><span class="sxs-lookup"><span data-stu-id="051eb-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="051eb-142">响应</span><span class="sxs-lookup"><span data-stu-id="051eb-142">Response</span></span>

<span data-ttu-id="051eb-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="051eb-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="051eb-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="051eb-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="051eb-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="051eb-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="051eb-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="051eb-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="051eb-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="051eb-147">Report Refresh Date</span></span>
- <span data-ttu-id="051eb-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="051eb-148">Report Date</span></span>
- <span data-ttu-id="051eb-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="051eb-149">Report Period</span></span>
- <span data-ttu-id="051eb-150">IM</span><span class="sxs-lookup"><span data-stu-id="051eb-150">IM</span></span>
- <span data-ttu-id="051eb-151">音频/视频</span><span class="sxs-lookup"><span data-stu-id="051eb-151">Audio/Video</span></span>
- <span data-ttu-id="051eb-152">应用共享</span><span class="sxs-lookup"><span data-stu-id="051eb-152">App Sharing</span></span>
- <span data-ttu-id="051eb-153">Web</span><span class="sxs-lookup"><span data-stu-id="051eb-153">Web</span></span>
- <span data-ttu-id="051eb-154">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="051eb-154">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="051eb-155">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="051eb-155">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="051eb-156">示例</span><span class="sxs-lookup"><span data-stu-id="051eb-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="051eb-157">请求</span><span class="sxs-lookup"><span data-stu-id="051eb-157">Request</span></span>

<span data-ttu-id="051eb-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="051eb-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="051eb-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="051eb-159">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="051eb-160">C#</span><span class="sxs-lookup"><span data-stu-id="051eb-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="051eb-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="051eb-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="051eb-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="051eb-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="051eb-163">Java</span><span class="sxs-lookup"><span data-stu-id="051eb-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="051eb-164">响应</span><span class="sxs-lookup"><span data-stu-id="051eb-164">Response</span></span>

<span data-ttu-id="051eb-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="051eb-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="051eb-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="051eb-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
