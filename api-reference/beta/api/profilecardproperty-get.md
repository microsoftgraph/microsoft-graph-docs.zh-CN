---
title: 获取 profileCardProperty
description: 检索 profileCardProperty 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1047159a1e2f0a481796004d461b00a29aa88482
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123839"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="4a87d-103">获取 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="4a87d-103">Get profileCardProperty</span></span>

<span data-ttu-id="4a87d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a87d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a87d-105">检索[profileCardProperty](../resources/profilecardproperty.md)实体的属性和关系，其中包含在给定字段的 Microsoft 365 组织中存在的配置文件卡片自定义项。</span><span class="sxs-lookup"><span data-stu-id="4a87d-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="4a87d-106">ProfileCardProperty 由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="4a87d-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a87d-107">权限</span><span class="sxs-lookup"><span data-stu-id="4a87d-107">Permissions</span></span>

<span data-ttu-id="4a87d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a87d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a87d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a87d-110">Permission type</span></span>                        | <span data-ttu-id="4a87d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a87d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a87d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a87d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a87d-113">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="4a87d-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="4a87d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a87d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a87d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a87d-115">Not supported.</span></span>                              |
| <span data-ttu-id="4a87d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a87d-116">Application</span></span>                            | <span data-ttu-id="4a87d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a87d-117">Not supported.</span></span>                              |

><span data-ttu-id="4a87d-118">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="4a87d-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a87d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a87d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a87d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a87d-120">Optional query parameters</span></span>

<span data-ttu-id="4a87d-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a87d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4a87d-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4a87d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a87d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a87d-123">Request headers</span></span>

| <span data-ttu-id="4a87d-124">名称</span><span class="sxs-lookup"><span data-stu-id="4a87d-124">Name</span></span>      |<span data-ttu-id="4a87d-125">说明</span><span class="sxs-lookup"><span data-stu-id="4a87d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a87d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a87d-126">Authorization</span></span> | <span data-ttu-id="4a87d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a87d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a87d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a87d-129">Request body</span></span>

<span data-ttu-id="4a87d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a87d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a87d-131">响应</span><span class="sxs-lookup"><span data-stu-id="4a87d-131">Response</span></span>

<span data-ttu-id="4a87d-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a87d-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a87d-133">示例</span><span class="sxs-lookup"><span data-stu-id="4a87d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a87d-134">请求</span><span class="sxs-lookup"><span data-stu-id="4a87d-134">Request</span></span>

<span data-ttu-id="4a87d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4a87d-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a87d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a87d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="4a87d-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a87d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a87d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a87d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a87d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a87d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a87d-140">响应</span><span class="sxs-lookup"><span data-stu-id="4a87d-140">Response</span></span>

<span data-ttu-id="4a87d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a87d-141">The following is an example of the response.</span></span>

> <span data-ttu-id="4a87d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a87d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
