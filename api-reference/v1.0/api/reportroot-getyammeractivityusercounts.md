---
title: 'reportRoot: getYammerActivityUserCounts'
description: 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: bd49374f339034dfa9c43f5cca7299287b40ffd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956162"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="2c9c5-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2c9c5-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="2c9c5-104">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="2c9c5-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c9c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="2c9c5-106">Permissions</span></span>

<span data-ttu-id="2c9c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c9c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c9c5-109">Permission type</span></span>                        | <span data-ttu-id="2c9c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c9c5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2c9c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c9c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c9c5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c9c5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2c9c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c9c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c9c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-114">Not supported.</span></span>                           |
| <span data-ttu-id="2c9c5-115">应用</span><span class="sxs-lookup"><span data-stu-id="2c9c5-115">Application</span></span>                            | <span data-ttu-id="2c9c5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c9c5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2c9c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c9c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2c9c5-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="2c9c5-118">Function parameters</span></span>

<span data-ttu-id="2c9c5-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2c9c5-120">参数</span><span class="sxs-lookup"><span data-stu-id="2c9c5-120">Parameter</span></span> | <span data-ttu-id="2c9c5-121">类型</span><span class="sxs-lookup"><span data-stu-id="2c9c5-121">Type</span></span>   | <span data-ttu-id="2c9c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c9c5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2c9c5-123">period</span><span class="sxs-lookup"><span data-stu-id="2c9c5-123">period</span></span>    | <span data-ttu-id="2c9c5-124">string</span><span class="sxs-lookup"><span data-stu-id="2c9c5-124">string</span></span> | <span data-ttu-id="2c9c5-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2c9c5-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2c9c5-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2c9c5-128">必需。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2c9c5-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c9c5-129">Request headers</span></span>

| <span data-ttu-id="2c9c5-130">名称</span><span class="sxs-lookup"><span data-stu-id="2c9c5-130">Name</span></span>          | <span data-ttu-id="2c9c5-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c9c5-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2c9c5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c9c5-132">Authorization</span></span> | <span data-ttu-id="2c9c5-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2c9c5-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2c9c5-135">If-None-Match</span></span> | <span data-ttu-id="2c9c5-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2c9c5-137">可选。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2c9c5-138">响应</span><span class="sxs-lookup"><span data-stu-id="2c9c5-138">Response</span></span>

<span data-ttu-id="2c9c5-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2c9c5-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2c9c5-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2c9c5-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2c9c5-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2c9c5-143">Report Refresh Date</span></span>
- <span data-ttu-id="2c9c5-144">已赞</span><span class="sxs-lookup"><span data-stu-id="2c9c5-144">Liked</span></span>
- <span data-ttu-id="2c9c5-145">已发布</span><span class="sxs-lookup"><span data-stu-id="2c9c5-145">Posted</span></span>
- <span data-ttu-id="2c9c5-146">已阅读</span><span class="sxs-lookup"><span data-stu-id="2c9c5-146">Read</span></span>
- <span data-ttu-id="2c9c5-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="2c9c5-147">Report Date</span></span>
- <span data-ttu-id="2c9c5-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="2c9c5-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2c9c5-149">示例</span><span class="sxs-lookup"><span data-stu-id="2c9c5-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2c9c5-150">请求</span><span class="sxs-lookup"><span data-stu-id="2c9c5-150">Request</span></span>

<span data-ttu-id="2c9c5-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2c9c5-152">响应</span><span class="sxs-lookup"><span data-stu-id="2c9c5-152">Response</span></span>

<span data-ttu-id="2c9c5-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="2c9c5-154">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2c9c5-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
