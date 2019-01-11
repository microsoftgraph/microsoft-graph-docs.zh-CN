---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.openlocfilehash: 6e62bd5fb8145a2db941048c7b645f76a9f66619
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804821"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="b9d0a-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="b9d0a-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="b9d0a-105">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="b9d0a-106">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="b9d0a-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9d0a-108">权限</span><span class="sxs-lookup"><span data-stu-id="b9d0a-108">Permissions</span></span>

<span data-ttu-id="b9d0a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9d0a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9d0a-111">Permission type</span></span>                        | <span data-ttu-id="b9d0a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9d0a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b9d0a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9d0a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9d0a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9d0a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b9d0a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9d0a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9d0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-116">Not supported.</span></span>                           |
| <span data-ttu-id="b9d0a-117">应用</span><span class="sxs-lookup"><span data-stu-id="b9d0a-117">Application</span></span>                            | <span data-ttu-id="b9d0a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9d0a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b9d0a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9d0a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b9d0a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="b9d0a-120">Function parameters</span></span>

<span data-ttu-id="b9d0a-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b9d0a-122">参数</span><span class="sxs-lookup"><span data-stu-id="b9d0a-122">Parameter</span></span> | <span data-ttu-id="b9d0a-123">类型</span><span class="sxs-lookup"><span data-stu-id="b9d0a-123">Type</span></span>   | <span data-ttu-id="b9d0a-124">说明</span><span class="sxs-lookup"><span data-stu-id="b9d0a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b9d0a-125">period</span><span class="sxs-lookup"><span data-stu-id="b9d0a-125">period</span></span>    | <span data-ttu-id="b9d0a-126">string</span><span class="sxs-lookup"><span data-stu-id="b9d0a-126">string</span></span> | <span data-ttu-id="b9d0a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b9d0a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b9d0a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b9d0a-130">必需。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b9d0a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9d0a-131">Request headers</span></span>

| <span data-ttu-id="b9d0a-132">名称</span><span class="sxs-lookup"><span data-stu-id="b9d0a-132">Name</span></span>          | <span data-ttu-id="b9d0a-133">说明</span><span class="sxs-lookup"><span data-stu-id="b9d0a-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b9d0a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9d0a-134">Authorization</span></span> | <span data-ttu-id="b9d0a-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b9d0a-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b9d0a-137">If-None-Match</span></span> | <span data-ttu-id="b9d0a-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b9d0a-139">可选。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b9d0a-140">响应</span><span class="sxs-lookup"><span data-stu-id="b9d0a-140">Response</span></span>

<span data-ttu-id="b9d0a-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b9d0a-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b9d0a-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b9d0a-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b9d0a-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b9d0a-145">Report Refresh Date</span></span>
- <span data-ttu-id="b9d0a-146">总计</span><span class="sxs-lookup"><span data-stu-id="b9d0a-146">Total</span></span>
- <span data-ttu-id="b9d0a-147">活跃</span><span class="sxs-lookup"><span data-stu-id="b9d0a-147">Active</span></span>
- <span data-ttu-id="b9d0a-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="b9d0a-148">Report Date</span></span>
- <span data-ttu-id="b9d0a-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="b9d0a-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b9d0a-150">示例</span><span class="sxs-lookup"><span data-stu-id="b9d0a-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9d0a-151">请求</span><span class="sxs-lookup"><span data-stu-id="b9d0a-151">Request</span></span>

<span data-ttu-id="b9d0a-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b9d0a-153">响应</span><span class="sxs-lookup"><span data-stu-id="b9d0a-153">Response</span></span>

<span data-ttu-id="b9d0a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="b9d0a-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b9d0a-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
