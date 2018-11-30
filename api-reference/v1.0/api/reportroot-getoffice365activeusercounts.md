---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
ms.openlocfilehash: 1abf72b50e7e6d6654d962757c0d28df967b8694
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011561"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="cee53-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="cee53-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="cee53-104">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="cee53-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="cee53-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="cee53-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="cee53-106">权限</span><span class="sxs-lookup"><span data-stu-id="cee53-106">Permissions</span></span>

<span data-ttu-id="cee53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cee53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cee53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cee53-109">Permission type</span></span>                        | <span data-ttu-id="cee53-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cee53-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cee53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cee53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cee53-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cee53-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cee53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cee53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee53-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cee53-114">Not supported.</span></span>                           |
| <span data-ttu-id="cee53-115">应用</span><span class="sxs-lookup"><span data-stu-id="cee53-115">Application</span></span>                            | <span data-ttu-id="cee53-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cee53-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cee53-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cee53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cee53-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="cee53-118">Function parameters</span></span>

<span data-ttu-id="cee53-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="cee53-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cee53-120">参数</span><span class="sxs-lookup"><span data-stu-id="cee53-120">Parameter</span></span> | <span data-ttu-id="cee53-121">类型</span><span class="sxs-lookup"><span data-stu-id="cee53-121">Type</span></span>   | <span data-ttu-id="cee53-122">说明</span><span class="sxs-lookup"><span data-stu-id="cee53-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cee53-123">period</span><span class="sxs-lookup"><span data-stu-id="cee53-123">period</span></span>    | <span data-ttu-id="cee53-124">string</span><span class="sxs-lookup"><span data-stu-id="cee53-124">string</span></span> | <span data-ttu-id="cee53-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cee53-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cee53-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cee53-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cee53-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cee53-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cee53-128">必需。</span><span class="sxs-lookup"><span data-stu-id="cee53-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cee53-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="cee53-129">Request headers</span></span>

| <span data-ttu-id="cee53-130">名称</span><span class="sxs-lookup"><span data-stu-id="cee53-130">Name</span></span>          | <span data-ttu-id="cee53-131">说明</span><span class="sxs-lookup"><span data-stu-id="cee53-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cee53-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee53-132">Authorization</span></span> | <span data-ttu-id="cee53-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cee53-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cee53-135">响应</span><span class="sxs-lookup"><span data-stu-id="cee53-135">Response</span></span>

<span data-ttu-id="cee53-136">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cee53-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cee53-137">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cee53-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cee53-138">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cee53-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cee53-139">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cee53-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cee53-140">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cee53-140">Report Refresh Date</span></span>
- <span data-ttu-id="cee53-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="cee53-141">Office 365</span></span>
- <span data-ttu-id="cee53-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="cee53-142">Exchange</span></span>
- <span data-ttu-id="cee53-143">OneDrive</span><span class="sxs-lookup"><span data-stu-id="cee53-143">OneDrive</span></span>
- <span data-ttu-id="cee53-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="cee53-144">SharePoint</span></span>
- <span data-ttu-id="cee53-145">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="cee53-145">Skype For Business</span></span> 
- <span data-ttu-id="cee53-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="cee53-146">Yammer</span></span>
- <span data-ttu-id="cee53-147">Teams</span><span class="sxs-lookup"><span data-stu-id="cee53-147">Teams</span></span>
- <span data-ttu-id="cee53-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="cee53-148">Report Date</span></span>
- <span data-ttu-id="cee53-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="cee53-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cee53-150">示例</span><span class="sxs-lookup"><span data-stu-id="cee53-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cee53-151">请求</span><span class="sxs-lookup"><span data-stu-id="cee53-151">Request</span></span>

<span data-ttu-id="cee53-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cee53-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cee53-153">响应</span><span class="sxs-lookup"><span data-stu-id="cee53-153">Response</span></span>

<span data-ttu-id="cee53-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cee53-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="cee53-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cee53-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
