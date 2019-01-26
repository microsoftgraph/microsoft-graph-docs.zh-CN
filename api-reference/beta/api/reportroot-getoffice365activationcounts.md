---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 635b3bf4ff66aee2ea792fa9bfaedd936447ea16
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571413"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="ee8d8-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="ee8d8-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee8d8-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="ee8d8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee8d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee8d8-106">Permissions</span></span>

<span data-ttu-id="ee8d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee8d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee8d8-109">Permission type</span></span>                        | <span data-ttu-id="ee8d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee8d8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee8d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee8d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee8d8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee8d8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee8d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee8d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee8d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-114">Not supported.</span></span>                           |
| <span data-ttu-id="ee8d8-115">应用</span><span class="sxs-lookup"><span data-stu-id="ee8d8-115">Application</span></span>                            | <span data-ttu-id="ee8d8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee8d8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee8d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee8d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="ee8d8-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="ee8d8-118">Query parameters</span></span>

<span data-ttu-id="ee8d8-119">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ee8d8-120">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-120">The default output type is text/csv.</span></span> <span data-ttu-id="ee8d8-121">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee8d8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee8d8-122">Request headers</span></span>

| <span data-ttu-id="ee8d8-123">名称</span><span class="sxs-lookup"><span data-stu-id="ee8d8-123">Name</span></span>          | <span data-ttu-id="ee8d8-124">说明</span><span class="sxs-lookup"><span data-stu-id="ee8d8-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ee8d8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee8d8-125">Authorization</span></span> | <span data-ttu-id="ee8d8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee8d8-128">响应</span><span class="sxs-lookup"><span data-stu-id="ee8d8-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ee8d8-129">CSV</span><span class="sxs-lookup"><span data-stu-id="ee8d8-129">CSV</span></span>

<span data-ttu-id="ee8d8-130">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee8d8-131">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee8d8-132">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee8d8-133">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee8d8-134">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ee8d8-134">Report Refresh Date</span></span>
- <span data-ttu-id="ee8d8-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="ee8d8-135">Product Type</span></span>
- <span data-ttu-id="ee8d8-136">Windows</span><span class="sxs-lookup"><span data-stu-id="ee8d8-136">Windows</span></span>
- <span data-ttu-id="ee8d8-137">Mac</span><span class="sxs-lookup"><span data-stu-id="ee8d8-137">Mac</span></span>
- <span data-ttu-id="ee8d8-138">Android</span><span class="sxs-lookup"><span data-stu-id="ee8d8-138">Android</span></span>
- <span data-ttu-id="ee8d8-139">iOS</span><span class="sxs-lookup"><span data-stu-id="ee8d8-139">iOS</span></span>
- <span data-ttu-id="ee8d8-140">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="ee8d8-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="ee8d8-141">JSON</span><span class="sxs-lookup"><span data-stu-id="ee8d8-141">JSON</span></span>

<span data-ttu-id="ee8d8-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee8d8-143">示例</span><span class="sxs-lookup"><span data-stu-id="ee8d8-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ee8d8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="ee8d8-144">CSV</span></span>

<span data-ttu-id="ee8d8-145">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ee8d8-146">请求</span><span class="sxs-lookup"><span data-stu-id="ee8d8-146">Request</span></span>

<span data-ttu-id="ee8d8-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ee8d8-148">响应</span><span class="sxs-lookup"><span data-stu-id="ee8d8-148">Response</span></span>

<span data-ttu-id="ee8d8-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ee8d8-150">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ee8d8-151">JSON</span><span class="sxs-lookup"><span data-stu-id="ee8d8-151">JSON</span></span>

<span data-ttu-id="ee8d8-152">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ee8d8-153">请求</span><span class="sxs-lookup"><span data-stu-id="ee8d8-153">Request</span></span>

<span data-ttu-id="ee8d8-154">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ee8d8-155">响应</span><span class="sxs-lookup"><span data-stu-id="ee8d8-155">Response</span></span>

<span data-ttu-id="ee8d8-156">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-156">The following example shows the response.</span></span>

> <span data-ttu-id="ee8d8-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ee8d8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
