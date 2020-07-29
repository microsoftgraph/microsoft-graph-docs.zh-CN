---
title: 创建 ediscoveryCase
description: 使用此 API 创建新的 ediscoveryCase。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0bc59ac1fd61695952aeb64a2cfe081597901dff
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509987"
---
# <a name="create-ediscoverycase"></a><span data-ttu-id="08199-103">创建 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="08199-103">Create ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08199-104">创建新的[ediscoveryCase](../resources/ediscoverycase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08199-104">Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08199-105">权限</span><span class="sxs-lookup"><span data-stu-id="08199-105">Permissions</span></span>

<span data-ttu-id="08199-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08199-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="08199-108">Permission type</span></span>                        | <span data-ttu-id="08199-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08199-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08199-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08199-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="08199-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="08199-111">User.Read</span></span>      |
| <span data-ttu-id="08199-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08199-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08199-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="08199-113">Not supported.</span></span> |
| <span data-ttu-id="08199-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="08199-114">Application</span></span>                            | <span data-ttu-id="08199-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08199-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08199-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08199-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="08199-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="08199-117">Request headers</span></span>

| <span data-ttu-id="08199-118">名称</span><span class="sxs-lookup"><span data-stu-id="08199-118">Name</span></span>          | <span data-ttu-id="08199-119">说明</span><span class="sxs-lookup"><span data-stu-id="08199-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="08199-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="08199-120">Authorization</span></span> | <span data-ttu-id="08199-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08199-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08199-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="08199-123">Request body</span></span>

<span data-ttu-id="08199-124">在请求正文中，提供[ediscoveryCase](../resources/ediscoverycase.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08199-124">In the request body, supply a JSON representation of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span> <span data-ttu-id="08199-125">下表列出了可以通过调用提交的属性。</span><span class="sxs-lookup"><span data-stu-id="08199-125">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="08199-126">属性</span><span class="sxs-lookup"><span data-stu-id="08199-126">Property</span></span>     | <span data-ttu-id="08199-127">类型</span><span class="sxs-lookup"><span data-stu-id="08199-127">Type</span></span>        | <span data-ttu-id="08199-128">说明</span><span class="sxs-lookup"><span data-stu-id="08199-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="08199-129">displayName</span><span class="sxs-lookup"><span data-stu-id="08199-129">displayName</span></span>  | <span data-ttu-id="08199-130">string</span><span class="sxs-lookup"><span data-stu-id="08199-130">string</span></span>      | <span data-ttu-id="08199-131">电子数据展示事例的名称。</span><span class="sxs-lookup"><span data-stu-id="08199-131">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="08199-132">响应</span><span class="sxs-lookup"><span data-stu-id="08199-132">Response</span></span>

<span data-ttu-id="08199-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[ediscoveryCase](../resources/ediscoverycase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08199-133">If successful, this method returns a `201 Created` response code and a new [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08199-134">示例</span><span class="sxs-lookup"><span data-stu-id="08199-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08199-135">请求</span><span class="sxs-lookup"><span data-stu-id="08199-135">Request</span></span>

<span data-ttu-id="08199-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08199-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_ediscoverycase"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```

### <a name="response"></a><span data-ttu-id="08199-137">响应</span><span class="sxs-lookup"><span data-stu-id="08199-137">Response</span></span>

<span data-ttu-id="08199-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08199-138">The following is an example of the response.</span></span>

> <span data-ttu-id="08199-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08199-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases/$entity",
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
