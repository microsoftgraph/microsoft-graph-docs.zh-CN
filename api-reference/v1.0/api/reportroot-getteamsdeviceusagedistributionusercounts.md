---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e2913d88e5a9c0a4bfe84b481eb4144f54d6ecff
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44893632"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="db16a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="db16a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="db16a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db16a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db16a-105">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="db16a-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="db16a-106">权限</span><span class="sxs-lookup"><span data-stu-id="db16a-106">Permissions</span></span>

<span data-ttu-id="db16a-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="db16a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="db16a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db16a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db16a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db16a-109">Permission type</span></span>                        | <span data-ttu-id="db16a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db16a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="db16a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db16a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db16a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db16a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="db16a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db16a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db16a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db16a-114">Not supported.</span></span>                           |
| <span data-ttu-id="db16a-115">应用</span><span class="sxs-lookup"><span data-stu-id="db16a-115">Application</span></span>                            | <span data-ttu-id="db16a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db16a-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="db16a-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="db16a-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="db16a-118">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="db16a-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="db16a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db16a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="db16a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="db16a-120">Function parameters</span></span>

<span data-ttu-id="db16a-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="db16a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="db16a-122">参数</span><span class="sxs-lookup"><span data-stu-id="db16a-122">Parameter</span></span> | <span data-ttu-id="db16a-123">类型</span><span class="sxs-lookup"><span data-stu-id="db16a-123">Type</span></span>   | <span data-ttu-id="db16a-124">说明</span><span class="sxs-lookup"><span data-stu-id="db16a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="db16a-125">period</span><span class="sxs-lookup"><span data-stu-id="db16a-125">period</span></span>    | <span data-ttu-id="db16a-126">string</span><span class="sxs-lookup"><span data-stu-id="db16a-126">string</span></span> | <span data-ttu-id="db16a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="db16a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="db16a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="db16a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="db16a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="db16a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="db16a-130">必需。</span><span class="sxs-lookup"><span data-stu-id="db16a-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="db16a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="db16a-131">Request headers</span></span>

| <span data-ttu-id="db16a-132">名称</span><span class="sxs-lookup"><span data-stu-id="db16a-132">Name</span></span>          | <span data-ttu-id="db16a-133">说明</span><span class="sxs-lookup"><span data-stu-id="db16a-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="db16a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="db16a-134">Authorization</span></span> | <span data-ttu-id="db16a-135">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="db16a-135">Bearer {token}.</span></span> <span data-ttu-id="db16a-136">Required.</span><span class="sxs-lookup"><span data-stu-id="db16a-136">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="db16a-137">响应</span><span class="sxs-lookup"><span data-stu-id="db16a-137">Response</span></span>

<span data-ttu-id="db16a-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="db16a-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="db16a-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="db16a-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="db16a-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="db16a-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="db16a-141">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="db16a-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="db16a-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="db16a-142">Report Refresh Date</span></span>
- <span data-ttu-id="db16a-143">Web</span><span class="sxs-lookup"><span data-stu-id="db16a-143">Web</span></span>
- <span data-ttu-id="db16a-144">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="db16a-144">Windows Phone</span></span>
- <span data-ttu-id="db16a-145">Android 手机</span><span class="sxs-lookup"><span data-stu-id="db16a-145">Android Phone</span></span>
- <span data-ttu-id="db16a-146">iOS</span><span class="sxs-lookup"><span data-stu-id="db16a-146">iOS</span></span>
- <span data-ttu-id="db16a-147">Mac</span><span class="sxs-lookup"><span data-stu-id="db16a-147">Mac</span></span>
- <span data-ttu-id="db16a-148">Windows</span><span class="sxs-lookup"><span data-stu-id="db16a-148">Windows</span></span>
- <span data-ttu-id="db16a-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="db16a-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="db16a-150">示例</span><span class="sxs-lookup"><span data-stu-id="db16a-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="db16a-151">请求</span><span class="sxs-lookup"><span data-stu-id="db16a-151">Request</span></span>

<span data-ttu-id="db16a-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db16a-152">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="db16a-153">响应</span><span class="sxs-lookup"><span data-stu-id="db16a-153">Response</span></span>

<span data-ttu-id="db16a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db16a-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="db16a-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="db16a-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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
