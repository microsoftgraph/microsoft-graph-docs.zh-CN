---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: 获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 303e4c98f3e9456811b06b1bc0883dd79b0606d9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052017"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="5056a-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="5056a-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="5056a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5056a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5056a-105">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="5056a-105">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="5056a-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="5056a-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="5056a-107">权限</span><span class="sxs-lookup"><span data-stu-id="5056a-107">Permissions</span></span>

<span data-ttu-id="5056a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5056a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5056a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5056a-110">Permission type</span></span>                        | <span data-ttu-id="5056a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5056a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5056a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5056a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5056a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5056a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5056a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5056a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5056a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5056a-115">Not supported.</span></span>                           |
| <span data-ttu-id="5056a-116">应用</span><span class="sxs-lookup"><span data-stu-id="5056a-116">Application</span></span>                            | <span data-ttu-id="5056a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5056a-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5056a-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5056a-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5056a-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="5056a-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5056a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5056a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5056a-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="5056a-121">Function parameters</span></span>

<span data-ttu-id="5056a-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5056a-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5056a-123">参数</span><span class="sxs-lookup"><span data-stu-id="5056a-123">Parameter</span></span> | <span data-ttu-id="5056a-124">类型</span><span class="sxs-lookup"><span data-stu-id="5056a-124">Type</span></span>   | <span data-ttu-id="5056a-125">说明</span><span class="sxs-lookup"><span data-stu-id="5056a-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5056a-126">period</span><span class="sxs-lookup"><span data-stu-id="5056a-126">period</span></span>    | <span data-ttu-id="5056a-127">string</span><span class="sxs-lookup"><span data-stu-id="5056a-127">string</span></span> | <span data-ttu-id="5056a-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5056a-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5056a-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5056a-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5056a-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5056a-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5056a-131">必需。</span><span class="sxs-lookup"><span data-stu-id="5056a-131">Required.</span></span> |

<span data-ttu-id="5056a-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5056a-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5056a-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="5056a-133">The default output type is text/csv.</span></span> <span data-ttu-id="5056a-134">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="5056a-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5056a-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="5056a-135">Request headers</span></span>

| <span data-ttu-id="5056a-136">名称</span><span class="sxs-lookup"><span data-stu-id="5056a-136">Name</span></span>          | <span data-ttu-id="5056a-137">说明</span><span class="sxs-lookup"><span data-stu-id="5056a-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5056a-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="5056a-138">Authorization</span></span> | <span data-ttu-id="5056a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5056a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5056a-141">响应</span><span class="sxs-lookup"><span data-stu-id="5056a-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5056a-142">CSV</span><span class="sxs-lookup"><span data-stu-id="5056a-142">CSV</span></span>

<span data-ttu-id="5056a-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5056a-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5056a-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5056a-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5056a-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5056a-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5056a-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5056a-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5056a-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5056a-147">Report Refresh Date</span></span>
- <span data-ttu-id="5056a-148">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="5056a-148">Viewed Or Edited</span></span>
- <span data-ttu-id="5056a-149">已同步</span><span class="sxs-lookup"><span data-stu-id="5056a-149">Synced</span></span>
- <span data-ttu-id="5056a-150">已内部共享</span><span class="sxs-lookup"><span data-stu-id="5056a-150">Shared Internally</span></span>
- <span data-ttu-id="5056a-151">已外部共享</span><span class="sxs-lookup"><span data-stu-id="5056a-151">Shared Externally</span></span>
- <span data-ttu-id="5056a-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="5056a-152">Report Date</span></span>
- <span data-ttu-id="5056a-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="5056a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5056a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="5056a-154">JSON</span></span>

<span data-ttu-id="5056a-155">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[siteActivitySummary](../resources/siteactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="5056a-155">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5056a-156">示例</span><span class="sxs-lookup"><span data-stu-id="5056a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5056a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="5056a-157">CSV</span></span>

<span data-ttu-id="5056a-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="5056a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5056a-159">请求</span><span class="sxs-lookup"><span data-stu-id="5056a-159">Request</span></span>

<span data-ttu-id="5056a-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5056a-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5056a-161">响应</span><span class="sxs-lookup"><span data-stu-id="5056a-161">Response</span></span>

<span data-ttu-id="5056a-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5056a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5056a-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5056a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="5056a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="5056a-164">JSON</span></span>

<span data-ttu-id="5056a-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="5056a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5056a-166">请求</span><span class="sxs-lookup"><span data-stu-id="5056a-166">Request</span></span>

<span data-ttu-id="5056a-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5056a-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5056a-168">响应</span><span class="sxs-lookup"><span data-stu-id="5056a-168">Response</span></span>

<span data-ttu-id="5056a-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5056a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="5056a-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5056a-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
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


