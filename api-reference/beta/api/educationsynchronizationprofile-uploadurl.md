---
title: 'educationSynchronizationProfile: uploadUrl'
description: 将源文件上载到租户中的特定学校数据同步配置文件的 Azure blob 存储检索共享的访问签名 (SA)。 SAS 令牌具有一小时的有效性。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 2f6b10bda218bafbe18698defed138c39a45cc7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894143"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="5bc1a-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="5bc1a-104">educationSynchronizationProfile: uploadUrl</span></span>

> <span data-ttu-id="5bc1a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bc1a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bc1a-107">将源文件上载到租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的 Azure blob 存储检索共享的访问签名 (SA)。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-107">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="5bc1a-108">SAS 令牌具有一小时的有效性。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-108">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="5bc1a-109">上载[CSV 数据提供](../resources/educationcsvdataprovider.md)程序仅提供 URL。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-109">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="5bc1a-110">**注意：** 若要访问与 SAS 令牌对 blob 存储，请使用[Azure 存储 Sdk](https://github.com/search?q=org%3AAzure+azure-storage)或[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-110">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bc1a-111">权限</span><span class="sxs-lookup"><span data-stu-id="5bc1a-111">Permissions</span></span>
<span data-ttu-id="5bc1a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bc1a-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bc1a-114">Permission type</span></span> | <span data-ttu-id="5bc1a-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="5bc1a-115">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5bc1a-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bc1a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5bc1a-117">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bc1a-117">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5bc1a-118">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5bc1a-118">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5bc1a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-119">Not supported.</span></span>|
|<span data-ttu-id="5bc1a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bc1a-120">Application</span></span>|<span data-ttu-id="5bc1a-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bc1a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bc1a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="5bc1a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bc1a-123">Request headers</span></span>
| <span data-ttu-id="5bc1a-124">名称</span><span class="sxs-lookup"><span data-stu-id="5bc1a-124">Name</span></span>       | <span data-ttu-id="5bc1a-125">类型</span><span class="sxs-lookup"><span data-stu-id="5bc1a-125">Type</span></span> | <span data-ttu-id="5bc1a-126">说明</span><span class="sxs-lookup"><span data-stu-id="5bc1a-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5bc1a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bc1a-127">Authorization</span></span>  | <span data-ttu-id="5bc1a-128">string</span><span class="sxs-lookup"><span data-stu-id="5bc1a-128">string</span></span>  | <span data-ttu-id="5bc1a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bc1a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bc1a-131">Request body</span></span>
<span data-ttu-id="5bc1a-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5bc1a-133">响应</span><span class="sxs-lookup"><span data-stu-id="5bc1a-133">Response</span></span>
<span data-ttu-id="5bc1a-134">如果成功，此方法返回`200 OK`响应代码和响应正文中[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) SAS URL。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-134">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="5bc1a-135">如果仍在处理的上一个请求，此方法返回`409 Conflict`，指出上载的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)目前被阻止。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-135">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="5bc1a-136">示例</span><span class="sxs-lookup"><span data-stu-id="5bc1a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bc1a-137">请求</span><span class="sxs-lookup"><span data-stu-id="5bc1a-137">Request</span></span>
<span data-ttu-id="5bc1a-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="5bc1a-139">响应</span><span class="sxs-lookup"><span data-stu-id="5bc1a-139">Response</span></span>
<span data-ttu-id="5bc1a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-140">The following is an example of the response.</span></span> 

><span data-ttu-id="5bc1a-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5bc1a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
