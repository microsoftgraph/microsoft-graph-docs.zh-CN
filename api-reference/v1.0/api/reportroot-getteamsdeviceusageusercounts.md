---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: 按设备类型获取 Microsoft Teams 每日唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2853da7e03b60ebe96013b402e5f32c910552ac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013039"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="05791-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="05791-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="05791-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05791-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05791-105">按设备类型获取 Microsoft Teams 每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="05791-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="05791-106">权限</span><span class="sxs-lookup"><span data-stu-id="05791-106">Permissions</span></span>

<span data-ttu-id="05791-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05791-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05791-109">Permission type</span></span>                        | <span data-ttu-id="05791-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05791-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="05791-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05791-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05791-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05791-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="05791-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05791-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05791-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05791-114">Not supported.</span></span>                           |
| <span data-ttu-id="05791-115">应用</span><span class="sxs-lookup"><span data-stu-id="05791-115">Application</span></span>                            | <span data-ttu-id="05791-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05791-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="05791-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="05791-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="05791-118">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="05791-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="05791-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05791-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="05791-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="05791-120">Function parameters</span></span>

<span data-ttu-id="05791-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="05791-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="05791-122">参数</span><span class="sxs-lookup"><span data-stu-id="05791-122">Parameter</span></span> | <span data-ttu-id="05791-123">类型</span><span class="sxs-lookup"><span data-stu-id="05791-123">Type</span></span>   | <span data-ttu-id="05791-124">说明</span><span class="sxs-lookup"><span data-stu-id="05791-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="05791-125">period</span><span class="sxs-lookup"><span data-stu-id="05791-125">period</span></span>    | <span data-ttu-id="05791-126">string</span><span class="sxs-lookup"><span data-stu-id="05791-126">string</span></span> | <span data-ttu-id="05791-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="05791-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="05791-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="05791-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="05791-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="05791-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="05791-130">必需。</span><span class="sxs-lookup"><span data-stu-id="05791-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="05791-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="05791-131">Request headers</span></span>

| <span data-ttu-id="05791-132">名称</span><span class="sxs-lookup"><span data-stu-id="05791-132">Name</span></span>          | <span data-ttu-id="05791-133">说明</span><span class="sxs-lookup"><span data-stu-id="05791-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="05791-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="05791-134">Authorization</span></span> | <span data-ttu-id="05791-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05791-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="05791-137">响应</span><span class="sxs-lookup"><span data-stu-id="05791-137">Response</span></span>

<span data-ttu-id="05791-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="05791-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="05791-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="05791-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="05791-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="05791-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="05791-141">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="05791-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="05791-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="05791-142">Report Refresh Date</span></span>
- <span data-ttu-id="05791-143">Web</span><span class="sxs-lookup"><span data-stu-id="05791-143">Web</span></span>
- <span data-ttu-id="05791-144">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="05791-144">Windows Phone</span></span>
- <span data-ttu-id="05791-145">Android 手机</span><span class="sxs-lookup"><span data-stu-id="05791-145">Android Phone</span></span>
- <span data-ttu-id="05791-146">iOS</span><span class="sxs-lookup"><span data-stu-id="05791-146">iOS</span></span>
- <span data-ttu-id="05791-147">Mac</span><span class="sxs-lookup"><span data-stu-id="05791-147">Mac</span></span>
- <span data-ttu-id="05791-148">Windows</span><span class="sxs-lookup"><span data-stu-id="05791-148">Windows</span></span>
- <span data-ttu-id="05791-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="05791-149">Report Date</span></span>
- <span data-ttu-id="05791-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="05791-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="05791-151">示例</span><span class="sxs-lookup"><span data-stu-id="05791-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="05791-152">请求</span><span class="sxs-lookup"><span data-stu-id="05791-152">Request</span></span>

<span data-ttu-id="05791-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05791-153">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="05791-154">响应</span><span class="sxs-lookup"><span data-stu-id="05791-154">Response</span></span>

<span data-ttu-id="05791-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05791-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="05791-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="05791-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

