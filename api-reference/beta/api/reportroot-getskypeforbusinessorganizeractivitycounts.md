---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4c8fb9b695b5722702dfcac6b77d2bd59582de93
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896684"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="879c1-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="879c1-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="879c1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="879c1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="879c1-106">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="879c1-106">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="879c1-107">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="879c1-107">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="879c1-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="879c1-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="879c1-109">权限</span><span class="sxs-lookup"><span data-stu-id="879c1-109">Permissions</span></span>

<span data-ttu-id="879c1-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="879c1-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="879c1-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="879c1-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="879c1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="879c1-112">Permission type</span></span>                        | <span data-ttu-id="879c1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="879c1-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="879c1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="879c1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="879c1-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="879c1-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="879c1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="879c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="879c1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="879c1-117">Not supported.</span></span>                           |
| <span data-ttu-id="879c1-118">应用</span><span class="sxs-lookup"><span data-stu-id="879c1-118">Application</span></span>                            | <span data-ttu-id="879c1-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="879c1-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="879c1-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="879c1-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="879c1-121">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="879c1-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="879c1-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="879c1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="879c1-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="879c1-123">Function parameters</span></span>

<span data-ttu-id="879c1-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="879c1-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="879c1-125">参数</span><span class="sxs-lookup"><span data-stu-id="879c1-125">Parameter</span></span> | <span data-ttu-id="879c1-126">类型</span><span class="sxs-lookup"><span data-stu-id="879c1-126">Type</span></span>   | <span data-ttu-id="879c1-127">说明</span><span class="sxs-lookup"><span data-stu-id="879c1-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="879c1-128">period</span><span class="sxs-lookup"><span data-stu-id="879c1-128">period</span></span>    | <span data-ttu-id="879c1-129">string</span><span class="sxs-lookup"><span data-stu-id="879c1-129">string</span></span> | <span data-ttu-id="879c1-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="879c1-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="879c1-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="879c1-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="879c1-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="879c1-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="879c1-133">必需。</span><span class="sxs-lookup"><span data-stu-id="879c1-133">Required.</span></span> |

<span data-ttu-id="879c1-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="879c1-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="879c1-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="879c1-135">The default output type is text/csv.</span></span> <span data-ttu-id="879c1-136">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="879c1-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="879c1-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="879c1-137">Request headers</span></span>

| <span data-ttu-id="879c1-138">名称</span><span class="sxs-lookup"><span data-stu-id="879c1-138">Name</span></span>          | <span data-ttu-id="879c1-139">说明</span><span class="sxs-lookup"><span data-stu-id="879c1-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="879c1-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="879c1-140">Authorization</span></span> | <span data-ttu-id="879c1-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="879c1-141">Bearer {token}.</span></span> <span data-ttu-id="879c1-142">Required.</span><span class="sxs-lookup"><span data-stu-id="879c1-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="879c1-143">响应</span><span class="sxs-lookup"><span data-stu-id="879c1-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="879c1-144">CSV</span><span class="sxs-lookup"><span data-stu-id="879c1-144">CSV</span></span>

<span data-ttu-id="879c1-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="879c1-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="879c1-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="879c1-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="879c1-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="879c1-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="879c1-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="879c1-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="879c1-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="879c1-149">Report Refresh Date</span></span>
- <span data-ttu-id="879c1-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="879c1-150">Report Date</span></span>
- <span data-ttu-id="879c1-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="879c1-151">Report Period</span></span>
- <span data-ttu-id="879c1-152">IM</span><span class="sxs-lookup"><span data-stu-id="879c1-152">IM</span></span>
- <span data-ttu-id="879c1-153">音频/视频</span><span class="sxs-lookup"><span data-stu-id="879c1-153">Audio/Video</span></span>
- <span data-ttu-id="879c1-154">应用共享</span><span class="sxs-lookup"><span data-stu-id="879c1-154">App Sharing</span></span>
- <span data-ttu-id="879c1-155">Web</span><span class="sxs-lookup"><span data-stu-id="879c1-155">Web</span></span>
- <span data-ttu-id="879c1-156">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="879c1-156">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="879c1-157">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="879c1-157">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="879c1-158">JSON</span><span class="sxs-lookup"><span data-stu-id="879c1-158">JSON</span></span>

<span data-ttu-id="879c1-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="879c1-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="879c1-160">示例</span><span class="sxs-lookup"><span data-stu-id="879c1-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="879c1-161">CSV</span><span class="sxs-lookup"><span data-stu-id="879c1-161">CSV</span></span>

<span data-ttu-id="879c1-162">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="879c1-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="879c1-163">请求</span><span class="sxs-lookup"><span data-stu-id="879c1-163">Request</span></span>

<span data-ttu-id="879c1-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="879c1-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="879c1-165">响应</span><span class="sxs-lookup"><span data-stu-id="879c1-165">Response</span></span>

<span data-ttu-id="879c1-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="879c1-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="879c1-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="879c1-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="879c1-168">JSON</span><span class="sxs-lookup"><span data-stu-id="879c1-168">JSON</span></span>

<span data-ttu-id="879c1-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="879c1-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="879c1-170">请求</span><span class="sxs-lookup"><span data-stu-id="879c1-170">Request</span></span>

<span data-ttu-id="879c1-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="879c1-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="879c1-172">响应</span><span class="sxs-lookup"><span data-stu-id="879c1-172">Response</span></span>

<span data-ttu-id="879c1-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="879c1-173">The following is an example of the response.</span></span>

> <span data-ttu-id="879c1-174">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="879c1-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="879c1-175">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="879c1-175">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
      "reportRefreshDate": "2017-09-01", 
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
