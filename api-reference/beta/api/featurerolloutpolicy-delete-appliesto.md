---
title: 删除 appliesTo
description: 从功能推出中删除 directoryObject。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1247cc352103bce040dc994feccd23ab9ba5a1bc
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062103"
---
# <a name="remove-appliesto"></a><span data-ttu-id="45b15-103">删除 appliesTo</span><span class="sxs-lookup"><span data-stu-id="45b15-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45b15-104">删除[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象上的 appliesTo, 以从功能展示中删除[directoryObject](../resources/directoryobject.md) 。</span><span class="sxs-lookup"><span data-stu-id="45b15-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="45b15-105">权限</span><span class="sxs-lookup"><span data-stu-id="45b15-105">Permissions</span></span>

<span data-ttu-id="45b15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45b15-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="45b15-108">Permission type</span></span>                        | <span data-ttu-id="45b15-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45b15-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="45b15-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45b15-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="45b15-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="45b15-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="45b15-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45b15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45b15-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="45b15-113">Not supported.</span></span> |
| <span data-ttu-id="45b15-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="45b15-114">Application</span></span>                            | <span data-ttu-id="45b15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="45b15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45b15-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45b15-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="45b15-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="45b15-117">Request headers</span></span>

| <span data-ttu-id="45b15-118">名称</span><span class="sxs-lookup"><span data-stu-id="45b15-118">Name</span></span>          | <span data-ttu-id="45b15-119">说明</span><span class="sxs-lookup"><span data-stu-id="45b15-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="45b15-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="45b15-120">Authorization</span></span> | <span data-ttu-id="45b15-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="45b15-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="45b15-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="45b15-122">Request body</span></span>

<span data-ttu-id="45b15-123">在请求正文中, 提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45b15-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45b15-124">响应</span><span class="sxs-lookup"><span data-stu-id="45b15-124">Response</span></span>

<span data-ttu-id="45b15-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="45b15-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45b15-127">示例</span><span class="sxs-lookup"><span data-stu-id="45b15-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45b15-128">请求</span><span class="sxs-lookup"><span data-stu-id="45b15-128">Request</span></span>

<span data-ttu-id="45b15-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45b15-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="45b15-130">响应</span><span class="sxs-lookup"><span data-stu-id="45b15-130">Response</span></span>

<span data-ttu-id="45b15-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45b15-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->