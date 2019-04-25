---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4684458b0b7198dcdc1657935c5641a2928d6c22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580867"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="77a46-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="77a46-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="77a46-105">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="77a46-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="77a46-106">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="77a46-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="77a46-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="77a46-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="77a46-108">权限</span><span class="sxs-lookup"><span data-stu-id="77a46-108">Permissions</span></span>

<span data-ttu-id="77a46-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77a46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77a46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77a46-111">Permission type</span></span>                        | <span data-ttu-id="77a46-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77a46-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="77a46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77a46-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="77a46-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="77a46-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="77a46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77a46-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a46-116">Not supported.</span></span>                           |
| <span data-ttu-id="77a46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77a46-117">Application</span></span>                            | <span data-ttu-id="77a46-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="77a46-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="77a46-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77a46-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="77a46-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="77a46-120">Function parameters</span></span>

<span data-ttu-id="77a46-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="77a46-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="77a46-122">参数</span><span class="sxs-lookup"><span data-stu-id="77a46-122">Parameter</span></span> | <span data-ttu-id="77a46-123">类型</span><span class="sxs-lookup"><span data-stu-id="77a46-123">Type</span></span>   | <span data-ttu-id="77a46-124">说明</span><span class="sxs-lookup"><span data-stu-id="77a46-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="77a46-125">period</span><span class="sxs-lookup"><span data-stu-id="77a46-125">period</span></span>    | <span data-ttu-id="77a46-126">string</span><span class="sxs-lookup"><span data-stu-id="77a46-126">string</span></span> | <span data-ttu-id="77a46-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="77a46-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="77a46-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="77a46-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="77a46-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="77a46-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="77a46-130">必需。</span><span class="sxs-lookup"><span data-stu-id="77a46-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="77a46-131">请求头</span><span class="sxs-lookup"><span data-stu-id="77a46-131">Request headers</span></span>

| <span data-ttu-id="77a46-132">名称</span><span class="sxs-lookup"><span data-stu-id="77a46-132">Name</span></span>          | <span data-ttu-id="77a46-133">说明</span><span class="sxs-lookup"><span data-stu-id="77a46-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="77a46-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a46-134">Authorization</span></span> | <span data-ttu-id="77a46-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77a46-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="77a46-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="77a46-137">If-None-Match</span></span> | <span data-ttu-id="77a46-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="77a46-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="77a46-139">可选。</span><span class="sxs-lookup"><span data-stu-id="77a46-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="77a46-140">响应</span><span class="sxs-lookup"><span data-stu-id="77a46-140">Response</span></span>

<span data-ttu-id="77a46-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="77a46-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="77a46-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="77a46-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="77a46-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="77a46-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="77a46-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="77a46-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="77a46-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="77a46-145">Report Refresh Date</span></span>
- <span data-ttu-id="77a46-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="77a46-146">Report Date</span></span>
- <span data-ttu-id="77a46-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="77a46-147">Report Period</span></span>
- <span data-ttu-id="77a46-148">IM</span><span class="sxs-lookup"><span data-stu-id="77a46-148">IM</span></span>
- <span data-ttu-id="77a46-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="77a46-149">Audio/Video</span></span>
- <span data-ttu-id="77a46-150">应用共享</span><span class="sxs-lookup"><span data-stu-id="77a46-150">App Sharing</span></span>
- <span data-ttu-id="77a46-151">Web</span><span class="sxs-lookup"><span data-stu-id="77a46-151">Web</span></span>
- <span data-ttu-id="77a46-152">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="77a46-152">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="77a46-153">示例</span><span class="sxs-lookup"><span data-stu-id="77a46-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="77a46-154">请求</span><span class="sxs-lookup"><span data-stu-id="77a46-154">Request</span></span>

<span data-ttu-id="77a46-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77a46-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="77a46-156">响应</span><span class="sxs-lookup"><span data-stu-id="77a46-156">Response</span></span>

<span data-ttu-id="77a46-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77a46-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="77a46-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="77a46-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```
