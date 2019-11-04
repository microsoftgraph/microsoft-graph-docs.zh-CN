---
title: 列出 accessPackageAssignmentPolicies
description: 检索 accessPackageAssignmentPolicy 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2e823980dc9966a5f3e85eef82d00c606e5c180
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935250"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="91413-103">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="91413-103">List accessPackageAssignmentPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91413-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="91413-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="91413-105">生成的列表包括呼叫者有权读取的所有目录和访问包中的所有分配策略。</span><span class="sxs-lookup"><span data-stu-id="91413-105">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="91413-106">权限</span><span class="sxs-lookup"><span data-stu-id="91413-106">Permissions</span></span>

<span data-ttu-id="91413-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91413-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91413-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91413-109">Permission type</span></span>                        | <span data-ttu-id="91413-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91413-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91413-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91413-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91413-112">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="91413-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="91413-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91413-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91413-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="91413-114">Not supported.</span></span> |
| <span data-ttu-id="91413-115">Application</span><span class="sxs-lookup"><span data-stu-id="91413-115">Application</span></span>                            | <span data-ttu-id="91413-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91413-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91413-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91413-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91413-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91413-118">Optional query parameters</span></span>

<span data-ttu-id="91413-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91413-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="91413-120">例如，若要检索具有指定显示名称的 access 程序包分配策略，请在`$filter=displayName eq 'Employee sales support'`查询中加入。</span><span class="sxs-lookup"><span data-stu-id="91413-120">For example, to retrieve a access package assignment policy with a specifed display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="91413-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="91413-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="91413-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="91413-122">Request headers</span></span>

| <span data-ttu-id="91413-123">名称</span><span class="sxs-lookup"><span data-stu-id="91413-123">Name</span></span>      |<span data-ttu-id="91413-124">说明</span><span class="sxs-lookup"><span data-stu-id="91413-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91413-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91413-125">Authorization</span></span> | <span data-ttu-id="91413-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="91413-126">Bearer \{token\}.</span></span> <span data-ttu-id="91413-127">必填。</span><span class="sxs-lookup"><span data-stu-id="91413-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91413-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="91413-128">Request body</span></span>

<span data-ttu-id="91413-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91413-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91413-130">响应</span><span class="sxs-lookup"><span data-stu-id="91413-130">Response</span></span>

<span data-ttu-id="91413-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="91413-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91413-132">示例</span><span class="sxs-lookup"><span data-stu-id="91413-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91413-133">请求</span><span class="sxs-lookup"><span data-stu-id="91413-133">Request</span></span>

<span data-ttu-id="91413-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91413-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

### <a name="response"></a><span data-ttu-id="91413-135">响应</span><span class="sxs-lookup"><span data-stu-id="91413-135">Response</span></span>

<span data-ttu-id="91413-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91413-136">The following is an example of the response.</span></span>

> <span data-ttu-id="91413-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91413-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "isEnabled": false,
      "canExtend": false,
      "durationInDays": 365
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
