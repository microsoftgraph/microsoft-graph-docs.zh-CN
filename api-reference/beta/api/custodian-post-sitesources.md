---
title: 创建 siteSource
description: 创建新的 siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 93cb37a6ff94a52830675f876084fc85a6365a40
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597556"
---
# <a name="create-sitesource"></a><span data-ttu-id="f516b-103">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="f516b-103">Create siteSource</span></span>

<span data-ttu-id="f516b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f516b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f516b-105">创建新的 [siteSource](../resources/sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f516b-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f516b-106">权限</span><span class="sxs-lookup"><span data-stu-id="f516b-106">Permissions</span></span>

<span data-ttu-id="f516b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f516b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f516b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f516b-109">Permission type</span></span>|<span data-ttu-id="f516b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f516b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f516b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f516b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f516b-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="f516b-112">User.Read</span></span>|
|<span data-ttu-id="f516b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f516b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f516b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f516b-114">Not supported.</span></span>|
|<span data-ttu-id="f516b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f516b-115">Application</span></span>|<span data-ttu-id="f516b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f516b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f516b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f516b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="f516b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f516b-118">Request headers</span></span>

|<span data-ttu-id="f516b-119">名称</span><span class="sxs-lookup"><span data-stu-id="f516b-119">Name</span></span>|<span data-ttu-id="f516b-120">说明</span><span class="sxs-lookup"><span data-stu-id="f516b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f516b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f516b-121">Authorization</span></span>|<span data-ttu-id="f516b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f516b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f516b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f516b-124">Content-Type</span></span>|<span data-ttu-id="f516b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f516b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f516b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f516b-127">Request body</span></span>

<span data-ttu-id="f516b-128">在请求正文中，提供 [siteSource](../resources/sitesource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f516b-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="f516b-129">下表显示创建 [siteSource](../resources/sitesource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f516b-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="f516b-130">属性</span><span class="sxs-lookup"><span data-stu-id="f516b-130">Property</span></span>|<span data-ttu-id="f516b-131">类型</span><span class="sxs-lookup"><span data-stu-id="f516b-131">Type</span></span>|<span data-ttu-id="f516b-132">Description</span><span class="sxs-lookup"><span data-stu-id="f516b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f516b-133">site@odata 绑定</span><span class="sxs-lookup"><span data-stu-id="f516b-133">site@odata.bind</span></span>|<span data-ttu-id="f516b-134">String</span><span class="sxs-lookup"><span data-stu-id="f516b-134">String</span></span>|<span data-ttu-id="f516b-135">网站的 ID，可以使用 "[按路径获取网站资源](../api/site-getbypath.md)" 方法从[网站](../resources/site.md)资源中获取此 ID。</span><span class="sxs-lookup"><span data-stu-id="f516b-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="f516b-136">用法为 {hostname}：/{relative-path}。</span><span class="sxs-lookup"><span data-stu-id="f516b-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="f516b-137">对于网站 URL `https://contoso.sharepoint.com/sites/HumanResources` ，Microsoft Graph 请求将为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。</span><span class="sxs-lookup"><span data-stu-id="f516b-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="f516b-138">ID 是 ID 字段中列出的第一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="f516b-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="f516b-139">响应</span><span class="sxs-lookup"><span data-stu-id="f516b-139">Response</span></span>

<span data-ttu-id="f516b-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [siteSource](../resources/sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f516b-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f516b-141">示例</span><span class="sxs-lookup"><span data-stu-id="f516b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f516b-142">请求</span><span class="sxs-lookup"><span data-stu-id="f516b-142">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="f516b-143">响应</span><span class="sxs-lookup"><span data-stu-id="f516b-143">Response</span></span>

<span data-ttu-id="f516b-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f516b-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
