---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: 获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。 还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 79df65aa3323757bf01ce890303bfa3210d0a7ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972775"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="6e92f-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e92f-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="6e92f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e92f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e92f-106">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="6e92f-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="6e92f-107">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="6e92f-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="6e92f-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-使用的 Skype For business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="6e92f-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e92f-109">权限</span><span class="sxs-lookup"><span data-stu-id="6e92f-109">Permissions</span></span>

<span data-ttu-id="6e92f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e92f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e92f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e92f-112">Permission type</span></span>                        | <span data-ttu-id="6e92f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e92f-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6e92f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e92f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e92f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e92f-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6e92f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e92f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e92f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e92f-117">Not supported.</span></span>                           |
| <span data-ttu-id="6e92f-118">应用</span><span class="sxs-lookup"><span data-stu-id="6e92f-118">Application</span></span>                            | <span data-ttu-id="6e92f-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e92f-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="6e92f-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6e92f-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6e92f-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="6e92f-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6e92f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e92f-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6e92f-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="6e92f-123">Function parameters</span></span>

<span data-ttu-id="6e92f-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6e92f-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6e92f-125">参数</span><span class="sxs-lookup"><span data-stu-id="6e92f-125">Parameter</span></span> | <span data-ttu-id="6e92f-126">类型</span><span class="sxs-lookup"><span data-stu-id="6e92f-126">Type</span></span>   | <span data-ttu-id="6e92f-127">说明</span><span class="sxs-lookup"><span data-stu-id="6e92f-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6e92f-128">period</span><span class="sxs-lookup"><span data-stu-id="6e92f-128">period</span></span>    | <span data-ttu-id="6e92f-129">string</span><span class="sxs-lookup"><span data-stu-id="6e92f-129">string</span></span> | <span data-ttu-id="6e92f-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e92f-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6e92f-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6e92f-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6e92f-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e92f-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6e92f-133">必需。</span><span class="sxs-lookup"><span data-stu-id="6e92f-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6e92f-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e92f-134">Request headers</span></span>

| <span data-ttu-id="6e92f-135">名称</span><span class="sxs-lookup"><span data-stu-id="6e92f-135">Name</span></span>          | <span data-ttu-id="6e92f-136">说明</span><span class="sxs-lookup"><span data-stu-id="6e92f-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6e92f-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e92f-137">Authorization</span></span> | <span data-ttu-id="6e92f-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e92f-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6e92f-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6e92f-140">If-None-Match</span></span> | <span data-ttu-id="6e92f-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e92f-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6e92f-142">可选。</span><span class="sxs-lookup"><span data-stu-id="6e92f-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6e92f-143">响应</span><span class="sxs-lookup"><span data-stu-id="6e92f-143">Response</span></span>

<span data-ttu-id="6e92f-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6e92f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6e92f-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6e92f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6e92f-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6e92f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6e92f-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6e92f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6e92f-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6e92f-148">Report Refresh Date</span></span>
- <span data-ttu-id="6e92f-149">Windows</span><span class="sxs-lookup"><span data-stu-id="6e92f-149">Windows</span></span>
- <span data-ttu-id="6e92f-150">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="6e92f-150">Windows Phone</span></span>
- <span data-ttu-id="6e92f-151">Android 手机</span><span class="sxs-lookup"><span data-stu-id="6e92f-151">Android Phone</span></span>
- <span data-ttu-id="6e92f-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="6e92f-152">iPhone</span></span>
- <span data-ttu-id="6e92f-153">iPad</span><span class="sxs-lookup"><span data-stu-id="6e92f-153">iPad</span></span>
- <span data-ttu-id="6e92f-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="6e92f-154">Report Date</span></span>
- <span data-ttu-id="6e92f-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="6e92f-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6e92f-156">示例</span><span class="sxs-lookup"><span data-stu-id="6e92f-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6e92f-157">请求</span><span class="sxs-lookup"><span data-stu-id="6e92f-157">Request</span></span>

<span data-ttu-id="6e92f-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e92f-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="6e92f-159">响应</span><span class="sxs-lookup"><span data-stu-id="6e92f-159">Response</span></span>

<span data-ttu-id="6e92f-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e92f-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="6e92f-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6e92f-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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

