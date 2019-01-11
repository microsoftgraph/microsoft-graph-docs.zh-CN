---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: 按 Outlook 桌面版获取唯一用户数。
localization_priority: Normal
ms.openlocfilehash: d5699e736720ffec05eec8d506fe5bde42a29214
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833997"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="97914-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="97914-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="97914-104">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="97914-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="97914-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="97914-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="97914-106">权限</span><span class="sxs-lookup"><span data-stu-id="97914-106">Permissions</span></span>

<span data-ttu-id="97914-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97914-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97914-109">Permission type</span></span>                        | <span data-ttu-id="97914-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97914-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="97914-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97914-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="97914-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97914-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="97914-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97914-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97914-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97914-114">Not supported.</span></span>                           |
| <span data-ttu-id="97914-115">应用</span><span class="sxs-lookup"><span data-stu-id="97914-115">Application</span></span>                            | <span data-ttu-id="97914-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97914-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="97914-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97914-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="97914-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="97914-118">Function parameters</span></span>

<span data-ttu-id="97914-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="97914-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="97914-120">参数</span><span class="sxs-lookup"><span data-stu-id="97914-120">Parameter</span></span> | <span data-ttu-id="97914-121">类型</span><span class="sxs-lookup"><span data-stu-id="97914-121">Type</span></span>   | <span data-ttu-id="97914-122">说明</span><span class="sxs-lookup"><span data-stu-id="97914-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="97914-123">period</span><span class="sxs-lookup"><span data-stu-id="97914-123">period</span></span>    | <span data-ttu-id="97914-124">string</span><span class="sxs-lookup"><span data-stu-id="97914-124">string</span></span> | <span data-ttu-id="97914-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="97914-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="97914-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="97914-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="97914-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="97914-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="97914-128">必需。</span><span class="sxs-lookup"><span data-stu-id="97914-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="97914-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="97914-129">Request headers</span></span>

| <span data-ttu-id="97914-130">名称</span><span class="sxs-lookup"><span data-stu-id="97914-130">Name</span></span>          | <span data-ttu-id="97914-131">说明</span><span class="sxs-lookup"><span data-stu-id="97914-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="97914-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="97914-132">Authorization</span></span> | <span data-ttu-id="97914-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="97914-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="97914-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="97914-135">If-None-Match</span></span> | <span data-ttu-id="97914-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="97914-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="97914-137">可选。</span><span class="sxs-lookup"><span data-stu-id="97914-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="97914-138">响应</span><span class="sxs-lookup"><span data-stu-id="97914-138">Response</span></span>

<span data-ttu-id="97914-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="97914-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="97914-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="97914-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="97914-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="97914-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="97914-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="97914-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="97914-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="97914-143">Report Refresh Date</span></span>
- <span data-ttu-id="97914-144">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="97914-144">Outlook 2016</span></span>
- <span data-ttu-id="97914-145">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="97914-145">Outlook 2013</span></span>
- <span data-ttu-id="97914-146">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="97914-146">Outlook 2010</span></span>
- <span data-ttu-id="97914-147">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="97914-147">Outlook 2007</span></span>
- <span data-ttu-id="97914-148">不确定</span><span class="sxs-lookup"><span data-stu-id="97914-148">Undetermined</span></span>
- <span data-ttu-id="97914-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="97914-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="97914-150">示例</span><span class="sxs-lookup"><span data-stu-id="97914-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97914-151">请求</span><span class="sxs-lookup"><span data-stu-id="97914-151">Request</span></span>

<span data-ttu-id="97914-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97914-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="97914-153">响应</span><span class="sxs-lookup"><span data-stu-id="97914-153">Response</span></span>

<span data-ttu-id="97914-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97914-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="97914-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="97914-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```
