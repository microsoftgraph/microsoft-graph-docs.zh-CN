---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 032fdde812a8fa0f4ae2725184c4f1254841a096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510114"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="2a44c-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="2a44c-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="2a44c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a44c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a44c-106">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="2a44c-106">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="2a44c-107">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="2a44c-107">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="2a44c-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="2a44c-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a44c-109">权限</span><span class="sxs-lookup"><span data-stu-id="2a44c-109">Permissions</span></span>

<span data-ttu-id="2a44c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a44c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a44c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a44c-112">Permission type</span></span>                        | <span data-ttu-id="2a44c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a44c-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2a44c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a44c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a44c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a44c-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2a44c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a44c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a44c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a44c-117">Not supported.</span></span>                           |
| <span data-ttu-id="2a44c-118">应用</span><span class="sxs-lookup"><span data-stu-id="2a44c-118">Application</span></span>                            | <span data-ttu-id="2a44c-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a44c-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="2a44c-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="2a44c-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2a44c-121">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="2a44c-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2a44c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a44c-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2a44c-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="2a44c-123">Function parameters</span></span>

<span data-ttu-id="2a44c-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2a44c-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2a44c-125">参数</span><span class="sxs-lookup"><span data-stu-id="2a44c-125">Parameter</span></span> | <span data-ttu-id="2a44c-126">类型</span><span class="sxs-lookup"><span data-stu-id="2a44c-126">Type</span></span>   | <span data-ttu-id="2a44c-127">说明</span><span class="sxs-lookup"><span data-stu-id="2a44c-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2a44c-128">period</span><span class="sxs-lookup"><span data-stu-id="2a44c-128">period</span></span>    | <span data-ttu-id="2a44c-129">string</span><span class="sxs-lookup"><span data-stu-id="2a44c-129">string</span></span> | <span data-ttu-id="2a44c-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2a44c-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2a44c-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2a44c-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2a44c-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2a44c-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2a44c-133">必需。</span><span class="sxs-lookup"><span data-stu-id="2a44c-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2a44c-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a44c-134">Request headers</span></span>

| <span data-ttu-id="2a44c-135">名称</span><span class="sxs-lookup"><span data-stu-id="2a44c-135">Name</span></span>          | <span data-ttu-id="2a44c-136">说明</span><span class="sxs-lookup"><span data-stu-id="2a44c-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2a44c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a44c-137">Authorization</span></span> | <span data-ttu-id="2a44c-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a44c-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2a44c-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2a44c-140">If-None-Match</span></span> | <span data-ttu-id="2a44c-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a44c-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2a44c-142">可选。</span><span class="sxs-lookup"><span data-stu-id="2a44c-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2a44c-143">响应</span><span class="sxs-lookup"><span data-stu-id="2a44c-143">Response</span></span>

<span data-ttu-id="2a44c-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2a44c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2a44c-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2a44c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2a44c-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2a44c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2a44c-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2a44c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2a44c-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2a44c-148">Report Refresh Date</span></span>
- <span data-ttu-id="2a44c-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="2a44c-149">Report Date</span></span>
- <span data-ttu-id="2a44c-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="2a44c-150">Report Period</span></span>
- <span data-ttu-id="2a44c-151">音频/视频</span><span class="sxs-lookup"><span data-stu-id="2a44c-151">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="2a44c-152">示例</span><span class="sxs-lookup"><span data-stu-id="2a44c-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2a44c-153">请求</span><span class="sxs-lookup"><span data-stu-id="2a44c-153">Request</span></span>

<span data-ttu-id="2a44c-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a44c-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a44c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a44c-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="2a44c-156">C#</span><span class="sxs-lookup"><span data-stu-id="2a44c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a44c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a44c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a44c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a44c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a44c-159">Java</span><span class="sxs-lookup"><span data-stu-id="2a44c-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a44c-160">响应</span><span class="sxs-lookup"><span data-stu-id="2a44c-160">Response</span></span>

<span data-ttu-id="2a44c-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a44c-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="2a44c-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2a44c-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
