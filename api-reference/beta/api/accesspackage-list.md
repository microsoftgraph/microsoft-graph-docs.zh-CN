---
title: 列出 accessPackages
description: 检索 accessPackage 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 219d5a53c6b20666c4727430ccae6bebee9bb325
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935265"
---
# <a name="list-accesspackages"></a><span data-ttu-id="51190-103">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="51190-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51190-104">检索[accessPackage](../resources/accesspackage.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="51190-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="51190-105">生成的列表包括呼叫者有权读取的所有目录中的所有 access 程序包。</span><span class="sxs-lookup"><span data-stu-id="51190-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="51190-106">权限</span><span class="sxs-lookup"><span data-stu-id="51190-106">Permissions</span></span>

<span data-ttu-id="51190-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51190-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51190-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="51190-109">Permission type</span></span>                        | <span data-ttu-id="51190-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51190-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51190-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51190-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="51190-112">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="51190-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="51190-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51190-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51190-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="51190-114">Not supported.</span></span> |
| <span data-ttu-id="51190-115">Application</span><span class="sxs-lookup"><span data-stu-id="51190-115">Application</span></span>                            | <span data-ttu-id="51190-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51190-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51190-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51190-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51190-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="51190-118">Optional query parameters</span></span>

<span data-ttu-id="51190-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="51190-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="51190-120">例如，若要检索每个访问程序包的访问程序包策略，请`$expand=accessPackageAssignmentPolicies`添加。</span><span class="sxs-lookup"><span data-stu-id="51190-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="51190-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="51190-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="51190-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="51190-122">Request headers</span></span>

| <span data-ttu-id="51190-123">名称</span><span class="sxs-lookup"><span data-stu-id="51190-123">Name</span></span>      |<span data-ttu-id="51190-124">说明</span><span class="sxs-lookup"><span data-stu-id="51190-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51190-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51190-125">Authorization</span></span> | <span data-ttu-id="51190-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="51190-126">Bearer \{token\}.</span></span> <span data-ttu-id="51190-127">必填。</span><span class="sxs-lookup"><span data-stu-id="51190-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51190-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="51190-128">Request body</span></span>

<span data-ttu-id="51190-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51190-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51190-130">响应</span><span class="sxs-lookup"><span data-stu-id="51190-130">Response</span></span>

<span data-ttu-id="51190-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackage](../resources/accesspackage.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="51190-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51190-132">示例</span><span class="sxs-lookup"><span data-stu-id="51190-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51190-133">请求</span><span class="sxs-lookup"><span data-stu-id="51190-133">Request</span></span>

<span data-ttu-id="51190-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="51190-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```

### <a name="response"></a><span data-ttu-id="51190-135">响应</span><span class="sxs-lookup"><span data-stu-id="51190-135">Response</span></span>

<span data-ttu-id="51190-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="51190-136">The following is an example of the response.</span></span>

> <span data-ttu-id="51190-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="51190-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package",
      "displayName":"Access package for testing",
      "isHidden":false,
      "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
      "isRoleScopesVisible":false,
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->