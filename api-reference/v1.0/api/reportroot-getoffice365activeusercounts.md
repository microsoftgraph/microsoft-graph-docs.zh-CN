---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f5e49018ddc6d0f576fffbd03b39d69675475eee
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865410"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="4d351-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="4d351-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="4d351-104">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="4d351-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="4d351-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="4d351-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d351-106">权限</span><span class="sxs-lookup"><span data-stu-id="4d351-106">Permissions</span></span>

<span data-ttu-id="4d351-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d351-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d351-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d351-109">Permission type</span></span>                        | <span data-ttu-id="4d351-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d351-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4d351-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d351-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d351-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d351-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4d351-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d351-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d351-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d351-114">Not supported.</span></span>                           |
| <span data-ttu-id="4d351-115">应用</span><span class="sxs-lookup"><span data-stu-id="4d351-115">Application</span></span>                            | <span data-ttu-id="4d351-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d351-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="4d351-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="4d351-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4d351-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="4d351-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4d351-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d351-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4d351-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="4d351-120">Function parameters</span></span>

<span data-ttu-id="4d351-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4d351-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4d351-122">参数</span><span class="sxs-lookup"><span data-stu-id="4d351-122">Parameter</span></span> | <span data-ttu-id="4d351-123">类型</span><span class="sxs-lookup"><span data-stu-id="4d351-123">Type</span></span>   | <span data-ttu-id="4d351-124">说明</span><span class="sxs-lookup"><span data-stu-id="4d351-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4d351-125">period</span><span class="sxs-lookup"><span data-stu-id="4d351-125">period</span></span>    | <span data-ttu-id="4d351-126">string</span><span class="sxs-lookup"><span data-stu-id="4d351-126">string</span></span> | <span data-ttu-id="4d351-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4d351-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4d351-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4d351-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4d351-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4d351-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4d351-130">必需。</span><span class="sxs-lookup"><span data-stu-id="4d351-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4d351-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d351-131">Request headers</span></span>

| <span data-ttu-id="4d351-132">名称</span><span class="sxs-lookup"><span data-stu-id="4d351-132">Name</span></span>          | <span data-ttu-id="4d351-133">说明</span><span class="sxs-lookup"><span data-stu-id="4d351-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4d351-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d351-134">Authorization</span></span> | <span data-ttu-id="4d351-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d351-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4d351-137">响应</span><span class="sxs-lookup"><span data-stu-id="4d351-137">Response</span></span>

<span data-ttu-id="4d351-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4d351-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4d351-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4d351-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4d351-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4d351-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4d351-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4d351-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4d351-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4d351-142">Report Refresh Date</span></span>
- <span data-ttu-id="4d351-143">Office 365</span><span class="sxs-lookup"><span data-stu-id="4d351-143">Office 365</span></span>
- <span data-ttu-id="4d351-144">Exchange</span><span class="sxs-lookup"><span data-stu-id="4d351-144">Exchange</span></span>
- <span data-ttu-id="4d351-145">OneDrive</span><span class="sxs-lookup"><span data-stu-id="4d351-145">OneDrive</span></span>
- <span data-ttu-id="4d351-146">SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d351-146">SharePoint</span></span>
- <span data-ttu-id="4d351-147">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="4d351-147">Skype For Business</span></span> 
- <span data-ttu-id="4d351-148">Yammer</span><span class="sxs-lookup"><span data-stu-id="4d351-148">Yammer</span></span>
- <span data-ttu-id="4d351-149">Teams</span><span class="sxs-lookup"><span data-stu-id="4d351-149">Teams</span></span>
- <span data-ttu-id="4d351-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="4d351-150">Report Date</span></span>
- <span data-ttu-id="4d351-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="4d351-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4d351-152">示例</span><span class="sxs-lookup"><span data-stu-id="4d351-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4d351-153">请求</span><span class="sxs-lookup"><span data-stu-id="4d351-153">Request</span></span>

<span data-ttu-id="4d351-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d351-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4d351-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d351-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d351-156">C#</span><span class="sxs-lookup"><span data-stu-id="4d351-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d351-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d351-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d351-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d351-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4d351-159">Java</span><span class="sxs-lookup"><span data-stu-id="4d351-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4d351-160">响应</span><span class="sxs-lookup"><span data-stu-id="4d351-160">Response</span></span>

<span data-ttu-id="4d351-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d351-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="4d351-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4d351-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
