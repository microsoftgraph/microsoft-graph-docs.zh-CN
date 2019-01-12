---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 要获取的已启用的用户和那些必须激活桌面或设备上的 Office 订阅或共享计算机的计数。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 18d1ba6da1faf983fe8da3756bb843fe6ac328e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950569"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="fb219-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="fb219-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

> <span data-ttu-id="fb219-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb219-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb219-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb219-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb219-106">要获取的已启用的用户和那些必须激活桌面或设备上的 Office 订阅或共享计算机的计数。</span><span class="sxs-lookup"><span data-stu-id="fb219-106">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="fb219-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="fb219-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb219-108">权限</span><span class="sxs-lookup"><span data-stu-id="fb219-108">Permissions</span></span>

<span data-ttu-id="fb219-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb219-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb219-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb219-111">Permission type</span></span>                        | <span data-ttu-id="fb219-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb219-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fb219-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb219-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb219-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb219-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fb219-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb219-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb219-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb219-116">Not supported.</span></span>                           |
| <span data-ttu-id="fb219-117">应用</span><span class="sxs-lookup"><span data-stu-id="fb219-117">Application</span></span>                            | <span data-ttu-id="fb219-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb219-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fb219-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb219-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="fb219-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="fb219-120">Query parameters</span></span>

<span data-ttu-id="fb219-121">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fb219-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fb219-122">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="fb219-122">The default output type is text/csv.</span></span> <span data-ttu-id="fb219-123">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="fb219-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb219-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb219-124">Request headers</span></span>

| <span data-ttu-id="fb219-125">名称</span><span class="sxs-lookup"><span data-stu-id="fb219-125">Name</span></span>          | <span data-ttu-id="fb219-126">说明</span><span class="sxs-lookup"><span data-stu-id="fb219-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fb219-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb219-127">Authorization</span></span> | <span data-ttu-id="fb219-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb219-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fb219-130">响应</span><span class="sxs-lookup"><span data-stu-id="fb219-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fb219-131">CSV</span><span class="sxs-lookup"><span data-stu-id="fb219-131">CSV</span></span>

<span data-ttu-id="fb219-132">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fb219-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fb219-133">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fb219-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fb219-134">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fb219-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fb219-135">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fb219-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fb219-136">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fb219-136">Report Refresh Date</span></span>
- <span data-ttu-id="fb219-137">产品类型</span><span class="sxs-lookup"><span data-stu-id="fb219-137">Product Type</span></span>
- <span data-ttu-id="fb219-138">已分配</span><span class="sxs-lookup"><span data-stu-id="fb219-138">Assigned</span></span>
- <span data-ttu-id="fb219-139">已激活</span><span class="sxs-lookup"><span data-stu-id="fb219-139">Activated</span></span>
- <span data-ttu-id="fb219-140">共享的计算机激活</span><span class="sxs-lookup"><span data-stu-id="fb219-140">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="fb219-141">JSON</span><span class="sxs-lookup"><span data-stu-id="fb219-141">JSON</span></span>

<span data-ttu-id="fb219-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fb219-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb219-143">示例</span><span class="sxs-lookup"><span data-stu-id="fb219-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fb219-144">CSV</span><span class="sxs-lookup"><span data-stu-id="fb219-144">CSV</span></span>

<span data-ttu-id="fb219-145">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="fb219-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fb219-146">请求</span><span class="sxs-lookup"><span data-stu-id="fb219-146">Request</span></span>

<span data-ttu-id="fb219-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb219-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="fb219-148">响应</span><span class="sxs-lookup"><span data-stu-id="fb219-148">Response</span></span>

<span data-ttu-id="fb219-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb219-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fb219-150">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fb219-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="fb219-151">JSON</span><span class="sxs-lookup"><span data-stu-id="fb219-151">JSON</span></span>

<span data-ttu-id="fb219-152">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fb219-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fb219-153">请求</span><span class="sxs-lookup"><span data-stu-id="fb219-153">Request</span></span>

<span data-ttu-id="fb219-154">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb219-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="fb219-155">响应</span><span class="sxs-lookup"><span data-stu-id="fb219-155">Response</span></span>

<span data-ttu-id="fb219-156">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="fb219-156">The following example shows the response.</span></span>

> <span data-ttu-id="fb219-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb219-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
    }
  ]
}
```
