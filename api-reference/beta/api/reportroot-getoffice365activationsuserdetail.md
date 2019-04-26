---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8f40f2ecc16dbea7c749b5932369063cdaaa85f1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336758"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="4f82a-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="4f82a-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f82a-104">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4f82a-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="4f82a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="4f82a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f82a-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f82a-106">Permissions</span></span>

<span data-ttu-id="4f82a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f82a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f82a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f82a-109">Permission type</span></span>                        | <span data-ttu-id="4f82a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f82a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4f82a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f82a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f82a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f82a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4f82a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f82a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f82a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f82a-114">Not supported.</span></span>                           |
| <span data-ttu-id="4f82a-115">应用</span><span class="sxs-lookup"><span data-stu-id="4f82a-115">Application</span></span>                            | <span data-ttu-id="4f82a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f82a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4f82a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f82a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="4f82a-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="4f82a-118">Query parameters</span></span>

<span data-ttu-id="4f82a-119">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4f82a-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4f82a-120">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="4f82a-120">The default output type is text/csv.</span></span> <span data-ttu-id="4f82a-121">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="4f82a-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f82a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f82a-122">Request headers</span></span>

| <span data-ttu-id="4f82a-123">名称</span><span class="sxs-lookup"><span data-stu-id="4f82a-123">Name</span></span>          | <span data-ttu-id="4f82a-124">说明</span><span class="sxs-lookup"><span data-stu-id="4f82a-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4f82a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f82a-125">Authorization</span></span> | <span data-ttu-id="4f82a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f82a-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4f82a-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f82a-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4f82a-129">CSV</span><span class="sxs-lookup"><span data-stu-id="4f82a-129">CSV</span></span>

<span data-ttu-id="4f82a-130">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4f82a-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4f82a-131">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4f82a-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4f82a-132">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4f82a-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4f82a-133">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4f82a-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4f82a-134">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4f82a-134">Report Refresh Date</span></span>
- <span data-ttu-id="4f82a-135">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4f82a-135">User Principal Name</span></span>
- <span data-ttu-id="4f82a-136">显示名称</span><span class="sxs-lookup"><span data-stu-id="4f82a-136">Display Name</span></span>
- <span data-ttu-id="4f82a-137">产品类型</span><span class="sxs-lookup"><span data-stu-id="4f82a-137">Product Type</span></span>
- <span data-ttu-id="4f82a-138">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="4f82a-138">Last Activated Date</span></span>
- <span data-ttu-id="4f82a-139">Windows</span><span class="sxs-lookup"><span data-stu-id="4f82a-139">Windows</span></span>
- <span data-ttu-id="4f82a-140">Mac</span><span class="sxs-lookup"><span data-stu-id="4f82a-140">Mac</span></span>
- <span data-ttu-id="4f82a-141">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="4f82a-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="4f82a-142">iOS</span><span class="sxs-lookup"><span data-stu-id="4f82a-142">iOS</span></span>
- <span data-ttu-id="4f82a-143">Android</span><span class="sxs-lookup"><span data-stu-id="4f82a-143">Android</span></span>
- <span data-ttu-id="4f82a-144">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="4f82a-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="4f82a-145">JSON</span><span class="sxs-lookup"><span data-stu-id="4f82a-145">JSON</span></span>

<span data-ttu-id="4f82a-146">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="4f82a-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="4f82a-147">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="4f82a-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4f82a-148">示例</span><span class="sxs-lookup"><span data-stu-id="4f82a-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4f82a-149">CSV</span><span class="sxs-lookup"><span data-stu-id="4f82a-149">CSV</span></span>

<span data-ttu-id="4f82a-150">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="4f82a-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4f82a-151">请求</span><span class="sxs-lookup"><span data-stu-id="4f82a-151">Request</span></span>

<span data-ttu-id="4f82a-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f82a-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4f82a-153">响应</span><span class="sxs-lookup"><span data-stu-id="4f82a-153">Response</span></span>

<span data-ttu-id="4f82a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f82a-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4f82a-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4f82a-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="4f82a-156">JSON</span><span class="sxs-lookup"><span data-stu-id="4f82a-156">JSON</span></span>

<span data-ttu-id="4f82a-157">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="4f82a-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4f82a-158">请求</span><span class="sxs-lookup"><span data-stu-id="4f82a-158">Request</span></span>

<span data-ttu-id="4f82a-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f82a-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4f82a-160">响应</span><span class="sxs-lookup"><span data-stu-id="4f82a-160">Response</span></span>

<span data-ttu-id="4f82a-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f82a-161">The following is an example of the response.</span></span>

> <span data-ttu-id="4f82a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f82a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
        }
      ]
    }
  ]
}
```
