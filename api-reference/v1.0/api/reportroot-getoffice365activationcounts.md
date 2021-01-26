---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上 Microsoft 365 激活的计数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: dd33f734adc5a01b2f86909a7e0d7535740fa151
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981786"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="2658d-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="2658d-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="2658d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2658d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2658d-105">获取桌面和设备上 Microsoft 365 激活的计数。</span><span class="sxs-lookup"><span data-stu-id="2658d-105">Get the count of Microsoft 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="2658d-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。</span><span class="sxs-lookup"><span data-stu-id="2658d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2658d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2658d-107">Permissions</span></span>

<span data-ttu-id="2658d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2658d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2658d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2658d-110">Permission type</span></span>                        | <span data-ttu-id="2658d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2658d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2658d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2658d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2658d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2658d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2658d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2658d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2658d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2658d-115">Not supported.</span></span>                           |
| <span data-ttu-id="2658d-116">应用</span><span class="sxs-lookup"><span data-stu-id="2658d-116">Application</span></span>                            | <span data-ttu-id="2658d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2658d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="2658d-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="2658d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2658d-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="2658d-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2658d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2658d-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="2658d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2658d-121">Request headers</span></span>

| <span data-ttu-id="2658d-122">名称</span><span class="sxs-lookup"><span data-stu-id="2658d-122">Name</span></span>          | <span data-ttu-id="2658d-123">说明</span><span class="sxs-lookup"><span data-stu-id="2658d-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2658d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2658d-124">Authorization</span></span> | <span data-ttu-id="2658d-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2658d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2658d-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2658d-127">If-None-Match</span></span> | <span data-ttu-id="2658d-128">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2658d-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2658d-129">可选。</span><span class="sxs-lookup"><span data-stu-id="2658d-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2658d-130">响应</span><span class="sxs-lookup"><span data-stu-id="2658d-130">Response</span></span>

<span data-ttu-id="2658d-131">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2658d-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2658d-132">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2658d-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2658d-133">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2658d-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2658d-134">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2658d-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2658d-135">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2658d-135">Report Refresh Date</span></span>
- <span data-ttu-id="2658d-136">产品类型</span><span class="sxs-lookup"><span data-stu-id="2658d-136">Product Type</span></span>
- <span data-ttu-id="2658d-137">Windows</span><span class="sxs-lookup"><span data-stu-id="2658d-137">Windows</span></span>
- <span data-ttu-id="2658d-138">Mac</span><span class="sxs-lookup"><span data-stu-id="2658d-138">Mac</span></span>
- <span data-ttu-id="2658d-139">Android</span><span class="sxs-lookup"><span data-stu-id="2658d-139">Android</span></span>
- <span data-ttu-id="2658d-140">iOS</span><span class="sxs-lookup"><span data-stu-id="2658d-140">iOS</span></span>
- <span data-ttu-id="2658d-141">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="2658d-141">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="2658d-142">示例</span><span class="sxs-lookup"><span data-stu-id="2658d-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2658d-143">请求</span><span class="sxs-lookup"><span data-stu-id="2658d-143">Request</span></span>

<span data-ttu-id="2658d-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2658d-144">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```


#### <a name="response"></a><span data-ttu-id="2658d-145">响应</span><span class="sxs-lookup"><span data-stu-id="2658d-145">Response</span></span>

<span data-ttu-id="2658d-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2658d-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="2658d-147">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2658d-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
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

