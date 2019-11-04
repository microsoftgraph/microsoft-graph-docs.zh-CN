---
title: 获取配置文件
description: 检索 profile 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b6d551ff4920a7e7c132cac532dd1c7a59f54604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937817"
---
# <a name="get-profile"></a><span data-ttu-id="3d027-103">获取配置文件</span><span class="sxs-lookup"><span data-stu-id="3d027-103">Get profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d027-104">检索给定用户的[配置文件](../resources/profile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d027-104">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d027-105">权限</span><span class="sxs-lookup"><span data-stu-id="3d027-105">Permissions</span></span>

<span data-ttu-id="3d027-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d027-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d027-108">Permission type</span></span>                        | <span data-ttu-id="3d027-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d027-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d027-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d027-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d027-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d027-111">Not supported.</span></span>                              |
| <span data-ttu-id="3d027-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d027-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d027-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d027-113">Not supported.</span></span>                              |
| <span data-ttu-id="3d027-114">Application</span><span class="sxs-lookup"><span data-stu-id="3d027-114">Application</span></span>                            | <span data-ttu-id="3d027-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d027-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3d027-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d027-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d027-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d027-117">Optional query parameters</span></span>

<span data-ttu-id="3d027-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3d027-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3d027-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3d027-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d027-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d027-120">Request headers</span></span>

| <span data-ttu-id="3d027-121">名称</span><span class="sxs-lookup"><span data-stu-id="3d027-121">Name</span></span>           |<span data-ttu-id="3d027-122">说明</span><span class="sxs-lookup"><span data-stu-id="3d027-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3d027-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d027-123">Authorization</span></span>  | <span data-ttu-id="3d027-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d027-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3d027-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d027-126">Content-Type</span></span>   | <span data-ttu-id="3d027-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3d027-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d027-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d027-129">Request body</span></span>

<span data-ttu-id="3d027-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d027-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d027-131">响应</span><span class="sxs-lookup"><span data-stu-id="3d027-131">Response</span></span>

<span data-ttu-id="3d027-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[配置文件](../resources/profile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d027-132">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d027-133">示例</span><span class="sxs-lookup"><span data-stu-id="3d027-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d027-134">请求</span><span class="sxs-lookup"><span data-stu-id="3d027-134">Request</span></span>

<span data-ttu-id="3d027-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d027-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile
```

### <a name="response"></a><span data-ttu-id="3d027-136">响应</span><span class="sxs-lookup"><span data-stu-id="3d027-136">Response</span></span>

<span data-ttu-id="3d027-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3d027-137">The following is an example of the response.</span></span>

> <span data-ttu-id="3d027-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3d027-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->