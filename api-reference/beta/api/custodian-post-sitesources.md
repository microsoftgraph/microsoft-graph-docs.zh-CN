---
title: 创建 siteSource
description: 创建新的 siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0196fac3cf9b44915aa8f979072b2daadf6213f9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659071"
---
# <a name="create-sitesource"></a><span data-ttu-id="36259-103">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="36259-103">Create siteSource</span></span>

<span data-ttu-id="36259-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36259-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36259-105">创建新的 [siteSource](../resources/sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36259-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36259-106">权限</span><span class="sxs-lookup"><span data-stu-id="36259-106">Permissions</span></span>

<span data-ttu-id="36259-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36259-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36259-109">Permission type</span></span>|<span data-ttu-id="36259-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36259-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36259-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36259-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36259-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="36259-112">User.Read</span></span>|
|<span data-ttu-id="36259-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36259-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36259-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36259-114">Not supported.</span></span>|
|<span data-ttu-id="36259-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36259-115">Application</span></span>|<span data-ttu-id="36259-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36259-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36259-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36259-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="36259-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36259-118">Request headers</span></span>

|<span data-ttu-id="36259-119">名称</span><span class="sxs-lookup"><span data-stu-id="36259-119">Name</span></span>|<span data-ttu-id="36259-120">说明</span><span class="sxs-lookup"><span data-stu-id="36259-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36259-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36259-121">Authorization</span></span>|<span data-ttu-id="36259-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36259-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="36259-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36259-124">Content-Type</span></span>|<span data-ttu-id="36259-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="36259-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36259-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36259-127">Request body</span></span>

<span data-ttu-id="36259-128">在请求正文中，提供 [siteSource](../resources/sitesource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36259-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="36259-129">下表显示创建 [siteSource](../resources/sitesource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36259-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="36259-130">属性</span><span class="sxs-lookup"><span data-stu-id="36259-130">Property</span></span>|<span data-ttu-id="36259-131">类型</span><span class="sxs-lookup"><span data-stu-id="36259-131">Type</span></span>|<span data-ttu-id="36259-132">说明</span><span class="sxs-lookup"><span data-stu-id="36259-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36259-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="36259-133">site@odata.bind</span></span>|<span data-ttu-id="36259-134">String</span><span class="sxs-lookup"><span data-stu-id="36259-134">String</span></span>|<span data-ttu-id="36259-135">网站的 ID，您可以通过使用"按路径获取网站[](../resources/site.md)资源"方法从[网站资源获取此](../api/site-getbypath.md)ID。</span><span class="sxs-lookup"><span data-stu-id="36259-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="36259-136">用法为 {hostname}：/{relative-path}。</span><span class="sxs-lookup"><span data-stu-id="36259-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="36259-137">对于网站 `https://contoso.sharepoint.com/sites/HumanResources` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。</span><span class="sxs-lookup"><span data-stu-id="36259-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="36259-138">ID 是 ID 字段中列出的第一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="36259-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="36259-139">响应</span><span class="sxs-lookup"><span data-stu-id="36259-139">Response</span></span>

<span data-ttu-id="36259-140">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [siteSource](../resources/sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36259-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36259-141">示例</span><span class="sxs-lookup"><span data-stu-id="36259-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36259-142">请求</span><span class="sxs-lookup"><span data-stu-id="36259-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36259-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="36259-143">HTTP</span></span>](#tab/http)
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
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/{siteId}"
}
```
# <a name="c"></a>[<span data-ttu-id="36259-144">C#</span><span class="sxs-lookup"><span data-stu-id="36259-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36259-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36259-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36259-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36259-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36259-147">Java</span><span class="sxs-lookup"><span data-stu-id="36259-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36259-148">响应</span><span class="sxs-lookup"><span data-stu-id="36259-148">Response</span></span>

<span data-ttu-id="36259-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36259-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteSource"
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
