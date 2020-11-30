---
title: 列表包括 permissionGrantPolicy 的集合
description: 检索描述在权限授予策略中包含权限授予事件的条件的条件集的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e85fdb159f275eb1dc4a7a31604b7d51e698288f
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377148"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="ebcd0-103">列表包括 permissionGrantPolicy 的集合</span><span class="sxs-lookup"><span data-stu-id="ebcd0-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="ebcd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebcd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebcd0-105">检索 [permissionGrantPolicy](../resources/permissiongrantpolicy.md)中 *包含* 的条件集。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebcd0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebcd0-106">Permissions</span></span>

<span data-ttu-id="ebcd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcd0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebcd0-109">Permission type</span></span>      | <span data-ttu-id="ebcd0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebcd0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcd0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcd0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebcd0-112">PermissionGrant、目录、读取。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="ebcd0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcd0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-114">Not supported.</span></span>    |
|<span data-ttu-id="ebcd0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebcd0-115">Application</span></span> | <span data-ttu-id="ebcd0-116">PermissionGrant、目录、读取。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebcd0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebcd0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebcd0-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="ebcd0-118">Optional query parameters</span></span>

<span data-ttu-id="ebcd0-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebcd0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebcd0-120">Request headers</span></span>

| <span data-ttu-id="ebcd0-121">名称</span><span class="sxs-lookup"><span data-stu-id="ebcd0-121">Name</span></span>           | <span data-ttu-id="ebcd0-122">说明</span><span class="sxs-lookup"><span data-stu-id="ebcd0-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ebcd0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebcd0-123">Authorization</span></span>  | <span data-ttu-id="ebcd0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebcd0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebcd0-126">Request body</span></span>

<span data-ttu-id="ebcd0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebcd0-128">响应</span><span class="sxs-lookup"><span data-stu-id="ebcd0-128">Response</span></span>

<span data-ttu-id="ebcd0-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebcd0-130">示例</span><span class="sxs-lookup"><span data-stu-id="ebcd0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebcd0-131">请求</span><span class="sxs-lookup"><span data-stu-id="ebcd0-131">Request</span></span>

<span data-ttu-id="ebcd0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/includes
```

### <a name="response"></a><span data-ttu-id="ebcd0-133">响应</span><span class="sxs-lookup"><span data-stu-id="ebcd0-133">Response</span></span>

<span data-ttu-id="ebcd0-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-134">The following is an example of the response.</span></span>

> <span data-ttu-id="ebcd0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ebcd0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
