---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 要获取的已启用的用户和那些必须激活桌面或设备上的 Office 订阅或共享计算机的计数。
ms.openlocfilehash: f46d3e01e7eeb212ea50675bbcf7371e4af2ec40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008916"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="be4f4-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="be4f4-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="be4f4-104">要获取的已启用的用户和那些必须激活桌面或设备上的 Office 订阅或共享计算机的计数。</span><span class="sxs-lookup"><span data-stu-id="be4f4-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="be4f4-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="be4f4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="be4f4-106">权限</span><span class="sxs-lookup"><span data-stu-id="be4f4-106">Permissions</span></span>

<span data-ttu-id="be4f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be4f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be4f4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be4f4-109">Permission type</span></span>                        | <span data-ttu-id="be4f4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be4f4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="be4f4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be4f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be4f4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be4f4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="be4f4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be4f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be4f4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be4f4-114">Not supported.</span></span>                           |
| <span data-ttu-id="be4f4-115">应用</span><span class="sxs-lookup"><span data-stu-id="be4f4-115">Application</span></span>                            | <span data-ttu-id="be4f4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="be4f4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="be4f4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be4f4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="be4f4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be4f4-118">Request headers</span></span>

| <span data-ttu-id="be4f4-119">名称</span><span class="sxs-lookup"><span data-stu-id="be4f4-119">Name</span></span>          | <span data-ttu-id="be4f4-120">说明</span><span class="sxs-lookup"><span data-stu-id="be4f4-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="be4f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4f4-121">Authorization</span></span> | <span data-ttu-id="be4f4-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="be4f4-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="be4f4-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="be4f4-124">If-None-Match</span></span> | <span data-ttu-id="be4f4-125">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="be4f4-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="be4f4-126">可选。</span><span class="sxs-lookup"><span data-stu-id="be4f4-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="be4f4-127">响应</span><span class="sxs-lookup"><span data-stu-id="be4f4-127">Response</span></span>

<span data-ttu-id="be4f4-128">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="be4f4-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="be4f4-129">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="be4f4-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="be4f4-130">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="be4f4-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="be4f4-131">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="be4f4-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="be4f4-132">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="be4f4-132">Report Refresh Date</span></span>
- <span data-ttu-id="be4f4-133">产品类型</span><span class="sxs-lookup"><span data-stu-id="be4f4-133">Product Type</span></span>
- <span data-ttu-id="be4f4-134">已分配</span><span class="sxs-lookup"><span data-stu-id="be4f4-134">Assigned</span></span>
- <span data-ttu-id="be4f4-135">已激活</span><span class="sxs-lookup"><span data-stu-id="be4f4-135">Activated</span></span>
- <span data-ttu-id="be4f4-136">共享的计算机激活</span><span class="sxs-lookup"><span data-stu-id="be4f4-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="be4f4-137">示例</span><span class="sxs-lookup"><span data-stu-id="be4f4-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="be4f4-138">请求</span><span class="sxs-lookup"><span data-stu-id="be4f4-138">Request</span></span>

<span data-ttu-id="be4f4-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be4f4-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="be4f4-140">响应</span><span class="sxs-lookup"><span data-stu-id="be4f4-140">Response</span></span>

<span data-ttu-id="be4f4-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be4f4-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="be4f4-142">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="be4f4-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
