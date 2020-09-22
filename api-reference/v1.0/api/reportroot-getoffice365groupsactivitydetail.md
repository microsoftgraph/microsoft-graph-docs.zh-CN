---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 按组获取有关 Microsoft 365 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b53f50c976170a921d076eb56f599e23db878432
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083209"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="4f3b8-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4f3b8-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="4f3b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f3b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f3b8-105">按组获取有关 Microsoft 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="4f3b8-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [microsoft 365 报表-microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f3b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="4f3b8-107">Permissions</span></span>

<span data-ttu-id="4f3b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f3b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f3b8-110">Permission type</span></span>                        | <span data-ttu-id="4f3b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f3b8-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4f3b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f3b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f3b8-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f3b8-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4f3b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f3b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f3b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-115">Not supported.</span></span>                           |
| <span data-ttu-id="4f3b8-116">应用</span><span class="sxs-lookup"><span data-stu-id="4f3b8-116">Application</span></span>                            | <span data-ttu-id="4f3b8-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f3b8-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="4f3b8-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4f3b8-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4f3b8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f3b8-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4f3b8-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-121">Function parameters</span></span>

<span data-ttu-id="4f3b8-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4f3b8-123">参数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-123">Parameter</span></span> | <span data-ttu-id="4f3b8-124">类型</span><span class="sxs-lookup"><span data-stu-id="4f3b8-124">Type</span></span>   | <span data-ttu-id="4f3b8-125">说明</span><span class="sxs-lookup"><span data-stu-id="4f3b8-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4f3b8-126">period</span><span class="sxs-lookup"><span data-stu-id="4f3b8-126">period</span></span>    | <span data-ttu-id="4f3b8-127">string</span><span class="sxs-lookup"><span data-stu-id="4f3b8-127">string</span></span> | <span data-ttu-id="4f3b8-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4f3b8-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4f3b8-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4f3b8-131">date</span><span class="sxs-lookup"><span data-stu-id="4f3b8-131">date</span></span>      | <span data-ttu-id="4f3b8-132">Date</span><span class="sxs-lookup"><span data-stu-id="4f3b8-132">Date</span></span>   | <span data-ttu-id="4f3b8-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4f3b8-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4f3b8-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4f3b8-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f3b8-137">请求头</span><span class="sxs-lookup"><span data-stu-id="4f3b8-137">Request headers</span></span>

| <span data-ttu-id="4f3b8-138">名称</span><span class="sxs-lookup"><span data-stu-id="4f3b8-138">Name</span></span>          | <span data-ttu-id="4f3b8-139">说明</span><span class="sxs-lookup"><span data-stu-id="4f3b8-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4f3b8-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f3b8-140">Authorization</span></span> | <span data-ttu-id="4f3b8-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4f3b8-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4f3b8-143">If-None-Match</span></span> | <span data-ttu-id="4f3b8-144">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4f3b8-145">可选。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4f3b8-146">响应</span><span class="sxs-lookup"><span data-stu-id="4f3b8-146">Response</span></span>

<span data-ttu-id="4f3b8-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4f3b8-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4f3b8-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4f3b8-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4f3b8-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4f3b8-151">Report Refresh Date</span></span>
- <span data-ttu-id="4f3b8-152">组显示名称</span><span class="sxs-lookup"><span data-stu-id="4f3b8-152">Group Display Name</span></span>
- <span data-ttu-id="4f3b8-153">已删除</span><span class="sxs-lookup"><span data-stu-id="4f3b8-153">Is Deleted</span></span>
- <span data-ttu-id="4f3b8-154">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="4f3b8-154">Owner Principal Name</span></span>
- <span data-ttu-id="4f3b8-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="4f3b8-155">Last Activity Date</span></span>
- <span data-ttu-id="4f3b8-156">组类型</span><span class="sxs-lookup"><span data-stu-id="4f3b8-156">Group Type</span></span>
- <span data-ttu-id="4f3b8-157">成员数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-157">Member Count</span></span>
- <span data-ttu-id="4f3b8-158">外部成员数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-158">External Member Count</span></span>
- <span data-ttu-id="4f3b8-159">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="4f3b8-160">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="4f3b8-161">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="4f3b8-162">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="4f3b8-163">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="4f3b8-164">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="4f3b8-165">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="4f3b8-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="4f3b8-166">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="4f3b8-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="4f3b8-167">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="4f3b8-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="4f3b8-168">组 Id</span><span class="sxs-lookup"><span data-stu-id="4f3b8-168">Group Id</span></span>
- <span data-ttu-id="4f3b8-169">报表周期</span><span class="sxs-lookup"><span data-stu-id="4f3b8-169">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4f3b8-170">示例</span><span class="sxs-lookup"><span data-stu-id="4f3b8-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f3b8-171">请求</span><span class="sxs-lookup"><span data-stu-id="4f3b8-171">Request</span></span>

<span data-ttu-id="4f3b8-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-172">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="4f3b8-173">响应</span><span class="sxs-lookup"><span data-stu-id="4f3b8-173">Response</span></span>

<span data-ttu-id="4f3b8-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="4f3b8-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4f3b8-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
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

