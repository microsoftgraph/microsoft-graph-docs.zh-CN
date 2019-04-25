---
title: 列出域
description: 检索域对象的列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4039995fc8b588b3a6a318b457e0eaba28b8dfa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583618"
---
# <a name="list-domains"></a><span data-ttu-id="ce86d-103">列出域</span><span class="sxs-lookup"><span data-stu-id="ce86d-103">List domains</span></span>

<span data-ttu-id="ce86d-104">检索域对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ce86d-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce86d-105">权限</span><span class="sxs-lookup"><span data-stu-id="ce86d-105">Permissions</span></span>
<span data-ttu-id="ce86d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce86d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce86d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce86d-108">Permission type</span></span>      | <span data-ttu-id="ce86d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce86d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce86d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce86d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce86d-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce86d-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="ce86d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce86d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce86d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce86d-113">Not supported.</span></span>    |
|<span data-ttu-id="ce86d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce86d-114">Application</span></span> | <span data-ttu-id="ce86d-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce86d-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce86d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce86d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce86d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce86d-117">Optional query parameters</span></span>
<span data-ttu-id="ce86d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce86d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce86d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce86d-119">Request headers</span></span>
| <span data-ttu-id="ce86d-120">名称</span><span class="sxs-lookup"><span data-stu-id="ce86d-120">Name</span></span>      |<span data-ttu-id="ce86d-121">说明</span><span class="sxs-lookup"><span data-stu-id="ce86d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce86d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce86d-122">Authorization</span></span>  | <span data-ttu-id="ce86d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce86d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ce86d-125">接受</span><span class="sxs-lookup"><span data-stu-id="ce86d-125">Accept</span></span>         | <span data-ttu-id="ce86d-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="ce86d-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce86d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce86d-127">Request body</span></span>
<span data-ttu-id="ce86d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce86d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce86d-129">响应</span><span class="sxs-lookup"><span data-stu-id="ce86d-129">Response</span></span>

<span data-ttu-id="ce86d-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[domain](../resources/domain.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ce86d-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce86d-131">示例</span><span class="sxs-lookup"><span data-stu-id="ce86d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce86d-132">请求</span><span class="sxs-lookup"><span data-stu-id="ce86d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="ce86d-133">响应</span><span class="sxs-lookup"><span data-stu-id="ce86d-133">Response</span></span>
<span data-ttu-id="ce86d-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce86d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
