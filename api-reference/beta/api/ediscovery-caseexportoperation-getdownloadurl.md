---
title: caseExportOperation： getDownloadUrl
description: '返回下载 URL '
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f05c7a63dce306ff07993e6111a9323c6a14d599
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446068"
---
# <a name="caseexportoperation-getdownloadurl"></a><span data-ttu-id="3bca3-103">caseExportOperation： getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="3bca3-103">caseExportOperation: getDownloadUrl</span></span>

<span data-ttu-id="3bca3-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3bca3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bca3-105">返回导出准备就绪时导出的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3bca3-105">Returns the download URL for an export when the export is ready.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bca3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3bca3-106">Permissions</span></span>

<span data-ttu-id="3bca3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bca3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bca3-109">Permission type</span></span>|<span data-ttu-id="3bca3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bca3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bca3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bca3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bca3-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bca3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3bca3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bca3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bca3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bca3-114">Not supported.</span></span>|
|<span data-ttu-id="3bca3-115">Application</span><span class="sxs-lookup"><span data-stu-id="3bca3-115">Application</span></span>|<span data-ttu-id="3bca3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bca3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bca3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bca3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations/{operationId}/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="3bca3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bca3-118">Request headers</span></span>
|<span data-ttu-id="3bca3-119">名称</span><span class="sxs-lookup"><span data-stu-id="3bca3-119">Name</span></span>|<span data-ttu-id="3bca3-120">说明</span><span class="sxs-lookup"><span data-stu-id="3bca3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3bca3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bca3-121">Authorization</span></span>|<span data-ttu-id="3bca3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3bca3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bca3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bca3-124">Request body</span></span>
<span data-ttu-id="3bca3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3bca3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bca3-126">响应</span><span class="sxs-lookup"><span data-stu-id="3bca3-126">Response</span></span>

<span data-ttu-id="3bca3-127">如果成功，此函数在响应正文中返回响应 `200 OK` 代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="3bca3-127">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span> <span data-ttu-id="3bca3-128">值字段表示可从中检索导出的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3bca3-128">The value field represents the download URL from where the export can be retrieved.</span></span>

## <a name="examples"></a><span data-ttu-id="3bca3-129">示例</span><span class="sxs-lookup"><span data-stu-id="3bca3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3bca3-130">请求</span><span class="sxs-lookup"><span data-stu-id="3bca3-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "caseexportoperation_getdownloadurl"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

### <a name="response"></a><span data-ttu-id="3bca3-131">响应</span><span class="sxs-lookup"><span data-stu-id="3bca3-131">Response</span></span>

<span data-ttu-id="3bca3-132">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3bca3-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://nam01pkgg0052.blob.edproxy.nam01.ediscovery.outlook.com/packaging0041e27c6c924a48befe348d34066c25/d0b6d2a7-5fc5-44f0-9bca-6b9d34a9410b.zip?sv=2018-03-28&sr=c&sig=TRFQNUGFtuVO7zd39oNJjzcQYJus2TXY%2B50aed4pJJM%3D&se=2020-12-28T23%3A06%3A26Z&sp=racwdl"
}
```
