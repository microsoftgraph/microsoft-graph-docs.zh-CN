---
title: 列出 appliesTo
description: 获取已应用 claimsMappingPolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f749b040da90537ad362fe1d372ae6d090327039
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982526"
---
# <a name="list-appliesto"></a><span data-ttu-id="a2027-103">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="a2027-103">List appliesTo</span></span>

<span data-ttu-id="a2027-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2027-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2027-105">获取已应用[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a2027-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="a2027-106">ClaimsMappingPolicy 只能应用于 [application](../resources/application.md) 和 [servicePrincipal](../resources/serviceprincipal.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a2027-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2027-107">权限</span><span class="sxs-lookup"><span data-stu-id="a2027-107">Permissions</span></span>

<span data-ttu-id="a2027-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2027-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2027-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2027-110">Permission type</span></span>                        | <span data-ttu-id="a2027-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2027-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a2027-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2027-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2027-113">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="a2027-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="a2027-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2027-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2027-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2027-115">Not supported.</span></span> |
| <span data-ttu-id="a2027-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2027-116">Application</span></span>                            | <span data-ttu-id="a2027-117">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="a2027-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2027-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2027-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2027-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a2027-119">Optional query parameters</span></span>

<span data-ttu-id="a2027-120">此方法支持 `$expand` `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2027-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a2027-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a2027-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="a2027-122">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="a2027-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2027-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2027-123">Request headers</span></span>

| <span data-ttu-id="a2027-124">名称</span><span class="sxs-lookup"><span data-stu-id="a2027-124">Name</span></span>      |<span data-ttu-id="a2027-125">说明</span><span class="sxs-lookup"><span data-stu-id="a2027-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2027-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2027-126">Authorization</span></span> | <span data-ttu-id="a2027-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a2027-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2027-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2027-128">Request body</span></span>

<span data-ttu-id="a2027-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2027-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2027-130">响应</span><span class="sxs-lookup"><span data-stu-id="a2027-130">Response</span></span>

<span data-ttu-id="a2027-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2027-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2027-132">示例</span><span class="sxs-lookup"><span data-stu-id="a2027-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2027-133">请求</span><span class="sxs-lookup"><span data-stu-id="a2027-133">Request</span></span>

<span data-ttu-id="a2027-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2027-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/claimsMappingPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="a2027-135">响应</span><span class="sxs-lookup"><span data-stu-id="a2027-135">Response</span></span>

<span data-ttu-id="a2027-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2027-136">The following is an example of the response.</span></span>

> <span data-ttu-id="a2027-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a2027-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

