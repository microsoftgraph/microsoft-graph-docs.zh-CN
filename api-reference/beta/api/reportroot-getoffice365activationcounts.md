---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.openlocfilehash: aff0459cc1ea88fb67d182cdfdbd4e0536619bea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855956"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="b8d9b-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="b8d9b-103">reportRoot: getOffice365ActivationCounts</span></span>

> <span data-ttu-id="b8d9b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8d9b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8d9b-106">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-106">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="b8d9b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8d9b-108">权限</span><span class="sxs-lookup"><span data-stu-id="b8d9b-108">Permissions</span></span>

<span data-ttu-id="b8d9b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8d9b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8d9b-111">Permission type</span></span>                        | <span data-ttu-id="b8d9b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8d9b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b8d9b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d9b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8d9b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d9b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b8d9b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8d9b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8d9b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-116">Not supported.</span></span>                           |
| <span data-ttu-id="b8d9b-117">应用</span><span class="sxs-lookup"><span data-stu-id="b8d9b-117">Application</span></span>                            | <span data-ttu-id="b8d9b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d9b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b8d9b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8d9b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="b8d9b-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="b8d9b-120">Query parameters</span></span>

<span data-ttu-id="b8d9b-121">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b8d9b-122">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-122">The default output type is text/csv.</span></span> <span data-ttu-id="b8d9b-123">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8d9b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8d9b-124">Request headers</span></span>

| <span data-ttu-id="b8d9b-125">名称</span><span class="sxs-lookup"><span data-stu-id="b8d9b-125">Name</span></span>          | <span data-ttu-id="b8d9b-126">说明</span><span class="sxs-lookup"><span data-stu-id="b8d9b-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b8d9b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d9b-127">Authorization</span></span> | <span data-ttu-id="b8d9b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b8d9b-130">响应</span><span class="sxs-lookup"><span data-stu-id="b8d9b-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b8d9b-131">CSV</span><span class="sxs-lookup"><span data-stu-id="b8d9b-131">CSV</span></span>

<span data-ttu-id="b8d9b-132">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b8d9b-133">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b8d9b-134">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b8d9b-135">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b8d9b-136">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b8d9b-136">Report Refresh Date</span></span>
- <span data-ttu-id="b8d9b-137">产品类型</span><span class="sxs-lookup"><span data-stu-id="b8d9b-137">Product Type</span></span>
- <span data-ttu-id="b8d9b-138">Windows</span><span class="sxs-lookup"><span data-stu-id="b8d9b-138">Windows</span></span>
- <span data-ttu-id="b8d9b-139">Mac</span><span class="sxs-lookup"><span data-stu-id="b8d9b-139">Mac</span></span>
- <span data-ttu-id="b8d9b-140">Android</span><span class="sxs-lookup"><span data-stu-id="b8d9b-140">Android</span></span>
- <span data-ttu-id="b8d9b-141">iOS</span><span class="sxs-lookup"><span data-stu-id="b8d9b-141">iOS</span></span>
- <span data-ttu-id="b8d9b-142">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="b8d9b-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="b8d9b-143">JSON</span><span class="sxs-lookup"><span data-stu-id="b8d9b-143">JSON</span></span>

<span data-ttu-id="b8d9b-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActivationCounts](../resources/office365activationcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d9b-145">示例</span><span class="sxs-lookup"><span data-stu-id="b8d9b-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b8d9b-146">CSV</span><span class="sxs-lookup"><span data-stu-id="b8d9b-146">CSV</span></span>

<span data-ttu-id="b8d9b-147">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b8d9b-148">请求</span><span class="sxs-lookup"><span data-stu-id="b8d9b-148">Request</span></span>

<span data-ttu-id="b8d9b-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b8d9b-150">响应</span><span class="sxs-lookup"><span data-stu-id="b8d9b-150">Response</span></span>

<span data-ttu-id="b8d9b-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b8d9b-152">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b8d9b-153">JSON</span><span class="sxs-lookup"><span data-stu-id="b8d9b-153">JSON</span></span>

<span data-ttu-id="b8d9b-154">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b8d9b-155">请求</span><span class="sxs-lookup"><span data-stu-id="b8d9b-155">Request</span></span>

<span data-ttu-id="b8d9b-156">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-156">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b8d9b-157">响应</span><span class="sxs-lookup"><span data-stu-id="b8d9b-157">Response</span></span>

<span data-ttu-id="b8d9b-158">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-158">The following example shows the response.</span></span>

> <span data-ttu-id="b8d9b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b8d9b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
