---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: 按设备类型获取 Microsoft Teams 每日唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 806f931c69e08451195317ca84eebc2bb990f613
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865237"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="c3043-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c3043-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="c3043-104">按设备类型获取 Microsoft Teams 每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="c3043-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3043-105">权限</span><span class="sxs-lookup"><span data-stu-id="c3043-105">Permissions</span></span>

<span data-ttu-id="c3043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3043-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3043-108">Permission type</span></span>                        | <span data-ttu-id="c3043-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3043-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c3043-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3043-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3043-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3043-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c3043-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3043-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3043-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3043-113">Not supported.</span></span>                           |
| <span data-ttu-id="c3043-114">应用</span><span class="sxs-lookup"><span data-stu-id="c3043-114">Application</span></span>                            | <span data-ttu-id="c3043-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3043-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="c3043-116">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="c3043-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c3043-117">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="c3043-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c3043-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3043-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c3043-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="c3043-119">Function parameters</span></span>

<span data-ttu-id="c3043-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c3043-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c3043-121">参数</span><span class="sxs-lookup"><span data-stu-id="c3043-121">Parameter</span></span> | <span data-ttu-id="c3043-122">类型</span><span class="sxs-lookup"><span data-stu-id="c3043-122">Type</span></span>   | <span data-ttu-id="c3043-123">说明</span><span class="sxs-lookup"><span data-stu-id="c3043-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c3043-124">period</span><span class="sxs-lookup"><span data-stu-id="c3043-124">period</span></span>    | <span data-ttu-id="c3043-125">string</span><span class="sxs-lookup"><span data-stu-id="c3043-125">string</span></span> | <span data-ttu-id="c3043-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c3043-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c3043-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c3043-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c3043-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c3043-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c3043-129">必需。</span><span class="sxs-lookup"><span data-stu-id="c3043-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c3043-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3043-130">Request headers</span></span>

| <span data-ttu-id="c3043-131">名称</span><span class="sxs-lookup"><span data-stu-id="c3043-131">Name</span></span>          | <span data-ttu-id="c3043-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3043-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c3043-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3043-133">Authorization</span></span> | <span data-ttu-id="c3043-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3043-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c3043-136">响应</span><span class="sxs-lookup"><span data-stu-id="c3043-136">Response</span></span>

<span data-ttu-id="c3043-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c3043-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c3043-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c3043-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c3043-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="c3043-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c3043-140">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="c3043-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c3043-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c3043-141">Report Refresh Date</span></span>
- <span data-ttu-id="c3043-142">Web</span><span class="sxs-lookup"><span data-stu-id="c3043-142">Web</span></span>
- <span data-ttu-id="c3043-143">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="c3043-143">Windows Phone</span></span>
- <span data-ttu-id="c3043-144">Android 手机</span><span class="sxs-lookup"><span data-stu-id="c3043-144">Android Phone</span></span>
- <span data-ttu-id="c3043-145">iOS</span><span class="sxs-lookup"><span data-stu-id="c3043-145">iOS</span></span>
- <span data-ttu-id="c3043-146">Mac</span><span class="sxs-lookup"><span data-stu-id="c3043-146">Mac</span></span>
- <span data-ttu-id="c3043-147">Windows</span><span class="sxs-lookup"><span data-stu-id="c3043-147">Windows</span></span>
- <span data-ttu-id="c3043-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="c3043-148">Report Date</span></span>
- <span data-ttu-id="c3043-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="c3043-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c3043-150">示例</span><span class="sxs-lookup"><span data-stu-id="c3043-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3043-151">请求</span><span class="sxs-lookup"><span data-stu-id="c3043-151">Request</span></span>

<span data-ttu-id="c3043-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c3043-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3043-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3043-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3043-154">C#</span><span class="sxs-lookup"><span data-stu-id="c3043-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3043-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3043-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3043-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3043-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3043-157">Java</span><span class="sxs-lookup"><span data-stu-id="c3043-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c3043-158">响应</span><span class="sxs-lookup"><span data-stu-id="c3043-158">Response</span></span>

<span data-ttu-id="c3043-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c3043-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="c3043-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c3043-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
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
