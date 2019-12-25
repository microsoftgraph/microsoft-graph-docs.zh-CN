---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 820f302f45bddce4dd0c594c89f23837b2637313
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864255"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="19173-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="19173-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="19173-105">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="19173-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="19173-106">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="19173-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="19173-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="19173-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="19173-108">权限</span><span class="sxs-lookup"><span data-stu-id="19173-108">Permissions</span></span>

<span data-ttu-id="19173-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19173-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19173-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19173-111">Permission type</span></span>                        | <span data-ttu-id="19173-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19173-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="19173-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19173-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="19173-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19173-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="19173-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19173-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19173-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19173-116">Not supported.</span></span>                           |
| <span data-ttu-id="19173-117">应用</span><span class="sxs-lookup"><span data-stu-id="19173-117">Application</span></span>                            | <span data-ttu-id="19173-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19173-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="19173-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="19173-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="19173-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="19173-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="19173-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19173-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="19173-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="19173-122">Function parameters</span></span>

<span data-ttu-id="19173-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="19173-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="19173-124">参数</span><span class="sxs-lookup"><span data-stu-id="19173-124">Parameter</span></span> | <span data-ttu-id="19173-125">类型</span><span class="sxs-lookup"><span data-stu-id="19173-125">Type</span></span>   | <span data-ttu-id="19173-126">说明</span><span class="sxs-lookup"><span data-stu-id="19173-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="19173-127">period</span><span class="sxs-lookup"><span data-stu-id="19173-127">period</span></span>    | <span data-ttu-id="19173-128">string</span><span class="sxs-lookup"><span data-stu-id="19173-128">string</span></span> | <span data-ttu-id="19173-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="19173-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="19173-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="19173-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="19173-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="19173-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="19173-132">必需。</span><span class="sxs-lookup"><span data-stu-id="19173-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="19173-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="19173-133">Request headers</span></span>

| <span data-ttu-id="19173-134">名称</span><span class="sxs-lookup"><span data-stu-id="19173-134">Name</span></span>          | <span data-ttu-id="19173-135">说明</span><span class="sxs-lookup"><span data-stu-id="19173-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="19173-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="19173-136">Authorization</span></span> | <span data-ttu-id="19173-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="19173-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="19173-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="19173-139">If-None-Match</span></span> | <span data-ttu-id="19173-140">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="19173-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="19173-141">可选。</span><span class="sxs-lookup"><span data-stu-id="19173-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="19173-142">响应</span><span class="sxs-lookup"><span data-stu-id="19173-142">Response</span></span>

<span data-ttu-id="19173-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="19173-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="19173-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="19173-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="19173-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="19173-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="19173-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="19173-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="19173-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="19173-147">Report Refresh Date</span></span>
- <span data-ttu-id="19173-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="19173-148">Report Date</span></span>
- <span data-ttu-id="19173-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="19173-149">Report Period</span></span>
- <span data-ttu-id="19173-150">音频/视频</span><span class="sxs-lookup"><span data-stu-id="19173-150">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="19173-151">示例</span><span class="sxs-lookup"><span data-stu-id="19173-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="19173-152">请求</span><span class="sxs-lookup"><span data-stu-id="19173-152">Request</span></span>

<span data-ttu-id="19173-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19173-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19173-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="19173-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19173-155">C#</span><span class="sxs-lookup"><span data-stu-id="19173-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19173-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19173-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19173-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19173-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19173-158">Java</span><span class="sxs-lookup"><span data-stu-id="19173-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19173-159">响应</span><span class="sxs-lookup"><span data-stu-id="19173-159">Response</span></span>

<span data-ttu-id="19173-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19173-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="19173-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="19173-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
