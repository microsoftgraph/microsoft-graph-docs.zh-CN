---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fa3b451e95194ce446934530b36baaba0cb2ed47
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897405"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="e383e-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="e383e-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="e383e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e383e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e383e-105">获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。</span><span class="sxs-lookup"><span data-stu-id="e383e-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="e383e-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="e383e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="e383e-107">权限</span><span class="sxs-lookup"><span data-stu-id="e383e-107">Permissions</span></span>

<span data-ttu-id="e383e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e383e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e383e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e383e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e383e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e383e-110">Permission type</span></span>                        | <span data-ttu-id="e383e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e383e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e383e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e383e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e383e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e383e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e383e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e383e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e383e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e383e-115">Not supported.</span></span>                           |
| <span data-ttu-id="e383e-116">应用</span><span class="sxs-lookup"><span data-stu-id="e383e-116">Application</span></span>                            | <span data-ttu-id="e383e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e383e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e383e-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e383e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e383e-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="e383e-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e383e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e383e-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="e383e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e383e-121">Request headers</span></span>

| <span data-ttu-id="e383e-122">名称</span><span class="sxs-lookup"><span data-stu-id="e383e-122">Name</span></span>          | <span data-ttu-id="e383e-123">说明</span><span class="sxs-lookup"><span data-stu-id="e383e-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e383e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e383e-124">Authorization</span></span> | <span data-ttu-id="e383e-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e383e-125">Bearer {token}.</span></span> <span data-ttu-id="e383e-126">Required.</span><span class="sxs-lookup"><span data-stu-id="e383e-126">Required.</span></span>                |
| <span data-ttu-id="e383e-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e383e-127">If-None-Match</span></span> | <span data-ttu-id="e383e-128">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e383e-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e383e-129">可选。</span><span class="sxs-lookup"><span data-stu-id="e383e-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e383e-130">响应</span><span class="sxs-lookup"><span data-stu-id="e383e-130">Response</span></span>

<span data-ttu-id="e383e-131">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e383e-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e383e-132">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e383e-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e383e-133">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e383e-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e383e-134">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e383e-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e383e-135">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e383e-135">Report Refresh Date</span></span>
- <span data-ttu-id="e383e-136">产品类型</span><span class="sxs-lookup"><span data-stu-id="e383e-136">Product Type</span></span>
- <span data-ttu-id="e383e-137">已分配</span><span class="sxs-lookup"><span data-stu-id="e383e-137">Assigned</span></span>
- <span data-ttu-id="e383e-138">已激活</span><span class="sxs-lookup"><span data-stu-id="e383e-138">Activated</span></span>
- <span data-ttu-id="e383e-139">共享计算机激活</span><span class="sxs-lookup"><span data-stu-id="e383e-139">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="e383e-140">示例</span><span class="sxs-lookup"><span data-stu-id="e383e-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e383e-141">请求</span><span class="sxs-lookup"><span data-stu-id="e383e-141">Request</span></span>

<span data-ttu-id="e383e-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e383e-142">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```


#### <a name="response"></a><span data-ttu-id="e383e-143">响应</span><span class="sxs-lookup"><span data-stu-id="e383e-143">Response</span></span>

<span data-ttu-id="e383e-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e383e-144">The following is an example of the response.</span></span>

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

<span data-ttu-id="e383e-145">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e383e-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
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
