---
title: 列出 contract
description: 检索与合作伙伴租户关联的 contract 对象列表。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6df390cbe742443bf8a996362fa2cf2909ef83f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971072"
---
# <a name="list-contracts"></a><span data-ttu-id="9612b-103">列出 contract</span><span class="sxs-lookup"><span data-stu-id="9612b-103">List contracts</span></span>

> <span data-ttu-id="9612b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9612b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9612b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9612b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9612b-106">检索与合作伙伴租户关联的 [contract](../resources/contract.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9612b-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9612b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9612b-107">Permissions</span></span>

<span data-ttu-id="9612b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9612b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9612b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9612b-110">Permission type</span></span>      | <span data-ttu-id="9612b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9612b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9612b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9612b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9612b-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9612b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9612b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9612b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9612b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9612b-115">Not supported.</span></span>    |
|<span data-ttu-id="9612b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9612b-116">Application</span></span> | <span data-ttu-id="9612b-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9612b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9612b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9612b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9612b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9612b-119">Optional query parameters</span></span>

<span data-ttu-id="9612b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9612b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="9612b-121">支持筛选 customerId、defaultDomainName 和 displayName。</span><span class="sxs-lookup"><span data-stu-id="9612b-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9612b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9612b-122">Request headers</span></span>

| <span data-ttu-id="9612b-123">名称</span><span class="sxs-lookup"><span data-stu-id="9612b-123">Name</span></span>      |<span data-ttu-id="9612b-124">说明</span><span class="sxs-lookup"><span data-stu-id="9612b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9612b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9612b-125">Authorization</span></span>  | <span data-ttu-id="9612b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9612b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9612b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9612b-128">Request body</span></span>

<span data-ttu-id="9612b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9612b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9612b-130">响应</span><span class="sxs-lookup"><span data-stu-id="9612b-130">Response</span></span>

<span data-ttu-id="9612b-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contract](../resources/contract.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9612b-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9612b-132">示例</span><span class="sxs-lookup"><span data-stu-id="9612b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9612b-133">请求</span><span class="sxs-lookup"><span data-stu-id="9612b-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="9612b-134">响应</span><span class="sxs-lookup"><span data-stu-id="9612b-134">Response</span></span>

<span data-ttu-id="9612b-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9612b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
