---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4896ca7cbe76ec9b0d730cc67faaafb78023ebae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582200"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="0c001-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="0c001-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="0c001-105">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="0c001-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="0c001-106">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="0c001-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="0c001-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="0c001-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c001-108">权限</span><span class="sxs-lookup"><span data-stu-id="0c001-108">Permissions</span></span>

<span data-ttu-id="0c001-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c001-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c001-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c001-111">Permission type</span></span>                        | <span data-ttu-id="0c001-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c001-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c001-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c001-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c001-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c001-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c001-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c001-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c001-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c001-116">Not supported.</span></span>                           |
| <span data-ttu-id="0c001-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c001-117">Application</span></span>                            | <span data-ttu-id="0c001-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c001-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0c001-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c001-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0c001-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="0c001-120">Function parameters</span></span>

<span data-ttu-id="0c001-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0c001-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0c001-122">参数</span><span class="sxs-lookup"><span data-stu-id="0c001-122">Parameter</span></span> | <span data-ttu-id="0c001-123">类型</span><span class="sxs-lookup"><span data-stu-id="0c001-123">Type</span></span>   | <span data-ttu-id="0c001-124">说明</span><span class="sxs-lookup"><span data-stu-id="0c001-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0c001-125">period</span><span class="sxs-lookup"><span data-stu-id="0c001-125">period</span></span>    | <span data-ttu-id="0c001-126">string</span><span class="sxs-lookup"><span data-stu-id="0c001-126">string</span></span> | <span data-ttu-id="0c001-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0c001-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0c001-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0c001-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0c001-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0c001-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0c001-130">必需。</span><span class="sxs-lookup"><span data-stu-id="0c001-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0c001-131">请求头</span><span class="sxs-lookup"><span data-stu-id="0c001-131">Request headers</span></span>

| <span data-ttu-id="0c001-132">名称</span><span class="sxs-lookup"><span data-stu-id="0c001-132">Name</span></span>          | <span data-ttu-id="0c001-133">说明</span><span class="sxs-lookup"><span data-stu-id="0c001-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0c001-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c001-134">Authorization</span></span> | <span data-ttu-id="0c001-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c001-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0c001-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0c001-137">If-None-Match</span></span> | <span data-ttu-id="0c001-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0c001-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0c001-139">可选。</span><span class="sxs-lookup"><span data-stu-id="0c001-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0c001-140">响应</span><span class="sxs-lookup"><span data-stu-id="0c001-140">Response</span></span>

<span data-ttu-id="0c001-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0c001-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c001-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0c001-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c001-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="0c001-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c001-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="0c001-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0c001-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0c001-145">Report Refresh Date</span></span>
- <span data-ttu-id="0c001-146">总计</span><span class="sxs-lookup"><span data-stu-id="0c001-146">Total</span></span>
- <span data-ttu-id="0c001-147">活跃</span><span class="sxs-lookup"><span data-stu-id="0c001-147">Active</span></span>
- <span data-ttu-id="0c001-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="0c001-148">Report Date</span></span>
- <span data-ttu-id="0c001-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="0c001-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0c001-150">示例</span><span class="sxs-lookup"><span data-stu-id="0c001-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0c001-151">请求</span><span class="sxs-lookup"><span data-stu-id="0c001-151">Request</span></span>

<span data-ttu-id="0c001-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c001-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0c001-153">响应</span><span class="sxs-lookup"><span data-stu-id="0c001-153">Response</span></span>

<span data-ttu-id="0c001-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c001-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="0c001-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0c001-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
