---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0d0bb083ca0f869584361e9f9d30f4c1af65e598
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589039"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="64e3b-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="64e3b-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="64e3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64e3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e3b-105">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="64e3b-105">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="64e3b-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="64e3b-106">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="64e3b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="64e3b-107">Permissions</span></span>

<span data-ttu-id="64e3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64e3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64e3b-110">Permission type</span></span>                        | <span data-ttu-id="64e3b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64e3b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64e3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64e3b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="64e3b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64e3b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64e3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64e3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64e3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64e3b-115">Not supported.</span></span>                           |
| <span data-ttu-id="64e3b-116">应用</span><span class="sxs-lookup"><span data-stu-id="64e3b-116">Application</span></span>                            | <span data-ttu-id="64e3b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64e3b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="64e3b-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="64e3b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="64e3b-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="64e3b-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="64e3b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64e3b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="64e3b-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="64e3b-121">Query parameters</span></span>

<span data-ttu-id="64e3b-122">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64e3b-122">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="64e3b-123">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="64e3b-123">The default output type is text/csv.</span></span> <span data-ttu-id="64e3b-124">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="64e3b-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64e3b-125">请求头</span><span class="sxs-lookup"><span data-stu-id="64e3b-125">Request headers</span></span>

| <span data-ttu-id="64e3b-126">名称</span><span class="sxs-lookup"><span data-stu-id="64e3b-126">Name</span></span>          | <span data-ttu-id="64e3b-127">说明</span><span class="sxs-lookup"><span data-stu-id="64e3b-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="64e3b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="64e3b-128">Authorization</span></span> | <span data-ttu-id="64e3b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64e3b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="64e3b-131">响应</span><span class="sxs-lookup"><span data-stu-id="64e3b-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="64e3b-132">CSV</span><span class="sxs-lookup"><span data-stu-id="64e3b-132">CSV</span></span>

<span data-ttu-id="64e3b-133">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="64e3b-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64e3b-134">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="64e3b-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64e3b-135">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="64e3b-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64e3b-136">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="64e3b-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64e3b-137">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="64e3b-137">Report Refresh Date</span></span>
- <span data-ttu-id="64e3b-138">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="64e3b-138">User Principal Name</span></span>
- <span data-ttu-id="64e3b-139">显示名称</span><span class="sxs-lookup"><span data-stu-id="64e3b-139">Display Name</span></span>
- <span data-ttu-id="64e3b-140">产品类型</span><span class="sxs-lookup"><span data-stu-id="64e3b-140">Product Type</span></span>
- <span data-ttu-id="64e3b-141">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="64e3b-141">Last Activated Date</span></span>
- <span data-ttu-id="64e3b-142">Windows</span><span class="sxs-lookup"><span data-stu-id="64e3b-142">Windows</span></span>
- <span data-ttu-id="64e3b-143">Mac</span><span class="sxs-lookup"><span data-stu-id="64e3b-143">Mac</span></span>
- <span data-ttu-id="64e3b-144">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="64e3b-144">Windows 10 Mobile</span></span>
- <span data-ttu-id="64e3b-145">iOS</span><span class="sxs-lookup"><span data-stu-id="64e3b-145">iOS</span></span>
- <span data-ttu-id="64e3b-146">Android</span><span class="sxs-lookup"><span data-stu-id="64e3b-146">Android</span></span>
- <span data-ttu-id="64e3b-147">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="64e3b-147">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="64e3b-148">JSON</span><span class="sxs-lookup"><span data-stu-id="64e3b-148">JSON</span></span>

<span data-ttu-id="64e3b-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="64e3b-149">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="64e3b-150">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="64e3b-150">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="64e3b-151">示例</span><span class="sxs-lookup"><span data-stu-id="64e3b-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="64e3b-152">CSV</span><span class="sxs-lookup"><span data-stu-id="64e3b-152">CSV</span></span>

<span data-ttu-id="64e3b-153">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="64e3b-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="64e3b-154">请求</span><span class="sxs-lookup"><span data-stu-id="64e3b-154">Request</span></span>

<span data-ttu-id="64e3b-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64e3b-155">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="64e3b-156">响应</span><span class="sxs-lookup"><span data-stu-id="64e3b-156">Response</span></span>

<span data-ttu-id="64e3b-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64e3b-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="64e3b-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="64e3b-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="64e3b-159">JSON</span><span class="sxs-lookup"><span data-stu-id="64e3b-159">JSON</span></span>

<span data-ttu-id="64e3b-160">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="64e3b-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="64e3b-161">请求</span><span class="sxs-lookup"><span data-stu-id="64e3b-161">Request</span></span>

<span data-ttu-id="64e3b-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64e3b-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="64e3b-163">响应</span><span class="sxs-lookup"><span data-stu-id="64e3b-163">Response</span></span>

<span data-ttu-id="64e3b-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="64e3b-164">The following is an example of the response.</span></span>

> <span data-ttu-id="64e3b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="64e3b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
