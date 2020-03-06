---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6cf2014dd422dcbedfeb509b008122d84b56a844
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510079"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="913ee-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="913ee-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="913ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="913ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="913ee-105">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="913ee-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="913ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="913ee-106">Permissions</span></span>

<span data-ttu-id="913ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="913ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="913ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="913ee-109">Permission type</span></span>                        | <span data-ttu-id="913ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="913ee-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="913ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="913ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="913ee-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="913ee-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="913ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="913ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913ee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="913ee-114">Not supported.</span></span>                           |
| <span data-ttu-id="913ee-115">应用</span><span class="sxs-lookup"><span data-stu-id="913ee-115">Application</span></span>                            | <span data-ttu-id="913ee-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="913ee-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="913ee-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="913ee-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="913ee-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="913ee-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="913ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="913ee-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="913ee-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="913ee-120">Function parameters</span></span>

<span data-ttu-id="913ee-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="913ee-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="913ee-122">参数</span><span class="sxs-lookup"><span data-stu-id="913ee-122">Parameter</span></span> | <span data-ttu-id="913ee-123">类型</span><span class="sxs-lookup"><span data-stu-id="913ee-123">Type</span></span>   | <span data-ttu-id="913ee-124">说明</span><span class="sxs-lookup"><span data-stu-id="913ee-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="913ee-125">period</span><span class="sxs-lookup"><span data-stu-id="913ee-125">period</span></span>    | <span data-ttu-id="913ee-126">string</span><span class="sxs-lookup"><span data-stu-id="913ee-126">string</span></span> | <span data-ttu-id="913ee-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="913ee-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="913ee-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="913ee-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="913ee-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="913ee-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="913ee-130">必需。</span><span class="sxs-lookup"><span data-stu-id="913ee-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="913ee-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="913ee-131">Request headers</span></span>

| <span data-ttu-id="913ee-132">名称</span><span class="sxs-lookup"><span data-stu-id="913ee-132">Name</span></span>          | <span data-ttu-id="913ee-133">说明</span><span class="sxs-lookup"><span data-stu-id="913ee-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="913ee-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="913ee-134">Authorization</span></span> | <span data-ttu-id="913ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="913ee-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="913ee-137">响应</span><span class="sxs-lookup"><span data-stu-id="913ee-137">Response</span></span>

<span data-ttu-id="913ee-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="913ee-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="913ee-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="913ee-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="913ee-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="913ee-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="913ee-141">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="913ee-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="913ee-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="913ee-142">Report Refresh Date</span></span>
- <span data-ttu-id="913ee-143">Web</span><span class="sxs-lookup"><span data-stu-id="913ee-143">Web</span></span>
- <span data-ttu-id="913ee-144">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="913ee-144">Windows Phone</span></span>
- <span data-ttu-id="913ee-145">Android 手机</span><span class="sxs-lookup"><span data-stu-id="913ee-145">Android Phone</span></span>
- <span data-ttu-id="913ee-146">iOS</span><span class="sxs-lookup"><span data-stu-id="913ee-146">iOS</span></span>
- <span data-ttu-id="913ee-147">Mac</span><span class="sxs-lookup"><span data-stu-id="913ee-147">Mac</span></span>
- <span data-ttu-id="913ee-148">Windows</span><span class="sxs-lookup"><span data-stu-id="913ee-148">Windows</span></span>
- <span data-ttu-id="913ee-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="913ee-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="913ee-150">示例</span><span class="sxs-lookup"><span data-stu-id="913ee-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="913ee-151">请求</span><span class="sxs-lookup"><span data-stu-id="913ee-151">Request</span></span>

<span data-ttu-id="913ee-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="913ee-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="913ee-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="913ee-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="913ee-154">C#</span><span class="sxs-lookup"><span data-stu-id="913ee-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="913ee-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="913ee-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="913ee-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="913ee-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="913ee-157">Java</span><span class="sxs-lookup"><span data-stu-id="913ee-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="913ee-158">响应</span><span class="sxs-lookup"><span data-stu-id="913ee-158">Response</span></span>

<span data-ttu-id="913ee-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="913ee-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="913ee-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="913ee-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
