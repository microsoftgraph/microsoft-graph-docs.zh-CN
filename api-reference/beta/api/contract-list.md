---
title: 列出 contract
description: 检索与合作伙伴租户关联的 contract 对象列表。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4161e6f4cfabaf5d2e4b23bef8007fd8a6c65c45
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520779"
---
# <a name="list-contracts"></a><span data-ttu-id="9765f-103">列出 contract</span><span class="sxs-lookup"><span data-stu-id="9765f-103">List contracts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9765f-104">检索与合作伙伴租户关联的 [contract](../resources/contract.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9765f-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9765f-105">权限</span><span class="sxs-lookup"><span data-stu-id="9765f-105">Permissions</span></span>

<span data-ttu-id="9765f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9765f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9765f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9765f-108">Permission type</span></span>      | <span data-ttu-id="9765f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9765f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9765f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9765f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9765f-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9765f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9765f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9765f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9765f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9765f-113">Not supported.</span></span>    |
|<span data-ttu-id="9765f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9765f-114">Application</span></span> | <span data-ttu-id="9765f-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9765f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9765f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9765f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9765f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9765f-117">Optional query parameters</span></span>

<span data-ttu-id="9765f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9765f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="9765f-119">支持筛选 customerId、defaultDomainName 和 displayName。</span><span class="sxs-lookup"><span data-stu-id="9765f-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9765f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9765f-120">Request headers</span></span>

| <span data-ttu-id="9765f-121">名称</span><span class="sxs-lookup"><span data-stu-id="9765f-121">Name</span></span>      |<span data-ttu-id="9765f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9765f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9765f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9765f-123">Authorization</span></span>  | <span data-ttu-id="9765f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9765f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9765f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9765f-126">Request body</span></span>

<span data-ttu-id="9765f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9765f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9765f-128">响应</span><span class="sxs-lookup"><span data-stu-id="9765f-128">Response</span></span>

<span data-ttu-id="9765f-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contract](../resources/contract.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9765f-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9765f-130">示例</span><span class="sxs-lookup"><span data-stu-id="9765f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9765f-131">请求</span><span class="sxs-lookup"><span data-stu-id="9765f-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="9765f-132">响应</span><span class="sxs-lookup"><span data-stu-id="9765f-132">Response</span></span>

<span data-ttu-id="9765f-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9765f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
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
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contract-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
