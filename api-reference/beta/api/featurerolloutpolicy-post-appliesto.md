---
title: 分配 appliesTo
description: 将 directoryObject 分配给功能推出。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efdc9e04e7e8554ef6acf5f3df7b2292b2c618e1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323553"
---
# <a name="assign-appliesto"></a><span data-ttu-id="b24bd-103">分配 appliesTo</span><span class="sxs-lookup"><span data-stu-id="b24bd-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b24bd-104">在[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象上添加 appliesTo, 以指定[featureRolloutPolicy](../resources/featurerolloutpolicy.md)应应用到的[directoryObject](../resources/directoryobject.md) 。</span><span class="sxs-lookup"><span data-stu-id="b24bd-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="b24bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="b24bd-105">Permissions</span></span>

<span data-ttu-id="b24bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b24bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b24bd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b24bd-108">Permission type</span></span>                        | <span data-ttu-id="b24bd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b24bd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b24bd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b24bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b24bd-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="b24bd-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="b24bd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b24bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b24bd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b24bd-113">Not supported.</span></span> |
| <span data-ttu-id="b24bd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b24bd-114">Application</span></span>                            | <span data-ttu-id="b24bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b24bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b24bd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b24bd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b24bd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b24bd-117">Request headers</span></span>

| <span data-ttu-id="b24bd-118">名称</span><span class="sxs-lookup"><span data-stu-id="b24bd-118">Name</span></span>          | <span data-ttu-id="b24bd-119">说明</span><span class="sxs-lookup"><span data-stu-id="b24bd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b24bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b24bd-120">Authorization</span></span> | <span data-ttu-id="b24bd-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b24bd-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b24bd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="b24bd-122">Request body</span></span>

<span data-ttu-id="b24bd-123">在请求正文中, 提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b24bd-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b24bd-124">响应</span><span class="sxs-lookup"><span data-stu-id="b24bd-124">Response</span></span>

<span data-ttu-id="b24bd-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[directoryObject](../resources/directoryobject.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b24bd-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b24bd-126">示例</span><span class="sxs-lookup"><span data-stu-id="b24bd-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b24bd-127">请求</span><span class="sxs-lookup"><span data-stu-id="b24bd-127">Request</span></span>

<span data-ttu-id="b24bd-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b24bd-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b24bd-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b24bd-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b24bd-130">C#</span><span class="sxs-lookup"><span data-stu-id="b24bd-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b24bd-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b24bd-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b24bd-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="b24bd-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b24bd-133">Java</span><span class="sxs-lookup"><span data-stu-id="b24bd-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b24bd-134">响应</span><span class="sxs-lookup"><span data-stu-id="b24bd-134">Response</span></span>

<span data-ttu-id="b24bd-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b24bd-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b24bd-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b24bd-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
