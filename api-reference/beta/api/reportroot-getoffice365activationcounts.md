---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面Microsoft 365激活次数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 21444eddb72e12f52d1ab462e649be87436ff0ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049798"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="42de0-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="42de0-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="42de0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42de0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42de0-105">获取桌面Microsoft 365激活次数。</span><span class="sxs-lookup"><span data-stu-id="42de0-105">Get the count of Microsoft 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="42de0-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。</span><span class="sxs-lookup"><span data-stu-id="42de0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="42de0-107">权限</span><span class="sxs-lookup"><span data-stu-id="42de0-107">Permissions</span></span>

<span data-ttu-id="42de0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42de0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42de0-110">Permission type</span></span>                        | <span data-ttu-id="42de0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42de0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="42de0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42de0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="42de0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42de0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="42de0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42de0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42de0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42de0-115">Not supported.</span></span>                           |
| <span data-ttu-id="42de0-116">应用</span><span class="sxs-lookup"><span data-stu-id="42de0-116">Application</span></span>                            | <span data-ttu-id="42de0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42de0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="42de0-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="42de0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="42de0-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="42de0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="42de0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42de0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="42de0-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="42de0-121">Query parameters</span></span>

<span data-ttu-id="42de0-122">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="42de0-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="42de0-123">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="42de0-123">The default output type is text/csv.</span></span> <span data-ttu-id="42de0-124">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="42de0-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42de0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="42de0-125">Request headers</span></span>

| <span data-ttu-id="42de0-126">名称</span><span class="sxs-lookup"><span data-stu-id="42de0-126">Name</span></span>          | <span data-ttu-id="42de0-127">说明</span><span class="sxs-lookup"><span data-stu-id="42de0-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="42de0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="42de0-128">Authorization</span></span> | <span data-ttu-id="42de0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42de0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="42de0-131">响应</span><span class="sxs-lookup"><span data-stu-id="42de0-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="42de0-132">CSV</span><span class="sxs-lookup"><span data-stu-id="42de0-132">CSV</span></span>

<span data-ttu-id="42de0-133">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="42de0-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="42de0-134">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="42de0-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="42de0-135">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="42de0-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="42de0-136">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="42de0-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="42de0-137">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="42de0-137">Report Refresh Date</span></span>
- <span data-ttu-id="42de0-138">产品类型</span><span class="sxs-lookup"><span data-stu-id="42de0-138">Product Type</span></span>
- <span data-ttu-id="42de0-139">Windows</span><span class="sxs-lookup"><span data-stu-id="42de0-139">Windows</span></span>
- <span data-ttu-id="42de0-140">Mac</span><span class="sxs-lookup"><span data-stu-id="42de0-140">Mac</span></span>
- <span data-ttu-id="42de0-141">Android</span><span class="sxs-lookup"><span data-stu-id="42de0-141">Android</span></span>
- <span data-ttu-id="42de0-142">iOS</span><span class="sxs-lookup"><span data-stu-id="42de0-142">iOS</span></span>
- <span data-ttu-id="42de0-143">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="42de0-143">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="42de0-144">JSON</span><span class="sxs-lookup"><span data-stu-id="42de0-144">JSON</span></span>

<span data-ttu-id="42de0-145">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="42de0-145">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42de0-146">示例</span><span class="sxs-lookup"><span data-stu-id="42de0-146">Example</span></span>

### <a name="csv"></a><span data-ttu-id="42de0-147">CSV</span><span class="sxs-lookup"><span data-stu-id="42de0-147">CSV</span></span>

<span data-ttu-id="42de0-148">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="42de0-148">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="42de0-149">请求</span><span class="sxs-lookup"><span data-stu-id="42de0-149">Request</span></span>

<span data-ttu-id="42de0-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42de0-150">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="42de0-151">响应</span><span class="sxs-lookup"><span data-stu-id="42de0-151">Response</span></span>

<span data-ttu-id="42de0-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="42de0-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="42de0-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="42de0-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="42de0-154">JSON</span><span class="sxs-lookup"><span data-stu-id="42de0-154">JSON</span></span>

<span data-ttu-id="42de0-155">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="42de0-155">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="42de0-156">请求</span><span class="sxs-lookup"><span data-stu-id="42de0-156">Request</span></span>

<span data-ttu-id="42de0-157">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="42de0-157">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="42de0-158">响应</span><span class="sxs-lookup"><span data-stu-id="42de0-158">Response</span></span>

<span data-ttu-id="42de0-159">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="42de0-159">The following example shows the response.</span></span>

> <span data-ttu-id="42de0-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="42de0-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Microsoft 365 Apps for enterprise", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
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


