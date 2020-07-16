---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 39f6ac1380c80052af236f44cd518004088a2e8e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895921"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="93e4c-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="93e4c-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="93e4c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e4c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93e4c-106">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="93e4c-106">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="93e4c-107">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="93e4c-107">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="93e4c-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-使用的 Skype For business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="93e4c-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="93e4c-109">权限</span><span class="sxs-lookup"><span data-stu-id="93e4c-109">Permissions</span></span>

<span data-ttu-id="93e4c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93e4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93e4c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="93e4c-112">Permission type</span></span>                        | <span data-ttu-id="93e4c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93e4c-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="93e4c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93e4c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="93e4c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93e4c-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="93e4c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93e4c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e4c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="93e4c-117">Not supported.</span></span>                           |
| <span data-ttu-id="93e4c-118">应用</span><span class="sxs-lookup"><span data-stu-id="93e4c-118">Application</span></span>                            | <span data-ttu-id="93e4c-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93e4c-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="93e4c-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="93e4c-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="93e4c-121">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="93e4c-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="93e4c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93e4c-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="93e4c-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="93e4c-123">Function parameters</span></span>

<span data-ttu-id="93e4c-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="93e4c-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="93e4c-125">参数</span><span class="sxs-lookup"><span data-stu-id="93e4c-125">Parameter</span></span> | <span data-ttu-id="93e4c-126">类型</span><span class="sxs-lookup"><span data-stu-id="93e4c-126">Type</span></span>   | <span data-ttu-id="93e4c-127">说明</span><span class="sxs-lookup"><span data-stu-id="93e4c-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="93e4c-128">period</span><span class="sxs-lookup"><span data-stu-id="93e4c-128">period</span></span>    | <span data-ttu-id="93e4c-129">string</span><span class="sxs-lookup"><span data-stu-id="93e4c-129">string</span></span> | <span data-ttu-id="93e4c-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="93e4c-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="93e4c-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="93e4c-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="93e4c-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="93e4c-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="93e4c-133">必需。</span><span class="sxs-lookup"><span data-stu-id="93e4c-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="93e4c-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="93e4c-134">Request headers</span></span>

| <span data-ttu-id="93e4c-135">名称</span><span class="sxs-lookup"><span data-stu-id="93e4c-135">Name</span></span>          | <span data-ttu-id="93e4c-136">说明</span><span class="sxs-lookup"><span data-stu-id="93e4c-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="93e4c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="93e4c-137">Authorization</span></span> | <span data-ttu-id="93e4c-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="93e4c-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="93e4c-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="93e4c-140">If-None-Match</span></span> | <span data-ttu-id="93e4c-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="93e4c-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="93e4c-142">可选。</span><span class="sxs-lookup"><span data-stu-id="93e4c-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="93e4c-143">响应</span><span class="sxs-lookup"><span data-stu-id="93e4c-143">Response</span></span>

<span data-ttu-id="93e4c-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="93e4c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="93e4c-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="93e4c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="93e4c-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="93e4c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="93e4c-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="93e4c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="93e4c-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="93e4c-148">Report Refresh Date</span></span>
- <span data-ttu-id="93e4c-149">Windows</span><span class="sxs-lookup"><span data-stu-id="93e4c-149">Windows</span></span>
- <span data-ttu-id="93e4c-150">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="93e4c-150">Windows Phone</span></span>
- <span data-ttu-id="93e4c-151">Android 手机</span><span class="sxs-lookup"><span data-stu-id="93e4c-151">Android Phone</span></span>
- <span data-ttu-id="93e4c-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="93e4c-152">iPhone</span></span>
- <span data-ttu-id="93e4c-153">iPad</span><span class="sxs-lookup"><span data-stu-id="93e4c-153">iPad</span></span>
- <span data-ttu-id="93e4c-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="93e4c-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="93e4c-155">示例</span><span class="sxs-lookup"><span data-stu-id="93e4c-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="93e4c-156">请求</span><span class="sxs-lookup"><span data-stu-id="93e4c-156">Request</span></span>

<span data-ttu-id="93e4c-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="93e4c-157">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="93e4c-158">响应</span><span class="sxs-lookup"><span data-stu-id="93e4c-158">Response</span></span>

<span data-ttu-id="93e4c-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="93e4c-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="93e4c-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="93e4c-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
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
