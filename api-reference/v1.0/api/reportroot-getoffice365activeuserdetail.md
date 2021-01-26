---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取有关 Microsoft 365 活动用户的详细信息。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 773f15ff0b61fb80b4a4cd542082a6305b405d1d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981758"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="036fc-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="036fc-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="036fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="036fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="036fc-105">获取有关 Microsoft 365 活动用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="036fc-105">Get details about Microsoft 365 active users.</span></span>

> <span data-ttu-id="036fc-106">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="036fc-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="036fc-107">权限</span><span class="sxs-lookup"><span data-stu-id="036fc-107">Permissions</span></span>

<span data-ttu-id="036fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="036fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="036fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="036fc-110">Permission type</span></span>                        | <span data-ttu-id="036fc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="036fc-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="036fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="036fc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="036fc-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="036fc-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="036fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="036fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="036fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="036fc-115">Not supported.</span></span>                           |
| <span data-ttu-id="036fc-116">应用</span><span class="sxs-lookup"><span data-stu-id="036fc-116">Application</span></span>                            | <span data-ttu-id="036fc-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="036fc-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="036fc-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="036fc-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="036fc-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="036fc-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="036fc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="036fc-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="036fc-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="036fc-121">Function parameters</span></span>

<span data-ttu-id="036fc-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="036fc-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="036fc-123">参数</span><span class="sxs-lookup"><span data-stu-id="036fc-123">Parameter</span></span> | <span data-ttu-id="036fc-124">类型</span><span class="sxs-lookup"><span data-stu-id="036fc-124">Type</span></span>   | <span data-ttu-id="036fc-125">说明</span><span class="sxs-lookup"><span data-stu-id="036fc-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="036fc-126">period</span><span class="sxs-lookup"><span data-stu-id="036fc-126">period</span></span>    | <span data-ttu-id="036fc-127">string</span><span class="sxs-lookup"><span data-stu-id="036fc-127">string</span></span> | <span data-ttu-id="036fc-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="036fc-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="036fc-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="036fc-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="036fc-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="036fc-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="036fc-131">date</span><span class="sxs-lookup"><span data-stu-id="036fc-131">date</span></span>      | <span data-ttu-id="036fc-132">Date</span><span class="sxs-lookup"><span data-stu-id="036fc-132">Date</span></span>   | <span data-ttu-id="036fc-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="036fc-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="036fc-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="036fc-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="036fc-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="036fc-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="036fc-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="036fc-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="036fc-137">请求头</span><span class="sxs-lookup"><span data-stu-id="036fc-137">Request headers</span></span>

| <span data-ttu-id="036fc-138">名称</span><span class="sxs-lookup"><span data-stu-id="036fc-138">Name</span></span>          | <span data-ttu-id="036fc-139">说明</span><span class="sxs-lookup"><span data-stu-id="036fc-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="036fc-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="036fc-140">Authorization</span></span> | <span data-ttu-id="036fc-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="036fc-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="036fc-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="036fc-143">If-None-Match</span></span> | <span data-ttu-id="036fc-144">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="036fc-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="036fc-145">可选。</span><span class="sxs-lookup"><span data-stu-id="036fc-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="036fc-146">响应</span><span class="sxs-lookup"><span data-stu-id="036fc-146">Response</span></span>

<span data-ttu-id="036fc-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="036fc-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="036fc-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="036fc-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="036fc-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="036fc-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="036fc-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="036fc-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="036fc-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="036fc-151">Report Refresh Date</span></span>
- <span data-ttu-id="036fc-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="036fc-152">User Principal Name</span></span>
- <span data-ttu-id="036fc-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="036fc-153">Display Name</span></span>
- <span data-ttu-id="036fc-154">已删除</span><span class="sxs-lookup"><span data-stu-id="036fc-154">Is Deleted</span></span>
- <span data-ttu-id="036fc-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="036fc-155">Deleted Date</span></span>
- <span data-ttu-id="036fc-156">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-156">Has Exchange License</span></span>
- <span data-ttu-id="036fc-157">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-157">Has OneDrive License</span></span>
- <span data-ttu-id="036fc-158">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-158">Has SharePoint License</span></span>
- <span data-ttu-id="036fc-159">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-159">Has Skype For Business License</span></span>
- <span data-ttu-id="036fc-160">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-160">Has Yammer License</span></span>
- <span data-ttu-id="036fc-161">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="036fc-161">Has Teams License</span></span>
- <span data-ttu-id="036fc-162">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="036fc-163">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="036fc-164">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="036fc-165">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="036fc-166">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="036fc-167">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="036fc-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="036fc-168">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="036fc-169">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="036fc-170">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="036fc-171">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="036fc-172">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="036fc-173">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="036fc-173">Teams License Assign Date</span></span>
- <span data-ttu-id="036fc-174">分配的产品</span><span class="sxs-lookup"><span data-stu-id="036fc-174">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="036fc-175">示例</span><span class="sxs-lookup"><span data-stu-id="036fc-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="036fc-176">请求</span><span class="sxs-lookup"><span data-stu-id="036fc-176">Request</span></span>

<span data-ttu-id="036fc-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="036fc-177">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="036fc-178">响应</span><span class="sxs-lookup"><span data-stu-id="036fc-178">Response</span></span>

<span data-ttu-id="036fc-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="036fc-179">The following is an example of the response.</span></span>

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

<span data-ttu-id="036fc-180">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="036fc-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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

