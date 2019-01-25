---
title: 列出 secureScores
description: 检索的属性和 secureScores 对象的关系。
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521479"
---
# <a name="list-securescores"></a><span data-ttu-id="a89d0-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="a89d0-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89d0-104">检索的属性和[secureScores](../resources/securescores.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a89d0-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a89d0-105">权限</span><span class="sxs-lookup"><span data-stu-id="a89d0-105">Permissions</span></span>

<span data-ttu-id="a89d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a89d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89d0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a89d0-108">Permission type</span></span>      | <span data-ttu-id="a89d0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a89d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89d0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a89d0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a89d0-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a89d0-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a89d0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a89d0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a89d0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a89d0-113">Not supported.</span></span>  |
|<span data-ttu-id="a89d0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a89d0-114">Application</span></span> | <span data-ttu-id="a89d0-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a89d0-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89d0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a89d0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="a89d0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a89d0-117">Request headers</span></span>

| <span data-ttu-id="a89d0-118">名称</span><span class="sxs-lookup"><span data-stu-id="a89d0-118">Name</span></span>      |<span data-ttu-id="a89d0-119">说明</span><span class="sxs-lookup"><span data-stu-id="a89d0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a89d0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a89d0-120">Authorization</span></span>  | <span data-ttu-id="a89d0-p102">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="a89d0-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89d0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a89d0-123">Request body</span></span>

<span data-ttu-id="a89d0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a89d0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89d0-125">响应</span><span class="sxs-lookup"><span data-stu-id="a89d0-125">Response</span></span>

<span data-ttu-id="a89d0-126">如果成功，此方法返回`200 OK`响应代码和响应正文中的**secureScores**对象。</span><span class="sxs-lookup"><span data-stu-id="a89d0-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89d0-127">示例</span><span class="sxs-lookup"><span data-stu-id="a89d0-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="a89d0-128">请求</span><span class="sxs-lookup"><span data-stu-id="a89d0-128">Request</span></span>

<span data-ttu-id="a89d0-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a89d0-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="a89d0-130">响应</span><span class="sxs-lookup"><span data-stu-id="a89d0-130">Response</span></span>

<span data-ttu-id="a89d0-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a89d0-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
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
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
