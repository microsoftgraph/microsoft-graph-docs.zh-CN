---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 5eec54e07b4f5cfc8bdb4f5c0f24c6988ef38007
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983104"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="07267-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="07267-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="07267-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07267-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07267-106">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="07267-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="07267-107">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="07267-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="07267-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="07267-108">Permissions</span></span>

<span data-ttu-id="07267-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07267-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07267-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07267-111">Permission type</span></span>                        | <span data-ttu-id="07267-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07267-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="07267-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07267-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="07267-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="07267-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="07267-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07267-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07267-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07267-116">Not supported.</span></span>                           |
| <span data-ttu-id="07267-117">应用</span><span class="sxs-lookup"><span data-stu-id="07267-117">Application</span></span>                            | <span data-ttu-id="07267-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="07267-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="07267-119">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="07267-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="07267-120">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="07267-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="07267-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07267-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="07267-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="07267-122">Function parameters</span></span>

<span data-ttu-id="07267-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="07267-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="07267-124">参数</span><span class="sxs-lookup"><span data-stu-id="07267-124">Parameter</span></span> | <span data-ttu-id="07267-125">类型</span><span class="sxs-lookup"><span data-stu-id="07267-125">Type</span></span>   | <span data-ttu-id="07267-126">说明</span><span class="sxs-lookup"><span data-stu-id="07267-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="07267-127">period</span><span class="sxs-lookup"><span data-stu-id="07267-127">period</span></span>    | <span data-ttu-id="07267-128">string</span><span class="sxs-lookup"><span data-stu-id="07267-128">string</span></span> | <span data-ttu-id="07267-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="07267-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="07267-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="07267-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="07267-131">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="07267-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="07267-132">必需。</span><span class="sxs-lookup"><span data-stu-id="07267-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="07267-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="07267-133">Request headers</span></span>

| <span data-ttu-id="07267-134">名称</span><span class="sxs-lookup"><span data-stu-id="07267-134">Name</span></span>          | <span data-ttu-id="07267-135">说明</span><span class="sxs-lookup"><span data-stu-id="07267-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="07267-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="07267-136">Authorization</span></span> | <span data-ttu-id="07267-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07267-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="07267-139">响应</span><span class="sxs-lookup"><span data-stu-id="07267-139">Response</span></span>

<span data-ttu-id="07267-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="07267-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="07267-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="07267-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="07267-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="07267-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="07267-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="07267-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="07267-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="07267-144">Report Refresh Date</span></span>
- <span data-ttu-id="07267-145">报表日期</span><span class="sxs-lookup"><span data-stu-id="07267-145">Report Date</span></span>
- <span data-ttu-id="07267-146">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="07267-146">Team Chat Messages</span></span>
- <span data-ttu-id="07267-147">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="07267-147">Private Chat Messages</span></span>
- <span data-ttu-id="07267-148">呼叫</span><span class="sxs-lookup"><span data-stu-id="07267-148">Calls</span></span>
- <span data-ttu-id="07267-149">会议</span><span class="sxs-lookup"><span data-stu-id="07267-149">Meetings</span></span>
- <span data-ttu-id="07267-150">其他操作</span><span class="sxs-lookup"><span data-stu-id="07267-150">Other Actions</span></span>
- <span data-ttu-id="07267-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="07267-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="07267-152">示例</span><span class="sxs-lookup"><span data-stu-id="07267-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="07267-153">请求</span><span class="sxs-lookup"><span data-stu-id="07267-153">Request</span></span>

<span data-ttu-id="07267-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07267-154">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="07267-155">响应</span><span class="sxs-lookup"><span data-stu-id="07267-155">Response</span></span>

<span data-ttu-id="07267-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07267-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="07267-157">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="07267-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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

