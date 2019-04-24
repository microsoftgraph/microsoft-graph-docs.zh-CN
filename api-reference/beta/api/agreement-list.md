---
title: 列出协议
description: 检索协议对象的列表。
localization_priority: Normal
ms.openlocfilehash: 82674e81b6b059ffafedf3b9c15c19e90438dc28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459199"
---
# <a name="list-agreements"></a><span data-ttu-id="af0aa-103">列出协议</span><span class="sxs-lookup"><span data-stu-id="af0aa-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af0aa-104">检索[协议](../resources/agreement.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="af0aa-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="af0aa-105">权限</span><span class="sxs-lookup"><span data-stu-id="af0aa-105">Permissions</span></span>
<span data-ttu-id="af0aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af0aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af0aa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="af0aa-108">Permission type</span></span>                        | <span data-ttu-id="af0aa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af0aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af0aa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af0aa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="af0aa-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="af0aa-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="af0aa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af0aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af0aa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="af0aa-113">Not supported.</span></span> |
|<span data-ttu-id="af0aa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="af0aa-114">Application</span></span>                            | <span data-ttu-id="af0aa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af0aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af0aa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af0aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="af0aa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="af0aa-117">Request headers</span></span>
| <span data-ttu-id="af0aa-118">名称</span><span class="sxs-lookup"><span data-stu-id="af0aa-118">Name</span></span>         | <span data-ttu-id="af0aa-119">类型</span><span class="sxs-lookup"><span data-stu-id="af0aa-119">Type</span></span>        | <span data-ttu-id="af0aa-120">说明</span><span class="sxs-lookup"><span data-stu-id="af0aa-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af0aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af0aa-121">Authorization</span></span> | <span data-ttu-id="af0aa-122">string</span><span class="sxs-lookup"><span data-stu-id="af0aa-122">string</span></span> | <span data-ttu-id="af0aa-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="af0aa-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af0aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="af0aa-125">Request body</span></span>
<span data-ttu-id="af0aa-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af0aa-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="af0aa-127">响应</span><span class="sxs-lookup"><span data-stu-id="af0aa-127">Response</span></span>
<span data-ttu-id="af0aa-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[协议](../resources/agreement.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="af0aa-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af0aa-129">示例</span><span class="sxs-lookup"><span data-stu-id="af0aa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af0aa-130">请求</span><span class="sxs-lookup"><span data-stu-id="af0aa-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="af0aa-131">响应</span><span class="sxs-lookup"><span data-stu-id="af0aa-131">Response</span></span>
><span data-ttu-id="af0aa-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="af0aa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
