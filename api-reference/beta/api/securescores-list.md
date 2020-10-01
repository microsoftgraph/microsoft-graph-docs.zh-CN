---
title: 列出 secureScores
description: 检索 secureScores 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: dc22a2c3e37d6c8303636e5033a55b016505b232
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330149"
---
# <a name="list-securescores"></a><span data-ttu-id="4d866-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="4d866-103">List secureScores</span></span>

<span data-ttu-id="4d866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d866-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d866-105">检索 [secureScores](../resources/securescores.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d866-105">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d866-106">权限</span><span class="sxs-lookup"><span data-stu-id="4d866-106">Permissions</span></span>

<span data-ttu-id="4d866-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d866-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d866-109">Permission type</span></span>      | <span data-ttu-id="4d866-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d866-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d866-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d866-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4d866-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d866-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="4d866-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d866-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4d866-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d866-114">Not supported.</span></span>  |
|<span data-ttu-id="4d866-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d866-115">Application</span></span> | <span data-ttu-id="4d866-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d866-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d866-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d866-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="4d866-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d866-118">Request headers</span></span>

| <span data-ttu-id="4d866-119">名称</span><span class="sxs-lookup"><span data-stu-id="4d866-119">Name</span></span>      |<span data-ttu-id="4d866-120">说明</span><span class="sxs-lookup"><span data-stu-id="4d866-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d866-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d866-121">Authorization</span></span>  | <span data-ttu-id="4d866-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="4d866-122">Bearer {code}.</span></span> <span data-ttu-id="4d866-123">必需。</span><span class="sxs-lookup"><span data-stu-id="4d866-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d866-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d866-124">Request body</span></span>

<span data-ttu-id="4d866-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d866-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d866-126">响应</span><span class="sxs-lookup"><span data-stu-id="4d866-126">Response</span></span>

<span data-ttu-id="4d866-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **secureScores** 对象。</span><span class="sxs-lookup"><span data-stu-id="4d866-127">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d866-128">示例</span><span class="sxs-lookup"><span data-stu-id="4d866-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d866-129">请求</span><span class="sxs-lookup"><span data-stu-id="4d866-129">Request</span></span>

<span data-ttu-id="4d866-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d866-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d866-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d866-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="4d866-132">C#</span><span class="sxs-lookup"><span data-stu-id="4d866-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d866-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d866-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d866-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d866-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d866-135">响应</span><span class="sxs-lookup"><span data-stu-id="4d866-135">Response</span></span>

<span data-ttu-id="4d866-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d866-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


