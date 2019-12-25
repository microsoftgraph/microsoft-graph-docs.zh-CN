---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 067641f5c44f24b86e1e41f7474bcd29d597a449
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865431"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="574a7-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="574a7-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="574a7-104">获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。</span><span class="sxs-lookup"><span data-stu-id="574a7-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="574a7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="574a7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="574a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="574a7-106">Permissions</span></span>

<span data-ttu-id="574a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="574a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="574a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="574a7-109">Permission type</span></span>                        | <span data-ttu-id="574a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="574a7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="574a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="574a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="574a7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="574a7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="574a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="574a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="574a7-114">Not supported.</span></span>                           |
| <span data-ttu-id="574a7-115">应用</span><span class="sxs-lookup"><span data-stu-id="574a7-115">Application</span></span>                            | <span data-ttu-id="574a7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="574a7-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="574a7-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="574a7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="574a7-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="574a7-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="574a7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="574a7-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="574a7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="574a7-120">Request headers</span></span>

| <span data-ttu-id="574a7-121">名称</span><span class="sxs-lookup"><span data-stu-id="574a7-121">Name</span></span>          | <span data-ttu-id="574a7-122">说明</span><span class="sxs-lookup"><span data-stu-id="574a7-122">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="574a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="574a7-123">Authorization</span></span> | <span data-ttu-id="574a7-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="574a7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="574a7-126">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="574a7-126">If-None-Match</span></span> | <span data-ttu-id="574a7-127">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="574a7-127">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="574a7-128">可选。</span><span class="sxs-lookup"><span data-stu-id="574a7-128">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="574a7-129">响应</span><span class="sxs-lookup"><span data-stu-id="574a7-129">Response</span></span>

<span data-ttu-id="574a7-130">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="574a7-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="574a7-131">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="574a7-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="574a7-132">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="574a7-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="574a7-133">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="574a7-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="574a7-134">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="574a7-134">Report Refresh Date</span></span>
- <span data-ttu-id="574a7-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="574a7-135">Product Type</span></span>
- <span data-ttu-id="574a7-136">已分配</span><span class="sxs-lookup"><span data-stu-id="574a7-136">Assigned</span></span>
- <span data-ttu-id="574a7-137">已激活</span><span class="sxs-lookup"><span data-stu-id="574a7-137">Activated</span></span>
- <span data-ttu-id="574a7-138">共享计算机激活</span><span class="sxs-lookup"><span data-stu-id="574a7-138">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="574a7-139">示例</span><span class="sxs-lookup"><span data-stu-id="574a7-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="574a7-140">请求</span><span class="sxs-lookup"><span data-stu-id="574a7-140">Request</span></span>

<span data-ttu-id="574a7-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="574a7-141">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="574a7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="574a7-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="574a7-143">C#</span><span class="sxs-lookup"><span data-stu-id="574a7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="574a7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="574a7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="574a7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="574a7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="574a7-146">Java</span><span class="sxs-lookup"><span data-stu-id="574a7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="574a7-147">响应</span><span class="sxs-lookup"><span data-stu-id="574a7-147">Response</span></span>

<span data-ttu-id="574a7-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="574a7-148">The following is an example of the response.</span></span>

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

<span data-ttu-id="574a7-149">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="574a7-149">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
