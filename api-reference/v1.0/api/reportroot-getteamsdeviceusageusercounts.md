---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: 按设备类型获取 Microsoft Teams 每日唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d883ed329ed7cda602003cb4f84ee509254bc10a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510072"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="3598b-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3598b-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="3598b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3598b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3598b-105">按设备类型获取 Microsoft Teams 每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="3598b-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="3598b-106">权限</span><span class="sxs-lookup"><span data-stu-id="3598b-106">Permissions</span></span>

<span data-ttu-id="3598b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3598b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3598b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3598b-109">Permission type</span></span>                        | <span data-ttu-id="3598b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3598b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3598b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3598b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3598b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3598b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3598b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3598b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3598b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3598b-114">Not supported.</span></span>                           |
| <span data-ttu-id="3598b-115">应用</span><span class="sxs-lookup"><span data-stu-id="3598b-115">Application</span></span>                            | <span data-ttu-id="3598b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3598b-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3598b-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3598b-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3598b-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3598b-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3598b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3598b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3598b-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="3598b-120">Function parameters</span></span>

<span data-ttu-id="3598b-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3598b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3598b-122">参数</span><span class="sxs-lookup"><span data-stu-id="3598b-122">Parameter</span></span> | <span data-ttu-id="3598b-123">类型</span><span class="sxs-lookup"><span data-stu-id="3598b-123">Type</span></span>   | <span data-ttu-id="3598b-124">说明</span><span class="sxs-lookup"><span data-stu-id="3598b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3598b-125">period</span><span class="sxs-lookup"><span data-stu-id="3598b-125">period</span></span>    | <span data-ttu-id="3598b-126">string</span><span class="sxs-lookup"><span data-stu-id="3598b-126">string</span></span> | <span data-ttu-id="3598b-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3598b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3598b-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3598b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3598b-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3598b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3598b-130">必需。</span><span class="sxs-lookup"><span data-stu-id="3598b-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3598b-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="3598b-131">Request headers</span></span>

| <span data-ttu-id="3598b-132">名称</span><span class="sxs-lookup"><span data-stu-id="3598b-132">Name</span></span>          | <span data-ttu-id="3598b-133">说明</span><span class="sxs-lookup"><span data-stu-id="3598b-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3598b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3598b-134">Authorization</span></span> | <span data-ttu-id="3598b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3598b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3598b-137">响应</span><span class="sxs-lookup"><span data-stu-id="3598b-137">Response</span></span>

<span data-ttu-id="3598b-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3598b-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3598b-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3598b-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3598b-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="3598b-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3598b-141">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="3598b-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3598b-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3598b-142">Report Refresh Date</span></span>
- <span data-ttu-id="3598b-143">Web</span><span class="sxs-lookup"><span data-stu-id="3598b-143">Web</span></span>
- <span data-ttu-id="3598b-144">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="3598b-144">Windows Phone</span></span>
- <span data-ttu-id="3598b-145">Android 手机</span><span class="sxs-lookup"><span data-stu-id="3598b-145">Android Phone</span></span>
- <span data-ttu-id="3598b-146">iOS</span><span class="sxs-lookup"><span data-stu-id="3598b-146">iOS</span></span>
- <span data-ttu-id="3598b-147">Mac</span><span class="sxs-lookup"><span data-stu-id="3598b-147">Mac</span></span>
- <span data-ttu-id="3598b-148">Windows</span><span class="sxs-lookup"><span data-stu-id="3598b-148">Windows</span></span>
- <span data-ttu-id="3598b-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="3598b-149">Report Date</span></span>
- <span data-ttu-id="3598b-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="3598b-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3598b-151">示例</span><span class="sxs-lookup"><span data-stu-id="3598b-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3598b-152">请求</span><span class="sxs-lookup"><span data-stu-id="3598b-152">Request</span></span>

<span data-ttu-id="3598b-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3598b-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3598b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3598b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="3598b-155">C#</span><span class="sxs-lookup"><span data-stu-id="3598b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3598b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3598b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3598b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3598b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3598b-158">Java</span><span class="sxs-lookup"><span data-stu-id="3598b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3598b-159">响应</span><span class="sxs-lookup"><span data-stu-id="3598b-159">Response</span></span>

<span data-ttu-id="3598b-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3598b-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="3598b-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3598b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
