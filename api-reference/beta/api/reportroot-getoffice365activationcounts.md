---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 635b3bf4ff66aee2ea792fa9bfaedd936447ea16
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545912"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="e0ddb-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="e0ddb-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ddb-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="e0ddb-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ddb-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0ddb-106">Permissions</span></span>

<span data-ttu-id="e0ddb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0ddb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0ddb-109">Permission type</span></span>                        | <span data-ttu-id="e0ddb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0ddb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e0ddb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ddb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0ddb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0ddb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e0ddb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ddb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ddb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-114">Not supported.</span></span>                           |
| <span data-ttu-id="e0ddb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0ddb-115">Application</span></span>                            | <span data-ttu-id="e0ddb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0ddb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e0ddb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0ddb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="e0ddb-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="e0ddb-118">Query parameters</span></span>

<span data-ttu-id="e0ddb-119">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e0ddb-120">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-120">The default output type is text/csv.</span></span> <span data-ttu-id="e0ddb-121">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0ddb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0ddb-122">Request headers</span></span>

| <span data-ttu-id="e0ddb-123">名称</span><span class="sxs-lookup"><span data-stu-id="e0ddb-123">Name</span></span>          | <span data-ttu-id="e0ddb-124">说明</span><span class="sxs-lookup"><span data-stu-id="e0ddb-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e0ddb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0ddb-125">Authorization</span></span> | <span data-ttu-id="e0ddb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0ddb-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0ddb-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e0ddb-129">CSV</span><span class="sxs-lookup"><span data-stu-id="e0ddb-129">CSV</span></span>

<span data-ttu-id="e0ddb-130">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e0ddb-131">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e0ddb-132">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e0ddb-133">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e0ddb-134">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e0ddb-134">Report Refresh Date</span></span>
- <span data-ttu-id="e0ddb-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="e0ddb-135">Product Type</span></span>
- <span data-ttu-id="e0ddb-136">Windows</span><span class="sxs-lookup"><span data-stu-id="e0ddb-136">Windows</span></span>
- <span data-ttu-id="e0ddb-137">Mac</span><span class="sxs-lookup"><span data-stu-id="e0ddb-137">Mac</span></span>
- <span data-ttu-id="e0ddb-138">Android</span><span class="sxs-lookup"><span data-stu-id="e0ddb-138">Android</span></span>
- <span data-ttu-id="e0ddb-139">iOS</span><span class="sxs-lookup"><span data-stu-id="e0ddb-139">iOS</span></span>
- <span data-ttu-id="e0ddb-140">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="e0ddb-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="e0ddb-141">JSON</span><span class="sxs-lookup"><span data-stu-id="e0ddb-141">JSON</span></span>

<span data-ttu-id="e0ddb-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ddb-143">示例</span><span class="sxs-lookup"><span data-stu-id="e0ddb-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e0ddb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e0ddb-144">CSV</span></span>

<span data-ttu-id="e0ddb-145">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e0ddb-146">请求</span><span class="sxs-lookup"><span data-stu-id="e0ddb-146">Request</span></span>

<span data-ttu-id="e0ddb-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e0ddb-148">响应</span><span class="sxs-lookup"><span data-stu-id="e0ddb-148">Response</span></span>

<span data-ttu-id="e0ddb-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e0ddb-150">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e0ddb-151">JSON</span><span class="sxs-lookup"><span data-stu-id="e0ddb-151">JSON</span></span>

<span data-ttu-id="e0ddb-152">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e0ddb-153">请求</span><span class="sxs-lookup"><span data-stu-id="e0ddb-153">Request</span></span>

<span data-ttu-id="e0ddb-154">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e0ddb-155">响应</span><span class="sxs-lookup"><span data-stu-id="e0ddb-155">Response</span></span>

<span data-ttu-id="e0ddb-156">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-156">The following example shows the response.</span></span>

> <span data-ttu-id="e0ddb-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0ddb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
