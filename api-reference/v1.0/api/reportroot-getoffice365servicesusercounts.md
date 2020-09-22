---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c59b34fdb961cdf189a621335aa1a47b036bb9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015685"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="f8452-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="f8452-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="f8452-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8452-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8452-105">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="f8452-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="f8452-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="f8452-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8452-107">权限</span><span class="sxs-lookup"><span data-stu-id="f8452-107">Permissions</span></span>

<span data-ttu-id="f8452-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8452-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8452-110">Permission type</span></span>                        | <span data-ttu-id="f8452-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8452-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8452-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8452-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8452-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8452-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f8452-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8452-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8452-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8452-115">Not supported.</span></span>                           |
| <span data-ttu-id="f8452-116">应用</span><span class="sxs-lookup"><span data-stu-id="f8452-116">Application</span></span>                            | <span data-ttu-id="f8452-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8452-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="f8452-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f8452-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f8452-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="f8452-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f8452-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8452-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f8452-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="f8452-121">Function parameters</span></span>

<span data-ttu-id="f8452-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f8452-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f8452-123">参数</span><span class="sxs-lookup"><span data-stu-id="f8452-123">Parameter</span></span> | <span data-ttu-id="f8452-124">类型</span><span class="sxs-lookup"><span data-stu-id="f8452-124">Type</span></span>   | <span data-ttu-id="f8452-125">说明</span><span class="sxs-lookup"><span data-stu-id="f8452-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8452-126">period</span><span class="sxs-lookup"><span data-stu-id="f8452-126">period</span></span>    | <span data-ttu-id="f8452-127">string</span><span class="sxs-lookup"><span data-stu-id="f8452-127">string</span></span> | <span data-ttu-id="f8452-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8452-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8452-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f8452-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8452-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8452-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8452-131">必需。</span><span class="sxs-lookup"><span data-stu-id="f8452-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f8452-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8452-132">Request headers</span></span>

| <span data-ttu-id="f8452-133">名称</span><span class="sxs-lookup"><span data-stu-id="f8452-133">Name</span></span>          | <span data-ttu-id="f8452-134">说明</span><span class="sxs-lookup"><span data-stu-id="f8452-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f8452-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8452-135">Authorization</span></span> | <span data-ttu-id="f8452-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8452-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f8452-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f8452-138">If-None-Match</span></span> | <span data-ttu-id="f8452-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f8452-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f8452-140">可选。</span><span class="sxs-lookup"><span data-stu-id="f8452-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f8452-141">响应</span><span class="sxs-lookup"><span data-stu-id="f8452-141">Response</span></span>

<span data-ttu-id="f8452-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f8452-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8452-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f8452-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8452-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f8452-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f8452-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f8452-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8452-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f8452-146">Report Refresh Date</span></span>
- <span data-ttu-id="f8452-147">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-147">Exchange Active</span></span>
- <span data-ttu-id="f8452-148">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-148">Exchange Inactive</span></span>
- <span data-ttu-id="f8452-149">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-149">OneDrive Active</span></span>
- <span data-ttu-id="f8452-150">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-150">OneDrive Inactive</span></span>
- <span data-ttu-id="f8452-151">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-151">SharePoint Active</span></span>
- <span data-ttu-id="f8452-152">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-152">SharePoint Inactive</span></span>
- <span data-ttu-id="f8452-153">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-153">Skype For Business Active</span></span>
- <span data-ttu-id="f8452-154">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="f8452-155">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-155">Yammer Active</span></span>
- <span data-ttu-id="f8452-156">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-156">Yammer Inactive</span></span>
- <span data-ttu-id="f8452-157">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-157">Teams Active</span></span>
- <span data-ttu-id="f8452-158">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8452-158">Teams Inactive</span></span>
- <span data-ttu-id="f8452-159">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="f8452-159">Office 365 Active</span></span>
- <span data-ttu-id="f8452-160">Office 365 非活动</span><span class="sxs-lookup"><span data-stu-id="f8452-160">Office 365 Inactive</span></span>
- <span data-ttu-id="f8452-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="f8452-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f8452-162">示例</span><span class="sxs-lookup"><span data-stu-id="f8452-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8452-163">请求</span><span class="sxs-lookup"><span data-stu-id="f8452-163">Request</span></span>

<span data-ttu-id="f8452-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8452-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="f8452-165">响应</span><span class="sxs-lookup"><span data-stu-id="f8452-165">Response</span></span>

<span data-ttu-id="f8452-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8452-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="f8452-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f8452-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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

