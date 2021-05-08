---
title: 创建 noncustodialDataSource
description: 创建新的 noncustodialDataSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 840cddbdfa4c0172bdce85a46238e95d5f059a86
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266657"
---
# <a name="create-noncustodialdatasource"></a><span data-ttu-id="25b2f-103">创建 noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="25b2f-103">Create noncustodialDataSource</span></span>

<span data-ttu-id="25b2f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="25b2f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25b2f-105">创建新的 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25b2f-105">Create a new [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25b2f-106">权限</span><span class="sxs-lookup"><span data-stu-id="25b2f-106">Permissions</span></span>

<span data-ttu-id="25b2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25b2f-109">Permission type</span></span>|<span data-ttu-id="25b2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25b2f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25b2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25b2f-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b2f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="25b2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25b2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="25b2f-114">Not supported.</span></span>|
|<span data-ttu-id="25b2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="25b2f-115">Application</span></span>|<span data-ttu-id="25b2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="25b2f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25b2f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="request-headers"></a><span data-ttu-id="25b2f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25b2f-118">Request headers</span></span>

|<span data-ttu-id="25b2f-119">名称</span><span class="sxs-lookup"><span data-stu-id="25b2f-119">Name</span></span>|<span data-ttu-id="25b2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="25b2f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25b2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b2f-121">Authorization</span></span>|<span data-ttu-id="25b2f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25b2f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="25b2f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25b2f-124">Content-Type</span></span>|<span data-ttu-id="25b2f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="25b2f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b2f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="25b2f-127">Request body</span></span>

<span data-ttu-id="25b2f-128">在请求正文中，提供 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25b2f-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="25b2f-129">下表显示创建 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25b2f-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="25b2f-130">属性</span><span class="sxs-lookup"><span data-stu-id="25b2f-130">Property</span></span>|<span data-ttu-id="25b2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="25b2f-131">Type</span></span>|<span data-ttu-id="25b2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="25b2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b2f-133">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="25b2f-133">applyHoldToSource</span></span>|<span data-ttu-id="25b2f-134">布尔</span><span class="sxs-lookup"><span data-stu-id="25b2f-134">Boolean</span></span>|<span data-ttu-id="25b2f-135">指示是否将保留应用于非 (数据源，如邮箱或网站) 。</span><span class="sxs-lookup"><span data-stu-id="25b2f-135">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="25b2f-136">datasource</span><span class="sxs-lookup"><span data-stu-id="25b2f-136">datasource</span></span>|[<span data-ttu-id="25b2f-137">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="25b2f-137">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="25b2f-138">userSource 或 siteSource。</span><span class="sxs-lookup"><span data-stu-id="25b2f-138">Either a userSource or siteSource.</span></span>  <span data-ttu-id="25b2f-139">对于 userSource，请使用"dataSource" ： { "@odata.type" ： "microsoft.graph.ediscovery.userSource"， "email" ： "SMTP address"}。</span><span class="sxs-lookup"><span data-stu-id="25b2f-139">For userSource, use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.</span></span>  <span data-ttu-id="25b2f-140">对于网站源，请使用"dataSource" ： { "@odata.type" ： "microsoft.graph.ediscovery.siteSource"， "site@odata.bind" ： "siteId" }，其中 siteId 可以派生自网站 URL，例如 `https://contoso.sharepoint.com/sites/HumanResources` ，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。</span><span class="sxs-lookup"><span data-stu-id="25b2f-140">For site source use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.siteSource", "site@odata.bind" : "siteId" }, where siteId can be derived from the site URL, e.g. `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="25b2f-141">ID 是 ID 字段中列出的第一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="25b2f-141">The ID is the first GUID listed in the ID field.</span></span>

## <a name="response"></a><span data-ttu-id="25b2f-142">响应</span><span class="sxs-lookup"><span data-stu-id="25b2f-142">Response</span></span>

<span data-ttu-id="25b2f-143">如果成功，此方法在响应正文中返回 响应代码和非 `201 Created` [custodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25b2f-143">If successful, this method returns a `201 Created` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25b2f-144">示例</span><span class="sxs-lookup"><span data-stu-id="25b2f-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25b2f-145">请求</span><span class="sxs-lookup"><span data-stu-id="25b2f-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25b2f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="25b2f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json
Content-length: 206

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="25b2f-147">C#</span><span class="sxs-lookup"><span data-stu-id="25b2f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25b2f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25b2f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25b2f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25b2f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25b2f-150">Java</span><span class="sxs-lookup"><span data-stu-id="25b2f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25b2f-151">响应</span><span class="sxs-lookup"><span data-stu-id="25b2f-151">Response</span></span>

<span data-ttu-id="25b2f-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="25b2f-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```
