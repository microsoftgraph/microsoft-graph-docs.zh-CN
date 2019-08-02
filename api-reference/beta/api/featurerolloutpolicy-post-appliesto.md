---
title: 分配 appliesTo
description: 将 directoryObject 分配给功能推出。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b5a01131adb20feccbccd55c2ce4f7e01ea1e214
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062106"
---
# <a name="assign-appliesto"></a><span data-ttu-id="bd85f-103">分配 appliesTo</span><span class="sxs-lookup"><span data-stu-id="bd85f-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd85f-104">在[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象上添加 appliesTo, 以指定[featureRolloutPolicy](../resources/featurerolloutpolicy.md)应应用到的[directoryObject](../resources/directoryobject.md) 。</span><span class="sxs-lookup"><span data-stu-id="bd85f-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd85f-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd85f-105">Permissions</span></span>

<span data-ttu-id="bd85f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd85f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd85f-108">Permission type</span></span>                        | <span data-ttu-id="bd85f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd85f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd85f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd85f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd85f-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="bd85f-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="bd85f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd85f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd85f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd85f-113">Not supported.</span></span> |
| <span data-ttu-id="bd85f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd85f-114">Application</span></span>                            | <span data-ttu-id="bd85f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd85f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd85f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd85f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bd85f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd85f-117">Request headers</span></span>

| <span data-ttu-id="bd85f-118">名称</span><span class="sxs-lookup"><span data-stu-id="bd85f-118">Name</span></span>          | <span data-ttu-id="bd85f-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd85f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd85f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd85f-120">Authorization</span></span> | <span data-ttu-id="bd85f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bd85f-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd85f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd85f-122">Request body</span></span>

<span data-ttu-id="bd85f-123">在请求正文中, 提供[directoryObject](../resources/directoryobject.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd85f-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bd85f-124">响应</span><span class="sxs-lookup"><span data-stu-id="bd85f-124">Response</span></span>

<span data-ttu-id="bd85f-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[directoryObject](../resources/directoryobject.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd85f-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd85f-126">示例</span><span class="sxs-lookup"><span data-stu-id="bd85f-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd85f-127">请求</span><span class="sxs-lookup"><span data-stu-id="bd85f-127">Request</span></span>

<span data-ttu-id="bd85f-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd85f-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd85f-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd85f-129">Response</span></span>

<span data-ttu-id="bd85f-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd85f-130">The following is an example of the response.</span></span>

> <span data-ttu-id="bd85f-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd85f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
