---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
ms.openlocfilehash: f62215296e59212aaf9dfef975f08534d2f56c64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008932"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="08262-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="08262-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="08262-105">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="08262-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="08262-106">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="08262-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="08262-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="08262-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="08262-108">权限</span><span class="sxs-lookup"><span data-stu-id="08262-108">Permissions</span></span>

<span data-ttu-id="08262-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08262-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08262-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08262-111">Permission type</span></span>                        | <span data-ttu-id="08262-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08262-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08262-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08262-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="08262-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08262-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08262-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08262-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08262-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08262-116">Not supported.</span></span>                           |
| <span data-ttu-id="08262-117">应用</span><span class="sxs-lookup"><span data-stu-id="08262-117">Application</span></span>                            | <span data-ttu-id="08262-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08262-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="08262-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08262-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="08262-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="08262-120">Function parameters</span></span>

<span data-ttu-id="08262-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="08262-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="08262-122">参数</span><span class="sxs-lookup"><span data-stu-id="08262-122">Parameter</span></span> | <span data-ttu-id="08262-123">类型</span><span class="sxs-lookup"><span data-stu-id="08262-123">Type</span></span>   | <span data-ttu-id="08262-124">说明</span><span class="sxs-lookup"><span data-stu-id="08262-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08262-125">period</span><span class="sxs-lookup"><span data-stu-id="08262-125">period</span></span>    | <span data-ttu-id="08262-126">string</span><span class="sxs-lookup"><span data-stu-id="08262-126">string</span></span> | <span data-ttu-id="08262-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="08262-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08262-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="08262-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08262-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="08262-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="08262-130">必需。</span><span class="sxs-lookup"><span data-stu-id="08262-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="08262-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="08262-131">Request headers</span></span>

| <span data-ttu-id="08262-132">名称</span><span class="sxs-lookup"><span data-stu-id="08262-132">Name</span></span>          | <span data-ttu-id="08262-133">说明</span><span class="sxs-lookup"><span data-stu-id="08262-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="08262-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="08262-134">Authorization</span></span> | <span data-ttu-id="08262-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="08262-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="08262-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="08262-137">If-None-Match</span></span> | <span data-ttu-id="08262-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="08262-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="08262-139">可选。</span><span class="sxs-lookup"><span data-stu-id="08262-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="08262-140">响应</span><span class="sxs-lookup"><span data-stu-id="08262-140">Response</span></span>

<span data-ttu-id="08262-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="08262-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08262-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="08262-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08262-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="08262-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08262-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="08262-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08262-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="08262-145">Report Refresh Date</span></span>
- <span data-ttu-id="08262-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="08262-146">Report Date</span></span>
- <span data-ttu-id="08262-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="08262-147">Report Period</span></span>
- <span data-ttu-id="08262-148">音频/视频</span><span class="sxs-lookup"><span data-stu-id="08262-148">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="08262-149">示例</span><span class="sxs-lookup"><span data-stu-id="08262-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08262-150">请求</span><span class="sxs-lookup"><span data-stu-id="08262-150">Request</span></span>

<span data-ttu-id="08262-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08262-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="08262-152">响应</span><span class="sxs-lookup"><span data-stu-id="08262-152">Response</span></span>

<span data-ttu-id="08262-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08262-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="08262-154">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="08262-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```
