---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: 获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6769f3a5124e0b4024e288c8bc02918c4df5e3d8
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896334"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="002a0-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="002a0-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="002a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="002a0-105">获取启用的用户数以及在桌面或设备或共享计算机上激活 Office 订阅的用户数。</span><span class="sxs-lookup"><span data-stu-id="002a0-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="002a0-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="002a0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="002a0-107">权限</span><span class="sxs-lookup"><span data-stu-id="002a0-107">Permissions</span></span>

<span data-ttu-id="002a0-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="002a0-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="002a0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="002a0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="002a0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="002a0-110">Permission type</span></span>                        | <span data-ttu-id="002a0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="002a0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="002a0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="002a0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="002a0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="002a0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="002a0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="002a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="002a0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="002a0-115">Not supported.</span></span>                           |
| <span data-ttu-id="002a0-116">应用</span><span class="sxs-lookup"><span data-stu-id="002a0-116">Application</span></span>                            | <span data-ttu-id="002a0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="002a0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="002a0-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="002a0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="002a0-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="002a0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="002a0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="002a0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="002a0-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="002a0-121">Query parameters</span></span>

<span data-ttu-id="002a0-122">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="002a0-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="002a0-123">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="002a0-123">The default output type is text/csv.</span></span> <span data-ttu-id="002a0-124">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="002a0-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="002a0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="002a0-125">Request headers</span></span>

| <span data-ttu-id="002a0-126">名称</span><span class="sxs-lookup"><span data-stu-id="002a0-126">Name</span></span>          | <span data-ttu-id="002a0-127">说明</span><span class="sxs-lookup"><span data-stu-id="002a0-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="002a0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="002a0-128">Authorization</span></span> | <span data-ttu-id="002a0-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="002a0-129">Bearer {token}.</span></span> <span data-ttu-id="002a0-130">Required.</span><span class="sxs-lookup"><span data-stu-id="002a0-130">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="002a0-131">响应</span><span class="sxs-lookup"><span data-stu-id="002a0-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="002a0-132">CSV</span><span class="sxs-lookup"><span data-stu-id="002a0-132">CSV</span></span>

<span data-ttu-id="002a0-133">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="002a0-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="002a0-134">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="002a0-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="002a0-135">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="002a0-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="002a0-136">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="002a0-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="002a0-137">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="002a0-137">Report Refresh Date</span></span>
- <span data-ttu-id="002a0-138">产品类型</span><span class="sxs-lookup"><span data-stu-id="002a0-138">Product Type</span></span>
- <span data-ttu-id="002a0-139">已分配</span><span class="sxs-lookup"><span data-stu-id="002a0-139">Assigned</span></span>
- <span data-ttu-id="002a0-140">已激活</span><span class="sxs-lookup"><span data-stu-id="002a0-140">Activated</span></span>
- <span data-ttu-id="002a0-141">共享计算机激活</span><span class="sxs-lookup"><span data-stu-id="002a0-141">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="002a0-142">JSON</span><span class="sxs-lookup"><span data-stu-id="002a0-142">JSON</span></span>

<span data-ttu-id="002a0-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="002a0-143">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="002a0-144">示例</span><span class="sxs-lookup"><span data-stu-id="002a0-144">Example</span></span>

### <a name="csv"></a><span data-ttu-id="002a0-145">CSV</span><span class="sxs-lookup"><span data-stu-id="002a0-145">CSV</span></span>

<span data-ttu-id="002a0-146">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="002a0-146">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="002a0-147">请求</span><span class="sxs-lookup"><span data-stu-id="002a0-147">Request</span></span>

<span data-ttu-id="002a0-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="002a0-148">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="002a0-149">响应</span><span class="sxs-lookup"><span data-stu-id="002a0-149">Response</span></span>

<span data-ttu-id="002a0-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="002a0-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="002a0-151">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="002a0-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="002a0-152">JSON</span><span class="sxs-lookup"><span data-stu-id="002a0-152">JSON</span></span>

<span data-ttu-id="002a0-153">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="002a0-153">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="002a0-154">请求</span><span class="sxs-lookup"><span data-stu-id="002a0-154">Request</span></span>

<span data-ttu-id="002a0-155">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="002a0-155">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="002a0-156">响应</span><span class="sxs-lookup"><span data-stu-id="002a0-156">Response</span></span>

<span data-ttu-id="002a0-157">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="002a0-157">The following example shows the response.</span></span>

> <span data-ttu-id="002a0-158">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="002a0-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="002a0-159">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="002a0-159">All the properties will be returned from an actual call.</span></span>

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
      "productType": "Microsoft 365 Apps for enterprise", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
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
