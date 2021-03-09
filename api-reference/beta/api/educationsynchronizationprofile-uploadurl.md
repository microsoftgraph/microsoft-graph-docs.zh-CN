---
title: educationSynchronizationProfile： uploadUrl
description: 检索 SAS (共享) ，以将源文件上传到租户中特定学校数据同步配置文件的 Azure blob 存储。 SAS 令牌的有效期为 1 小时。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e7fe3af888582fc38d617c1445e0e7c5473c528b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574147"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="f7800-104">educationSynchronizationProfile： uploadUrl</span><span class="sxs-lookup"><span data-stu-id="f7800-104">educationSynchronizationProfile: uploadUrl</span></span>

<span data-ttu-id="f7800-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7800-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7800-106">在 SAS (检索共享) 签名，以将源文件上传到租户中特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的 Azure blob 存储。</span><span class="sxs-lookup"><span data-stu-id="f7800-106">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f7800-107">SAS 令牌的有效期为 1 小时。</span><span class="sxs-lookup"><span data-stu-id="f7800-107">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="f7800-108">上载 URL 仅为 CSV 数据 [提供程序提供](../resources/educationcsvdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="f7800-108">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="f7800-109">**注意：** 若要使用 SAS 令牌访问 blob 存储，请使用 [Azure 存储 SDK](https://github.com/search?q=org%3AAzure+azure-storage)或 [AzCopy。](/azure/storage/storage-use-azcopy)</span><span class="sxs-lookup"><span data-stu-id="f7800-109">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7800-110">权限</span><span class="sxs-lookup"><span data-stu-id="f7800-110">Permissions</span></span>
<span data-ttu-id="f7800-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7800-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7800-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7800-113">Permission type</span></span> | <span data-ttu-id="f7800-114">权限</span><span class="sxs-lookup"><span data-stu-id="f7800-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f7800-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7800-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f7800-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7800-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f7800-117">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="f7800-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f7800-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7800-118">Not supported.</span></span>|
|<span data-ttu-id="f7800-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7800-119">Application</span></span>|<span data-ttu-id="f7800-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7800-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7800-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7800-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="f7800-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7800-122">Request headers</span></span>
| <span data-ttu-id="f7800-123">名称</span><span class="sxs-lookup"><span data-stu-id="f7800-123">Name</span></span>       | <span data-ttu-id="f7800-124">类型</span><span class="sxs-lookup"><span data-stu-id="f7800-124">Type</span></span> | <span data-ttu-id="f7800-125">说明</span><span class="sxs-lookup"><span data-stu-id="f7800-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7800-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7800-126">Authorization</span></span>  | <span data-ttu-id="f7800-127">string</span><span class="sxs-lookup"><span data-stu-id="f7800-127">string</span></span>  | <span data-ttu-id="f7800-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7800-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7800-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7800-130">Request body</span></span>
<span data-ttu-id="f7800-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7800-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f7800-132">响应</span><span class="sxs-lookup"><span data-stu-id="f7800-132">Response</span></span>
<span data-ttu-id="f7800-133">如果成功，此方法在响应正文中返回 `200 OK` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 的响应代码和 SAS URL。</span><span class="sxs-lookup"><span data-stu-id="f7800-133">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="f7800-134">如果上一个请求仍在处理中，此方法将返回一个指示当前已阻止 `409 Conflict` [educationSynchronizationProfile 的上载。](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f7800-134">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="f7800-135">示例</span><span class="sxs-lookup"><span data-stu-id="f7800-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7800-136">请求</span><span class="sxs-lookup"><span data-stu-id="f7800-136">Request</span></span>
<span data-ttu-id="f7800-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7800-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7800-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7800-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="c"></a>[<span data-ttu-id="f7800-139">C#</span><span class="sxs-lookup"><span data-stu-id="f7800-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7800-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7800-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7800-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7800-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7800-142">Java</span><span class="sxs-lookup"><span data-stu-id="f7800-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7800-143">响应</span><span class="sxs-lookup"><span data-stu-id="f7800-143">Response</span></span>
<span data-ttu-id="f7800-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7800-144">The following is an example of the response.</span></span>

><span data-ttu-id="f7800-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7800-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
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


