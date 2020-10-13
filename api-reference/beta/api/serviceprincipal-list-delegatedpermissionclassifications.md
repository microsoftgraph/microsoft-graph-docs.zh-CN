---
title: 列出 delegatedPermissionClassifications 集合的 servicePrincipal
description: 检索给定给 API 的服务主体公开的委派权限的分类列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: cb2b347917642eeed7a4ca07ecd4b1984514ae16
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433520"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="49b5e-103">列出 delegatedPermissionClassifications 集合的 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="49b5e-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="49b5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49b5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49b5e-105">检索当前为 API 公开的委派权限配置的 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="49b5e-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="49b5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="49b5e-106">Permissions</span></span>

<span data-ttu-id="49b5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49b5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49b5e-109">Permission type</span></span>      | <span data-ttu-id="49b5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49b5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49b5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49b5e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49b5e-112">Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="49b5e-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="49b5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49b5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49b5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49b5e-114">Not supported.</span></span>    |
|<span data-ttu-id="49b5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49b5e-115">Application</span></span> | <span data-ttu-id="49b5e-116">Application.readwrite.ownedby、Application、read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="49b5e-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49b5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49b5e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49b5e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49b5e-118">Optional query parameters</span></span>

<span data-ttu-id="49b5e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="49b5e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49b5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49b5e-120">Request headers</span></span>

| <span data-ttu-id="49b5e-121">名称</span><span class="sxs-lookup"><span data-stu-id="49b5e-121">Name</span></span>           | <span data-ttu-id="49b5e-122">说明</span><span class="sxs-lookup"><span data-stu-id="49b5e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="49b5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49b5e-123">Authorization</span></span>  | <span data-ttu-id="49b5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49b5e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49b5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="49b5e-126">Request body</span></span>

<span data-ttu-id="49b5e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49b5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49b5e-128">响应</span><span class="sxs-lookup"><span data-stu-id="49b5e-128">Response</span></span>

<span data-ttu-id="49b5e-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="49b5e-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b5e-130">示例</span><span class="sxs-lookup"><span data-stu-id="49b5e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49b5e-131">请求</span><span class="sxs-lookup"><span data-stu-id="49b5e-131">Request</span></span>

<span data-ttu-id="49b5e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49b5e-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
```

### <a name="response"></a><span data-ttu-id="49b5e-133">响应</span><span class="sxs-lookup"><span data-stu-id="49b5e-133">Response</span></span>

<span data-ttu-id="49b5e-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49b5e-134">The following is an example of the response.</span></span>

> <span data-ttu-id="49b5e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49b5e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id": "2G3-4TG6YU2J54hjnaRoPQE",
        "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
        "permissionName": "User.Read",
        "classification": "low"
    }
  ]
}
```
