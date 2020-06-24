---
title: 列出 appliesTo
description: 获取已应用 claimsMappingPolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f821e3f5878867dd00af71fead543b99e30ec06b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846232"
---
# <a name="list-appliesto"></a><span data-ttu-id="ba76a-103">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="ba76a-103">List appliesTo</span></span>

<span data-ttu-id="ba76a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba76a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba76a-105">获取已应用[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ba76a-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="ba76a-106">ClaimsMappingPolicy 只能应用于[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)资源。</span><span class="sxs-lookup"><span data-stu-id="ba76a-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba76a-107">权限</span><span class="sxs-lookup"><span data-stu-id="ba76a-107">Permissions</span></span>

<span data-ttu-id="ba76a-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ba76a-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ba76a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba76a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba76a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba76a-110">Permission type</span></span>                        | <span data-ttu-id="ba76a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba76a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba76a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba76a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba76a-113">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="ba76a-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ba76a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba76a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba76a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba76a-115">Not supported.</span></span> |
| <span data-ttu-id="ba76a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba76a-116">Application</span></span>                            | <span data-ttu-id="ba76a-117">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="ba76a-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba76a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba76a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba76a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba76a-119">Optional query parameters</span></span>

<span data-ttu-id="ba76a-120">此方法支持 `$expand` `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba76a-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba76a-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ba76a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ba76a-122">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="ba76a-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba76a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba76a-123">Request headers</span></span>

| <span data-ttu-id="ba76a-124">名称</span><span class="sxs-lookup"><span data-stu-id="ba76a-124">Name</span></span>      |<span data-ttu-id="ba76a-125">说明</span><span class="sxs-lookup"><span data-stu-id="ba76a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba76a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba76a-126">Authorization</span></span> | <span data-ttu-id="ba76a-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ba76a-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba76a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba76a-128">Request body</span></span>

<span data-ttu-id="ba76a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba76a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba76a-130">响应</span><span class="sxs-lookup"><span data-stu-id="ba76a-130">Response</span></span>

<span data-ttu-id="ba76a-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba76a-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba76a-132">示例</span><span class="sxs-lookup"><span data-stu-id="ba76a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba76a-133">请求</span><span class="sxs-lookup"><span data-stu-id="ba76a-133">Request</span></span>

<span data-ttu-id="ba76a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba76a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/v1.0/claimsMappingPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="ba76a-135">响应</span><span class="sxs-lookup"><span data-stu-id="ba76a-135">Response</span></span>

<span data-ttu-id="ba76a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba76a-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ba76a-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="ba76a-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba76a-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ba76a-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->