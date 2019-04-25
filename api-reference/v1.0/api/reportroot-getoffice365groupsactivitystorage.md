---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: 获取跨所有组邮箱和组网站使用的总存储。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a0b752387e55c54ded35b6faf5c87868fad0b2f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582316"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="bb6fc-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="bb6fc-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="bb6fc-104">获取跨所有组邮箱和组网站使用的总存储。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="bb6fc-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb6fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb6fc-106">Permissions</span></span>

<span data-ttu-id="bb6fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb6fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb6fc-109">Permission type</span></span>                        | <span data-ttu-id="bb6fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb6fc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb6fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb6fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb6fc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb6fc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb6fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb6fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb6fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-114">Not supported.</span></span>                           |
| <span data-ttu-id="bb6fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb6fc-115">Application</span></span>                            | <span data-ttu-id="bb6fc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb6fc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb6fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb6fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bb6fc-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="bb6fc-118">Function parameters</span></span>

<span data-ttu-id="bb6fc-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bb6fc-120">参数</span><span class="sxs-lookup"><span data-stu-id="bb6fc-120">Parameter</span></span> | <span data-ttu-id="bb6fc-121">类型</span><span class="sxs-lookup"><span data-stu-id="bb6fc-121">Type</span></span>   | <span data-ttu-id="bb6fc-122">说明</span><span class="sxs-lookup"><span data-stu-id="bb6fc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb6fc-123">period</span><span class="sxs-lookup"><span data-stu-id="bb6fc-123">period</span></span>    | <span data-ttu-id="bb6fc-124">string</span><span class="sxs-lookup"><span data-stu-id="bb6fc-124">string</span></span> | <span data-ttu-id="bb6fc-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb6fc-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb6fc-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bb6fc-128">必需。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bb6fc-129">请求头</span><span class="sxs-lookup"><span data-stu-id="bb6fc-129">Request headers</span></span>

| <span data-ttu-id="bb6fc-130">名称</span><span class="sxs-lookup"><span data-stu-id="bb6fc-130">Name</span></span>          | <span data-ttu-id="bb6fc-131">说明</span><span class="sxs-lookup"><span data-stu-id="bb6fc-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bb6fc-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb6fc-132">Authorization</span></span> | <span data-ttu-id="bb6fc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bb6fc-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bb6fc-135">If-None-Match</span></span> | <span data-ttu-id="bb6fc-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bb6fc-137">可选。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bb6fc-138">响应</span><span class="sxs-lookup"><span data-stu-id="bb6fc-138">Response</span></span>

<span data-ttu-id="bb6fc-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb6fc-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb6fc-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb6fc-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bb6fc-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bb6fc-143">Report Refresh Date</span></span>
- <span data-ttu-id="bb6fc-144">已使用的邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="bb6fc-144">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="bb6fc-145">已使用的网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="bb6fc-145">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="bb6fc-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="bb6fc-146">Report Date</span></span>
- <span data-ttu-id="bb6fc-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="bb6fc-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb6fc-148">示例</span><span class="sxs-lookup"><span data-stu-id="bb6fc-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb6fc-149">请求</span><span class="sxs-lookup"><span data-stu-id="bb6fc-149">Request</span></span>

<span data-ttu-id="bb6fc-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bb6fc-151">响应</span><span class="sxs-lookup"><span data-stu-id="bb6fc-151">Response</span></span>

<span data-ttu-id="bb6fc-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="bb6fc-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bb6fc-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```
