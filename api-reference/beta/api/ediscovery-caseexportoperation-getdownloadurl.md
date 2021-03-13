---
title: caseExportOperation： getDownloadUrl
description: '返回下载 URL '
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7e7f683d034f6c693cfdd16e96755471629e2a94
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773289"
---
# <a name="caseexportoperation-getdownloadurl"></a><span data-ttu-id="271b1-103">caseExportOperation： getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="271b1-103">caseExportOperation: getDownloadUrl</span></span>

<span data-ttu-id="271b1-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="271b1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="271b1-105">返回导出准备就绪时导出的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="271b1-105">Returns the download URL for an export when the export is ready.</span></span>

## <a name="permissions"></a><span data-ttu-id="271b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="271b1-106">Permissions</span></span>

<span data-ttu-id="271b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="271b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="271b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="271b1-109">Permission type</span></span>|<span data-ttu-id="271b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="271b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="271b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="271b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="271b1-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271b1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="271b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="271b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="271b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="271b1-114">Not supported.</span></span>|
|<span data-ttu-id="271b1-115">Application</span><span class="sxs-lookup"><span data-stu-id="271b1-115">Application</span></span>|<span data-ttu-id="271b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="271b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="271b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="271b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations/{operationId}/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="271b1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="271b1-118">Request headers</span></span>
|<span data-ttu-id="271b1-119">名称</span><span class="sxs-lookup"><span data-stu-id="271b1-119">Name</span></span>|<span data-ttu-id="271b1-120">说明</span><span class="sxs-lookup"><span data-stu-id="271b1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="271b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="271b1-121">Authorization</span></span>|<span data-ttu-id="271b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="271b1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="271b1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="271b1-124">Request body</span></span>
<span data-ttu-id="271b1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="271b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="271b1-126">响应</span><span class="sxs-lookup"><span data-stu-id="271b1-126">Response</span></span>

<span data-ttu-id="271b1-127">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 String。</span><span class="sxs-lookup"><span data-stu-id="271b1-127">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span> <span data-ttu-id="271b1-128">值字段表示可从中检索导出的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="271b1-128">The value field represents the download URL from where the export can be retrieved.</span></span>

## <a name="examples"></a><span data-ttu-id="271b1-129">示例</span><span class="sxs-lookup"><span data-stu-id="271b1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="271b1-130">请求</span><span class="sxs-lookup"><span data-stu-id="271b1-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="271b1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="271b1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "caseexportoperation_getdownloadurl"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```
# <a name="c"></a>[<span data-ttu-id="271b1-132">C#</span><span class="sxs-lookup"><span data-stu-id="271b1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/caseexportoperation-getdownloadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="271b1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="271b1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/caseexportoperation-getdownloadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="271b1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="271b1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/caseexportoperation-getdownloadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="271b1-135">Java</span><span class="sxs-lookup"><span data-stu-id="271b1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/caseexportoperation-getdownloadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="271b1-136">响应</span><span class="sxs-lookup"><span data-stu-id="271b1-136">Response</span></span>

<span data-ttu-id="271b1-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="271b1-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
