---
title: 创建保管人 siteSource
description: 创建新的保管人 siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 869f967073e4f41cf5d4cb40f18e9b7f6ba825d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773247"
---
# <a name="create-custodian-sitesource"></a><span data-ttu-id="e9233-103">创建保管人 siteSource</span><span class="sxs-lookup"><span data-stu-id="e9233-103">Create custodian siteSource</span></span>

<span data-ttu-id="e9233-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e9233-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9233-105">创建新的保管人 [siteSource](../resources/ediscovery-sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9233-105">Create a new custodian [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9233-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9233-106">Permissions</span></span>

<span data-ttu-id="e9233-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9233-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9233-109">Permission type</span></span>|<span data-ttu-id="e9233-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9233-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9233-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9233-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9233-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9233-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e9233-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9233-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9233-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9233-114">Not supported.</span></span>|
|<span data-ttu-id="e9233-115">Application</span><span class="sxs-lookup"><span data-stu-id="e9233-115">Application</span></span>|<span data-ttu-id="e9233-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9233-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9233-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9233-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="e9233-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9233-118">Request headers</span></span>

|<span data-ttu-id="e9233-119">名称</span><span class="sxs-lookup"><span data-stu-id="e9233-119">Name</span></span>|<span data-ttu-id="e9233-120">说明</span><span class="sxs-lookup"><span data-stu-id="e9233-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9233-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9233-121">Authorization</span></span>|<span data-ttu-id="e9233-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9233-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e9233-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9233-124">Content-Type</span></span>|<span data-ttu-id="e9233-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e9233-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9233-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9233-127">Request body</span></span>

<span data-ttu-id="e9233-128">在请求正文中，提供 [siteSource](../resources/ediscovery-sitesource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9233-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="e9233-129">下表显示创建 [siteSource](../resources/ediscovery-sitesource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e9233-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="e9233-130">属性</span><span class="sxs-lookup"><span data-stu-id="e9233-130">Property</span></span>|<span data-ttu-id="e9233-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9233-131">Type</span></span>|<span data-ttu-id="e9233-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9233-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9233-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="e9233-133">site@odata.bind</span></span>|<span data-ttu-id="e9233-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e9233-134">String</span></span>|<span data-ttu-id="e9233-135">网站的 ID，您可以使用"按路径获取网站资源[](../resources/site.md)"方法[从网站资源获取此](../api/site-getbypath.md)ID。</span><span class="sxs-lookup"><span data-stu-id="e9233-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="e9233-136">用法为 {hostname}：/{relative-path}。</span><span class="sxs-lookup"><span data-stu-id="e9233-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="e9233-137">对于网站 `https://contoso.sharepoint.com/sites/HumanResources` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。</span><span class="sxs-lookup"><span data-stu-id="e9233-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="e9233-138">ID 是 ID 字段中列出的第一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="e9233-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="e9233-139">对于 OneDrive for Business 网站 `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com` 。</span><span class="sxs-lookup"><span data-stu-id="e9233-139">For the OneDrive for Business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`.</span></span> |

## <a name="response"></a><span data-ttu-id="e9233-140">响应</span><span class="sxs-lookup"><span data-stu-id="e9233-140">Response</span></span>

<span data-ttu-id="e9233-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9233-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9233-142">示例</span><span class="sxs-lookup"><span data-stu-id="e9233-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9233-143">请求</span><span class="sxs-lookup"><span data-stu-id="e9233-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e9233-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9233-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
Content-Type: application/json
Content-length: 179

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```
# <a name="c"></a>[<span data-ttu-id="e9233-145">C#</span><span class="sxs-lookup"><span data-stu-id="e9233-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9233-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9233-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9233-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9233-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9233-148">Java</span><span class="sxs-lookup"><span data-stu-id="e9233-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9233-149">响应</span><span class="sxs-lookup"><span data-stu-id="e9233-149">Response</span></span>

<span data-ttu-id="e9233-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9233-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Human resources site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
