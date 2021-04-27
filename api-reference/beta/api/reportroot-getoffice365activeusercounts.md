---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2b155d27a0c32f934b6e5ea980f5ba85a5c8c652
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053529"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="e6f1f-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="e6f1f-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="e6f1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f1f-105">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="e6f1f-106">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f1f-107">权限</span><span class="sxs-lookup"><span data-stu-id="e6f1f-107">Permissions</span></span>

<span data-ttu-id="e6f1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6f1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6f1f-110">Permission type</span></span>                        | <span data-ttu-id="e6f1f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6f1f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6f1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f1f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6f1f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6f1f-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6f1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6f1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-115">Not supported.</span></span>                           |
| <span data-ttu-id="e6f1f-116">应用</span><span class="sxs-lookup"><span data-stu-id="e6f1f-116">Application</span></span>                            | <span data-ttu-id="e6f1f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6f1f-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e6f1f-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e6f1f-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e6f1f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6f1f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e6f1f-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="e6f1f-121">Function parameters</span></span>

<span data-ttu-id="e6f1f-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e6f1f-123">参数</span><span class="sxs-lookup"><span data-stu-id="e6f1f-123">Parameter</span></span> | <span data-ttu-id="e6f1f-124">类型</span><span class="sxs-lookup"><span data-stu-id="e6f1f-124">Type</span></span>   | <span data-ttu-id="e6f1f-125">说明</span><span class="sxs-lookup"><span data-stu-id="e6f1f-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6f1f-126">period</span><span class="sxs-lookup"><span data-stu-id="e6f1f-126">period</span></span>    | <span data-ttu-id="e6f1f-127">string</span><span class="sxs-lookup"><span data-stu-id="e6f1f-127">string</span></span> | <span data-ttu-id="e6f1f-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6f1f-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6f1f-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e6f1f-131">必需。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-131">Required.</span></span> |

<span data-ttu-id="e6f1f-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e6f1f-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-133">The default output type is text/csv.</span></span> <span data-ttu-id="e6f1f-134">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6f1f-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6f1f-135">Request headers</span></span>

| <span data-ttu-id="e6f1f-136">名称</span><span class="sxs-lookup"><span data-stu-id="e6f1f-136">Name</span></span>          | <span data-ttu-id="e6f1f-137">说明</span><span class="sxs-lookup"><span data-stu-id="e6f1f-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e6f1f-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6f1f-138">Authorization</span></span> | <span data-ttu-id="e6f1f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e6f1f-141">响应</span><span class="sxs-lookup"><span data-stu-id="e6f1f-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e6f1f-142">CSV</span><span class="sxs-lookup"><span data-stu-id="e6f1f-142">CSV</span></span>

<span data-ttu-id="e6f1f-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6f1f-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6f1f-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6f1f-146">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="e6f1f-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="e6f1f-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e6f1f-147">Report Refresh Date</span></span>
- <span data-ttu-id="e6f1f-148">Office 365</span><span class="sxs-lookup"><span data-stu-id="e6f1f-148">Office 365</span></span>
- <span data-ttu-id="e6f1f-149">Exchange</span><span class="sxs-lookup"><span data-stu-id="e6f1f-149">Exchange</span></span>
- <span data-ttu-id="e6f1f-150">OneDrive</span><span class="sxs-lookup"><span data-stu-id="e6f1f-150">OneDrive</span></span>
- <span data-ttu-id="e6f1f-151">SharePoint</span><span class="sxs-lookup"><span data-stu-id="e6f1f-151">SharePoint</span></span>
- <span data-ttu-id="e6f1f-152">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="e6f1f-152">Skype For Business</span></span> 
- <span data-ttu-id="e6f1f-153">Yammer</span><span class="sxs-lookup"><span data-stu-id="e6f1f-153">Yammer</span></span>
- <span data-ttu-id="e6f1f-154">Teams</span><span class="sxs-lookup"><span data-stu-id="e6f1f-154">Teams</span></span>
- <span data-ttu-id="e6f1f-155">报表日期</span><span class="sxs-lookup"><span data-stu-id="e6f1f-155">Report Date</span></span>
- <span data-ttu-id="e6f1f-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="e6f1f-156">Report Period</span></span>

<span data-ttu-id="e6f1f-157">由世纪Graph运营的 Microsoft Graph不支持以下列：</span><span class="sxs-lookup"><span data-stu-id="e6f1f-157">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e6f1f-158">Yammer</span><span class="sxs-lookup"><span data-stu-id="e6f1f-158">Yammer</span></span>
- <span data-ttu-id="e6f1f-159">Teams</span><span class="sxs-lookup"><span data-stu-id="e6f1f-159">Teams</span></span>

### <a name="json"></a><span data-ttu-id="e6f1f-160">JSON</span><span class="sxs-lookup"><span data-stu-id="e6f1f-160">JSON</span></span>

<span data-ttu-id="e6f1f-161">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-161">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="e6f1f-162">由世纪银行运营的 Microsoft Graph不支持 **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="e6f1f-162">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e6f1f-163">yammer</span><span class="sxs-lookup"><span data-stu-id="e6f1f-163">yammer</span></span>
- <span data-ttu-id="e6f1f-164">teams</span><span class="sxs-lookup"><span data-stu-id="e6f1f-164">teams</span></span>

## <a name="example"></a><span data-ttu-id="e6f1f-165">示例</span><span class="sxs-lookup"><span data-stu-id="e6f1f-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e6f1f-166">CSV</span><span class="sxs-lookup"><span data-stu-id="e6f1f-166">CSV</span></span>

<span data-ttu-id="e6f1f-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e6f1f-168">请求</span><span class="sxs-lookup"><span data-stu-id="e6f1f-168">Request</span></span>

<span data-ttu-id="e6f1f-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="e6f1f-170">响应</span><span class="sxs-lookup"><span data-stu-id="e6f1f-170">Response</span></span>

<span data-ttu-id="e6f1f-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e6f1f-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e6f1f-173">JSON</span><span class="sxs-lookup"><span data-stu-id="e6f1f-173">JSON</span></span>

<span data-ttu-id="e6f1f-174">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e6f1f-175">请求</span><span class="sxs-lookup"><span data-stu-id="e6f1f-175">Request</span></span>

<span data-ttu-id="e6f1f-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="e6f1f-177">响应</span><span class="sxs-lookup"><span data-stu-id="e6f1f-177">Response</span></span>

<span data-ttu-id="e6f1f-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-178">The following is an example of the response.</span></span>

> <span data-ttu-id="e6f1f-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e6f1f-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
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


