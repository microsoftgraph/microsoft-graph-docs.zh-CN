---
title: 获取配置文件
description: 检索 profile 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd6c68f79ffb417b12eb1f8e28d874f4461fb24e
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168552"
---
# <a name="get-profile"></a><span data-ttu-id="ebcf9-103">获取配置文件</span><span class="sxs-lookup"><span data-stu-id="ebcf9-103">Get profile</span></span>

<span data-ttu-id="ebcf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebcf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebcf9-105">检索给定用户的[配置文件](../resources/profile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="ebcf9-106">**配置文件**资源公开了将用户描述为[关系](../resources/profile.md#relationships)的各种丰富的属性，例如，周年纪念和教育活动。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="ebcf9-107">若要获取这些导航属性之一，请对该属性使用相应的 GET 方法。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="ebcf9-108">请参阅由**profile**公开的[方法](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebcf9-109">权限</span><span class="sxs-lookup"><span data-stu-id="ebcf9-109">Permissions</span></span>

<span data-ttu-id="ebcf9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebcf9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebcf9-112">Permission type</span></span>                        | <span data-ttu-id="ebcf9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebcf9-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ebcf9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcf9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebcf9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-115">Not supported.</span></span>                              |
| <span data-ttu-id="ebcf9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcf9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcf9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-117">Not supported.</span></span>                              |
| <span data-ttu-id="ebcf9-118">Application</span><span class="sxs-lookup"><span data-stu-id="ebcf9-118">Application</span></span>                            | <span data-ttu-id="ebcf9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="ebcf9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebcf9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebcf9-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ebcf9-121">Optional query parameters</span></span>

<span data-ttu-id="ebcf9-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ebcf9-123">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebcf9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebcf9-124">Request headers</span></span>

| <span data-ttu-id="ebcf9-125">名称</span><span class="sxs-lookup"><span data-stu-id="ebcf9-125">Name</span></span>           |<span data-ttu-id="ebcf9-126">说明</span><span class="sxs-lookup"><span data-stu-id="ebcf9-126">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ebcf9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebcf9-127">Authorization</span></span>  | <span data-ttu-id="ebcf9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ebcf9-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebcf9-130">Content-Type</span></span>   | <span data-ttu-id="ebcf9-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ebcf9-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebcf9-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebcf9-133">Request body</span></span>

<span data-ttu-id="ebcf9-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebcf9-135">响应</span><span class="sxs-lookup"><span data-stu-id="ebcf9-135">Response</span></span>

<span data-ttu-id="ebcf9-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[配置文件](../resources/profile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-136">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebcf9-137">示例</span><span class="sxs-lookup"><span data-stu-id="ebcf9-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebcf9-138">请求</span><span class="sxs-lookup"><span data-stu-id="ebcf9-138">Request</span></span>

<span data-ttu-id="ebcf9-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebcf9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcf9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="ebcf9-141">C#</span><span class="sxs-lookup"><span data-stu-id="ebcf9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebcf9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebcf9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebcf9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebcf9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebcf9-144">响应</span><span class="sxs-lookup"><span data-stu-id="ebcf9-144">Response</span></span>

<span data-ttu-id="ebcf9-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ebcf9-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ebcf9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
