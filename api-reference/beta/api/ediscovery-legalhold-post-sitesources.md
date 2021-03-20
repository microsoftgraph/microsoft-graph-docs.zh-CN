---
title: 创建 legalHold siteSource
description: 创建新的 legalHold siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bca1f4c54593cc92f9b085bc86669981974e4432
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952453"
---
# <a name="create-legalhold-sitesource"></a><span data-ttu-id="62388-103">创建 legalHold siteSource</span><span class="sxs-lookup"><span data-stu-id="62388-103">Create legalHold siteSource</span></span>

<span data-ttu-id="62388-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="62388-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62388-105">将 siteSource 添加到 legalHold 对象。</span><span class="sxs-lookup"><span data-stu-id="62388-105">Adds a siteSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62388-106">权限</span><span class="sxs-lookup"><span data-stu-id="62388-106">Permissions</span></span>

<span data-ttu-id="62388-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62388-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62388-109">Permission type</span></span>|<span data-ttu-id="62388-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62388-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62388-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62388-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62388-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62388-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="62388-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62388-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62388-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62388-114">Not supported.</span></span>|
|<span data-ttu-id="62388-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62388-115">Application</span></span>|<span data-ttu-id="62388-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="62388-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62388-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62388-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="62388-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62388-118">Request headers</span></span>

|<span data-ttu-id="62388-119">名称</span><span class="sxs-lookup"><span data-stu-id="62388-119">Name</span></span>|<span data-ttu-id="62388-120">说明</span><span class="sxs-lookup"><span data-stu-id="62388-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62388-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62388-121">Authorization</span></span>|<span data-ttu-id="62388-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62388-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62388-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62388-124">Content-Type</span></span>|<span data-ttu-id="62388-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62388-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62388-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62388-127">Request body</span></span>

<span data-ttu-id="62388-128">在请求正文中，提供 [siteSource](../resources/ediscovery-sitesource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62388-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="62388-129">下表显示创建 [siteSource](../resources/ediscovery-sitesource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="62388-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="62388-130">属性</span><span class="sxs-lookup"><span data-stu-id="62388-130">Property</span></span>|<span data-ttu-id="62388-131">类型</span><span class="sxs-lookup"><span data-stu-id="62388-131">Type</span></span>|<span data-ttu-id="62388-132">说明</span><span class="sxs-lookup"><span data-stu-id="62388-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62388-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="62388-133">site@odata.bind</span></span>|<span data-ttu-id="62388-134">String</span><span class="sxs-lookup"><span data-stu-id="62388-134">String</span></span>|<span data-ttu-id="62388-135">网站的 ID，您可以使用"按路径获取网站资源[](../resources/site.md)"方法[从网站资源获取此](../api/site-getbypath.md)ID。</span><span class="sxs-lookup"><span data-stu-id="62388-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="62388-136">用法为 {hostname}：/{relative-path}。</span><span class="sxs-lookup"><span data-stu-id="62388-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="62388-137">对于网站 `https://contoso.sharepoint.com/sites/HumanResources` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。</span><span class="sxs-lookup"><span data-stu-id="62388-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="62388-138">ID 是 ID 字段中列出的第一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="62388-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="62388-139">对于 OneDrive for Business 网站 `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span><span class="sxs-lookup"><span data-stu-id="62388-139">For the OneDrive for business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span></span> |

## <a name="response"></a><span data-ttu-id="62388-140">响应</span><span class="sxs-lookup"><span data-stu-id="62388-140">Response</span></span>

<span data-ttu-id="62388-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62388-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62388-142">示例</span><span class="sxs-lookup"><span data-stu-id="62388-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62388-143">请求</span><span class="sxs-lookup"><span data-stu-id="62388-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="62388-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="62388-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/siteSources
Content-Type: application/json
Content-length: 154

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```
# <a name="c"></a>[<span data-ttu-id="62388-145">C#</span><span class="sxs-lookup"><span data-stu-id="62388-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62388-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62388-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62388-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62388-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62388-148">Java</span><span class="sxs-lookup"><span data-stu-id="62388-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62388-149">响应</span><span class="sxs-lookup"><span data-stu-id="62388-149">Response</span></span>

<span data-ttu-id="62388-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62388-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('387566cc-38ae-4e85-ab4b-cd2dd34faa07')/siteSources/$entity",
    "displayName": "Adele Vance",
    "createdDateTime": "2020-12-28T20:08:57.857Z",
    "id": "50073f3e-cb22-48e5-95a9-51a3da455181",
    "createdBy": {
        "user": {
            "id": null,
            "displayName": "EDiscovery admin"
        }
    }
}
```
