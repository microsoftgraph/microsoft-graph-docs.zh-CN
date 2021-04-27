---
title: 列出 profileCardProperties
description: 检索 profilecardproperty 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7d0c064b6d422285d078a07edbc2ef24184a7d2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052052"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="ec660-103">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="ec660-103">List profileCardProperties</span></span>

<span data-ttu-id="ec660-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec660-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec660-105">获取组织的 [profileCardProperty](../resources/profilecardproperty.md) 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="ec660-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="ec660-106">每个资源都由它的 **directoryPropertyName** 属性标识。</span><span class="sxs-lookup"><span data-stu-id="ec660-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec660-107">权限</span><span class="sxs-lookup"><span data-stu-id="ec660-107">Permissions</span></span>

<span data-ttu-id="ec660-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec660-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec660-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec660-110">Permission type</span></span>                        | <span data-ttu-id="ec660-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec660-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec660-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec660-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec660-113">User.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec660-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="ec660-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec660-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec660-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec660-115">Not supported.</span></span>                              |
| <span data-ttu-id="ec660-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec660-116">Application</span></span>                            | <span data-ttu-id="ec660-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec660-117">Not supported.</span></span>                              |

><span data-ttu-id="ec660-118">**注意：** 对此操作使用委派权限要求登录用户具有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="ec660-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="ec660-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec660-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec660-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec660-120">Optional query parameters</span></span>

<span data-ttu-id="ec660-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec660-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec660-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ec660-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec660-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec660-123">Request headers</span></span>

| <span data-ttu-id="ec660-124">名称</span><span class="sxs-lookup"><span data-stu-id="ec660-124">Name</span></span>          |<span data-ttu-id="ec660-125">说明</span><span class="sxs-lookup"><span data-stu-id="ec660-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="ec660-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec660-126">Authorization</span></span> | <span data-ttu-id="ec660-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec660-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ec660-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec660-129">Content-Type</span></span>  | <span data-ttu-id="ec660-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ec660-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec660-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec660-132">Request body</span></span>

<span data-ttu-id="ec660-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec660-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec660-134">响应</span><span class="sxs-lookup"><span data-stu-id="ec660-134">Response</span></span>

<span data-ttu-id="ec660-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [profileCardProperty](../resources/profilecardproperty.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec660-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec660-136">示例</span><span class="sxs-lookup"><span data-stu-id="ec660-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec660-137">请求</span><span class="sxs-lookup"><span data-stu-id="ec660-137">Request</span></span>

<span data-ttu-id="ec660-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ec660-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec660-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec660-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```
# <a name="c"></a>[<span data-ttu-id="ec660-140">C#</span><span class="sxs-lookup"><span data-stu-id="ec660-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec660-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec660-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec660-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec660-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec660-143">Java</span><span class="sxs-lookup"><span data-stu-id="ec660-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec660-144">响应</span><span class="sxs-lookup"><span data-stu-id="ec660-144">Response</span></span>

<span data-ttu-id="ec660-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ec660-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ec660-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ec660-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List profileCardProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


