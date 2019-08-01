---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d84596fc283b09c0cbf30c8855424c7e76f4e45e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021998"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="0575f-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="0575f-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="0575f-104">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="0575f-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="0575f-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="0575f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="0575f-106">权限</span><span class="sxs-lookup"><span data-stu-id="0575f-106">Permissions</span></span>

<span data-ttu-id="0575f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0575f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0575f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0575f-109">Permission type</span></span>                        | <span data-ttu-id="0575f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0575f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0575f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0575f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0575f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0575f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0575f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0575f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0575f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0575f-114">Not supported.</span></span>                           |
| <span data-ttu-id="0575f-115">应用</span><span class="sxs-lookup"><span data-stu-id="0575f-115">Application</span></span>                            | <span data-ttu-id="0575f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0575f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0575f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0575f-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0575f-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0575f-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0575f-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="0575f-119">Function parameters</span></span>

<span data-ttu-id="0575f-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0575f-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0575f-121">参数</span><span class="sxs-lookup"><span data-stu-id="0575f-121">Parameter</span></span> | <span data-ttu-id="0575f-122">类型</span><span class="sxs-lookup"><span data-stu-id="0575f-122">Type</span></span>   | <span data-ttu-id="0575f-123">说明</span><span class="sxs-lookup"><span data-stu-id="0575f-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0575f-124">period</span><span class="sxs-lookup"><span data-stu-id="0575f-124">period</span></span>    | <span data-ttu-id="0575f-125">string</span><span class="sxs-lookup"><span data-stu-id="0575f-125">string</span></span> | <span data-ttu-id="0575f-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0575f-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0575f-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0575f-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0575f-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0575f-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0575f-129">必需。</span><span class="sxs-lookup"><span data-stu-id="0575f-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0575f-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="0575f-130">Request headers</span></span>

| <span data-ttu-id="0575f-131">名称</span><span class="sxs-lookup"><span data-stu-id="0575f-131">Name</span></span>          | <span data-ttu-id="0575f-132">说明</span><span class="sxs-lookup"><span data-stu-id="0575f-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0575f-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0575f-133">Authorization</span></span> | <span data-ttu-id="0575f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0575f-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0575f-136">响应</span><span class="sxs-lookup"><span data-stu-id="0575f-136">Response</span></span>

<span data-ttu-id="0575f-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0575f-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0575f-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0575f-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0575f-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="0575f-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0575f-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="0575f-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0575f-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0575f-141">Report Refresh Date</span></span>
- <span data-ttu-id="0575f-142">Office 365</span><span class="sxs-lookup"><span data-stu-id="0575f-142">Office 365</span></span>
- <span data-ttu-id="0575f-143">Exchange</span><span class="sxs-lookup"><span data-stu-id="0575f-143">Exchange</span></span>
- <span data-ttu-id="0575f-144">OneDrive</span><span class="sxs-lookup"><span data-stu-id="0575f-144">OneDrive</span></span>
- <span data-ttu-id="0575f-145">SharePoint</span><span class="sxs-lookup"><span data-stu-id="0575f-145">SharePoint</span></span>
- <span data-ttu-id="0575f-146">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="0575f-146">Skype For Business</span></span> 
- <span data-ttu-id="0575f-147">Yammer</span><span class="sxs-lookup"><span data-stu-id="0575f-147">Yammer</span></span>
- <span data-ttu-id="0575f-148">Teams</span><span class="sxs-lookup"><span data-stu-id="0575f-148">Teams</span></span>
- <span data-ttu-id="0575f-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="0575f-149">Report Date</span></span>
- <span data-ttu-id="0575f-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="0575f-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0575f-151">示例</span><span class="sxs-lookup"><span data-stu-id="0575f-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0575f-152">请求</span><span class="sxs-lookup"><span data-stu-id="0575f-152">Request</span></span>

<span data-ttu-id="0575f-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0575f-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0575f-154">C#</span><span class="sxs-lookup"><span data-stu-id="0575f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0575f-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="0575f-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0575f-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="0575f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0575f-157">Java</span><span class="sxs-lookup"><span data-stu-id="0575f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0575f-158">响应</span><span class="sxs-lookup"><span data-stu-id="0575f-158">Response</span></span>

<span data-ttu-id="0575f-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0575f-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="0575f-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0575f-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
