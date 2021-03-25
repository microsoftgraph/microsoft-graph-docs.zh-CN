---
title: Assign appliesTo
description: 将 directoryObject 分配给功能推出。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8bafd8a2ec3e869ccd20f5aa800be4e63f20ba16
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201312"
---
# <a name="assign-appliesto"></a><span data-ttu-id="e9a0c-103">Assign appliesTo</span><span class="sxs-lookup"><span data-stu-id="e9a0c-103">Assign appliesTo</span></span>

<span data-ttu-id="e9a0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9a0c-105">在[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象上添加一个 appliesTo，以指定应应用[featureRolloutPolicy](../resources/featurerolloutpolicy.md)的[directoryObject。](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e9a0c-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a0c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9a0c-106">Permissions</span></span>

<span data-ttu-id="e9a0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9a0c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9a0c-109">Permission type</span></span>                        | <span data-ttu-id="e9a0c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9a0c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9a0c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9a0c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9a0c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9a0c-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="e9a0c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9a0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a0c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-114">Not supported.</span></span> |
| <span data-ttu-id="e9a0c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9a0c-115">Application</span></span>                            | <span data-ttu-id="e9a0c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9a0c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9a0c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e9a0c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9a0c-118">Request headers</span></span>

| <span data-ttu-id="e9a0c-119">名称</span><span class="sxs-lookup"><span data-stu-id="e9a0c-119">Name</span></span>          | <span data-ttu-id="e9a0c-120">说明</span><span class="sxs-lookup"><span data-stu-id="e9a0c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9a0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9a0c-121">Authorization</span></span> | <span data-ttu-id="e9a0c-122">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-122">Bearer {token}.</span></span> <span data-ttu-id="e9a0c-123">必需</span><span class="sxs-lookup"><span data-stu-id="e9a0c-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a0c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9a0c-124">Request body</span></span>

<span data-ttu-id="e9a0c-125">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e9a0c-126">响应</span><span class="sxs-lookup"><span data-stu-id="e9a0c-126">Response</span></span>

<span data-ttu-id="e9a0c-127">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-127">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9a0c-128">示例</span><span class="sxs-lookup"><span data-stu-id="e9a0c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9a0c-129">请求</span><span class="sxs-lookup"><span data-stu-id="e9a0c-129">Request</span></span>

<span data-ttu-id="e9a0c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e9a0c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a0c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```
# <a name="c"></a>[<span data-ttu-id="e9a0c-132">C#</span><span class="sxs-lookup"><span data-stu-id="e9a0c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9a0c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9a0c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9a0c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9a0c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9a0c-135">Java</span><span class="sxs-lookup"><span data-stu-id="e9a0c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9a0c-136">响应</span><span class="sxs-lookup"><span data-stu-id="e9a0c-136">Response</span></span>

<span data-ttu-id="e9a0c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e9a0c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e9a0c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryObject": {
    "id": "2441b489-4f12-4882-b039-8f6006bd66da",
    "objectType": "group"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


