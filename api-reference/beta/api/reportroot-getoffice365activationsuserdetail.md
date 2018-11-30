---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
ms.openlocfilehash: 1dbbfefc7ea620f0926b037bd138bb04ed362c5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043741"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="7b632-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="7b632-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

> <span data-ttu-id="7b632-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b632-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b632-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b632-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b632-106">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7b632-106">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="7b632-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="7b632-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b632-108">权限</span><span class="sxs-lookup"><span data-stu-id="7b632-108">Permissions</span></span>

<span data-ttu-id="7b632-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b632-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b632-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b632-111">Permission type</span></span>                        | <span data-ttu-id="7b632-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b632-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7b632-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b632-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b632-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b632-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7b632-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b632-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b632-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b632-116">Not supported.</span></span>                           |
| <span data-ttu-id="7b632-117">应用</span><span class="sxs-lookup"><span data-stu-id="7b632-117">Application</span></span>                            | <span data-ttu-id="7b632-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b632-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7b632-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b632-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="7b632-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="7b632-120">Query parameters</span></span>

<span data-ttu-id="7b632-121">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b632-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7b632-122">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="7b632-122">The default output type is text/csv.</span></span> <span data-ttu-id="7b632-123">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="7b632-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b632-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b632-124">Request headers</span></span>

| <span data-ttu-id="7b632-125">名称</span><span class="sxs-lookup"><span data-stu-id="7b632-125">Name</span></span>          | <span data-ttu-id="7b632-126">说明</span><span class="sxs-lookup"><span data-stu-id="7b632-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7b632-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b632-127">Authorization</span></span> | <span data-ttu-id="7b632-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b632-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7b632-130">响应</span><span class="sxs-lookup"><span data-stu-id="7b632-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7b632-131">CSV</span><span class="sxs-lookup"><span data-stu-id="7b632-131">CSV</span></span>

<span data-ttu-id="7b632-132">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7b632-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7b632-133">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7b632-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7b632-134">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7b632-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7b632-135">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7b632-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7b632-136">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7b632-136">Report Refresh Date</span></span>
- <span data-ttu-id="7b632-137">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="7b632-137">User Principal Name</span></span>
- <span data-ttu-id="7b632-138">显示名称</span><span class="sxs-lookup"><span data-stu-id="7b632-138">Display Name</span></span>
- <span data-ttu-id="7b632-139">产品类型</span><span class="sxs-lookup"><span data-stu-id="7b632-139">Product Type</span></span>
- <span data-ttu-id="7b632-140">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="7b632-140">Last Activated Date</span></span>
- <span data-ttu-id="7b632-141">Windows</span><span class="sxs-lookup"><span data-stu-id="7b632-141">Windows</span></span>
- <span data-ttu-id="7b632-142">Mac</span><span class="sxs-lookup"><span data-stu-id="7b632-142">Mac</span></span>
- <span data-ttu-id="7b632-143">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="7b632-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="7b632-144">iOS</span><span class="sxs-lookup"><span data-stu-id="7b632-144">iOS</span></span>
- <span data-ttu-id="7b632-145">Android</span><span class="sxs-lookup"><span data-stu-id="7b632-145">Android</span></span>
- <span data-ttu-id="7b632-146">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="7b632-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="7b632-147">JSON</span><span class="sxs-lookup"><span data-stu-id="7b632-147">JSON</span></span>

<span data-ttu-id="7b632-148">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7b632-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7b632-149">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="7b632-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7b632-150">示例</span><span class="sxs-lookup"><span data-stu-id="7b632-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7b632-151">CSV</span><span class="sxs-lookup"><span data-stu-id="7b632-151">CSV</span></span>

<span data-ttu-id="7b632-152">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="7b632-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7b632-153">请求</span><span class="sxs-lookup"><span data-stu-id="7b632-153">Request</span></span>

<span data-ttu-id="7b632-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b632-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7b632-155">响应</span><span class="sxs-lookup"><span data-stu-id="7b632-155">Response</span></span>

<span data-ttu-id="7b632-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b632-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7b632-157">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7b632-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7b632-158">JSON</span><span class="sxs-lookup"><span data-stu-id="7b632-158">JSON</span></span>

<span data-ttu-id="7b632-159">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7b632-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7b632-160">请求</span><span class="sxs-lookup"><span data-stu-id="7b632-160">Request</span></span>

<span data-ttu-id="7b632-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b632-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7b632-162">响应</span><span class="sxs-lookup"><span data-stu-id="7b632-162">Response</span></span>

<span data-ttu-id="7b632-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b632-163">The following is an example of the response.</span></span>

> <span data-ttu-id="7b632-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b632-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
