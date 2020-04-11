---
title: 列出 tokenLifetimePolicies
description: 获取 tokenLifetimePolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8ef186128a428b9bc999a14fc61a588a4eb7859
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229540"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="78c8f-103">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="78c8f-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="78c8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78c8f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="78c8f-105">获取[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="78c8f-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="78c8f-106">权限</span><span class="sxs-lookup"><span data-stu-id="78c8f-106">Permissions</span></span>

<span data-ttu-id="78c8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78c8f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="78c8f-109">Permission type</span></span>                        | <span data-ttu-id="78c8f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78c8f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="78c8f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78c8f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="78c8f-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="78c8f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="78c8f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78c8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78c8f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78c8f-114">Not supported.</span></span> |
| <span data-ttu-id="78c8f-115">Application</span><span class="sxs-lookup"><span data-stu-id="78c8f-115">Application</span></span>                            | <span data-ttu-id="78c8f-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="78c8f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="78c8f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78c8f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78c8f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78c8f-118">Optional query parameters</span></span>

<span data-ttu-id="78c8f-119">`$expand`此方法支持`$filter`、 `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78c8f-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="78c8f-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="78c8f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="78c8f-121">使用`$expand`时，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="78c8f-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78c8f-122">请求头</span><span class="sxs-lookup"><span data-stu-id="78c8f-122">Request headers</span></span>

| <span data-ttu-id="78c8f-123">名称</span><span class="sxs-lookup"><span data-stu-id="78c8f-123">Name</span></span>      |<span data-ttu-id="78c8f-124">说明</span><span class="sxs-lookup"><span data-stu-id="78c8f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78c8f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="78c8f-125">Authorization</span></span> | <span data-ttu-id="78c8f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78c8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78c8f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="78c8f-128">Request body</span></span>

<span data-ttu-id="78c8f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78c8f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78c8f-130">响应</span><span class="sxs-lookup"><span data-stu-id="78c8f-130">Response</span></span>

<span data-ttu-id="78c8f-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="78c8f-131">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78c8f-132">示例</span><span class="sxs-lookup"><span data-stu-id="78c8f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78c8f-133">请求</span><span class="sxs-lookup"><span data-stu-id="78c8f-133">Request</span></span>

<span data-ttu-id="78c8f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="78c8f-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="78c8f-135">响应</span><span class="sxs-lookup"><span data-stu-id="78c8f-135">Response</span></span>

<span data-ttu-id="78c8f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78c8f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="78c8f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78c8f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
