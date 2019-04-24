---
title: 'educationSynchronizationProfile: uploadUrl'
description: 检索用于将源文件上载到租户中特定学校数据同步配置文件的 Azure blob 存储的共享访问签名 (SAS)。 SAS 令牌的有效期为1小时。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464696"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="c0c0a-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="c0c0a-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c0a-105">检索用于将源文件上载到租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的 Azure blob 存储的共享访问签名 (SAS)。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c0c0a-106">SAS 令牌的有效期为1小时。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="c0c0a-107">仅为[CSV 数据提供程序](../resources/educationcsvdataprovider.md)提供上载 URL。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="c0c0a-108">**注意:** 若要使用 SAS 令牌访问 blob 存储, 请使用[Azure 存储 sdk](https://github.com/search?q=org%3AAzure+azure-storage)或[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c0a-109">权限</span><span class="sxs-lookup"><span data-stu-id="c0c0a-109">Permissions</span></span>
<span data-ttu-id="c0c0a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0c0a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0c0a-112">Permission type</span></span> | <span data-ttu-id="c0c0a-113">权限</span><span class="sxs-lookup"><span data-stu-id="c0c0a-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c0c0a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0c0a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c0a-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c0a-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c0c0a-116">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c0c0a-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c0c0a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-117">Not supported.</span></span>|
|<span data-ttu-id="c0c0a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0c0a-118">Application</span></span>|<span data-ttu-id="c0c0a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c0a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0c0a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="c0c0a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0c0a-121">Request headers</span></span>
| <span data-ttu-id="c0c0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="c0c0a-122">Name</span></span>       | <span data-ttu-id="c0c0a-123">类型</span><span class="sxs-lookup"><span data-stu-id="c0c0a-123">Type</span></span> | <span data-ttu-id="c0c0a-124">说明</span><span class="sxs-lookup"><span data-stu-id="c0c0a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0c0a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c0a-125">Authorization</span></span>  | <span data-ttu-id="c0c0a-126">string</span><span class="sxs-lookup"><span data-stu-id="c0c0a-126">string</span></span>  | <span data-ttu-id="c0c0a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0c0a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0c0a-129">Request body</span></span>
<span data-ttu-id="c0c0a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0c0a-131">响应</span><span class="sxs-lookup"><span data-stu-id="c0c0a-131">Response</span></span>
<span data-ttu-id="c0c0a-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)的 SAS URL。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="c0c0a-133">如果仍在处理前一个请求, 则此方法将返回`409 Conflict`一个指示当前已为[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)阻止了上载。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="c0c0a-134">示例</span><span class="sxs-lookup"><span data-stu-id="c0c0a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0c0a-135">请求</span><span class="sxs-lookup"><span data-stu-id="c0c0a-135">Request</span></span>
<span data-ttu-id="c0c0a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="c0c0a-137">响应</span><span class="sxs-lookup"><span data-stu-id="c0c0a-137">Response</span></span>
<span data-ttu-id="c0c0a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c0c0a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0c0a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
