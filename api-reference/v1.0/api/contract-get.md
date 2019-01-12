---
title: 获取 Contract
description: 检索 contract 对象的属性和关系。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba6ba3dd1e0dc631f5aeb61dd6d714e9d7a81bb6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917424"
---
# <a name="get-contract"></a><span data-ttu-id="19a85-103">获取 Contract</span><span class="sxs-lookup"><span data-stu-id="19a85-103">Get Contract</span></span>

<span data-ttu-id="19a85-104">检索 [contract](../resources/contract.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19a85-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a85-105">权限</span><span class="sxs-lookup"><span data-stu-id="19a85-105">Permissions</span></span>

<span data-ttu-id="19a85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19a85-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19a85-108">Permission type</span></span>      | <span data-ttu-id="19a85-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19a85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19a85-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19a85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19a85-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19a85-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19a85-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19a85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a85-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19a85-113">Not supported.</span></span>    |
|<span data-ttu-id="19a85-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19a85-114">Application</span></span> | <span data-ttu-id="19a85-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a85-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a85-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19a85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19a85-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19a85-117">Optional query parameters</span></span>

<span data-ttu-id="19a85-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19a85-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19a85-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19a85-119">Request headers</span></span>

| <span data-ttu-id="19a85-120">名称</span><span class="sxs-lookup"><span data-stu-id="19a85-120">Name</span></span>      |<span data-ttu-id="19a85-121">说明</span><span class="sxs-lookup"><span data-stu-id="19a85-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19a85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a85-122">Authorization</span></span>  | <span data-ttu-id="19a85-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19a85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a85-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="19a85-125">Request body</span></span>

<span data-ttu-id="19a85-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19a85-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a85-127">响应</span><span class="sxs-lookup"><span data-stu-id="19a85-127">Response</span></span>

<span data-ttu-id="19a85-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contract](../resources/contract.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19a85-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a85-129">示例</span><span class="sxs-lookup"><span data-stu-id="19a85-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19a85-130">请求</span><span class="sxs-lookup"><span data-stu-id="19a85-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="19a85-131">响应</span><span class="sxs-lookup"><span data-stu-id="19a85-131">Response</span></span>
<span data-ttu-id="19a85-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19a85-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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
