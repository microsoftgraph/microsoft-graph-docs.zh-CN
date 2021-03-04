---
title: 列表标记
description: 从电子数据展示案例获取标记资源列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 936a1db060df423ec104170b971bc43c7fd3f69c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446088"
---
# <a name="list-tags"></a><span data-ttu-id="1584d-103">列表标记</span><span class="sxs-lookup"><span data-stu-id="1584d-103">List tags</span></span>

<span data-ttu-id="1584d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1584d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1584d-105">从电子数据展示 [案例](../resources/ediscovery-tag.md) 检索标记对象 [的列表](../resources/ediscovery-case.md)。</span><span class="sxs-lookup"><span data-stu-id="1584d-105">Retrieve a list of [tag](../resources/ediscovery-tag.md) objects from an eDiscovery [case](../resources/ediscovery-case.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1584d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1584d-106">Permissions</span></span>

<span data-ttu-id="1584d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1584d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1584d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1584d-109">Permission type</span></span>|<span data-ttu-id="1584d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1584d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1584d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1584d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1584d-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1584d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1584d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1584d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1584d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1584d-114">Not supported.</span></span>|
|<span data-ttu-id="1584d-115">Application</span><span class="sxs-lookup"><span data-stu-id="1584d-115">Application</span></span>|<span data-ttu-id="1584d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1584d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1584d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1584d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1584d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1584d-118">Optional query parameters</span></span>

<span data-ttu-id="1584d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1584d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1584d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1584d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1584d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1584d-121">Request headers</span></span>

|<span data-ttu-id="1584d-122">名称</span><span class="sxs-lookup"><span data-stu-id="1584d-122">Name</span></span>|<span data-ttu-id="1584d-123">说明</span><span class="sxs-lookup"><span data-stu-id="1584d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1584d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1584d-124">Authorization</span></span>|<span data-ttu-id="1584d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1584d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1584d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1584d-127">Request body</span></span>

<span data-ttu-id="1584d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1584d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1584d-129">响应</span><span class="sxs-lookup"><span data-stu-id="1584d-129">Response</span></span>

<span data-ttu-id="1584d-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1584d-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1584d-131">示例</span><span class="sxs-lookup"><span data-stu-id="1584d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1584d-132">请求</span><span class="sxs-lookup"><span data-stu-id="1584d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
```

### <a name="response"></a><span data-ttu-id="1584d-133">响应</span><span class="sxs-lookup"><span data-stu-id="1584d-133">Response</span></span>

<span data-ttu-id="1584d-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1584d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.tag)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags",
    "value": [
        {
            "displayName": "Responsiveness",
            "description": "Indicates the responsiveness of the document",
            "lastModifiedDateTime": "2021-01-11T19:32:23.1903658Z",
            "childSelectability": "One",
            "id": "e54b3f535b434a9a8743b84e34c00504",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "parent": null,
            "childTags": []
        },
        {
            "displayName": "Yes",
            "description": "The document is responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:22.4091161Z",
            "childSelectability": "One",
            "id": "081ff31e7324423186e01b549efe7033",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "parent": {
                "displayName": null,
                "createdBy": null,
                "description": null,
                "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                "childSelectability": "One",
                "id": "e54b3f535b434a9a8743b84e34c00504"
            },
            "childTags": []
        },
        {
            "displayName": "No",
            "description": "The document is not responsive",
            "lastModifiedDateTime": "2021-01-11T19:32:21.5693878Z",
            "childSelectability": "One",
            "id": "61624e6c96a64ccea40e0d2c48e23e16",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "EDisco Admin",
                    "userPrincipalName": "admin@contoso.com"
                }
            },
            "parent": {
                "displayName": null,
                "createdBy": null,
                "description": null,
                "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                "childSelectability": "One",
                "id": "e54b3f535b434a9a8743b84e34c00504"
            },
            "childTags": []
        }
    ]
}
```
