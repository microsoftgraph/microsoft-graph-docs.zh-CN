---
title: 列出 profileCardProperties
description: 检索 profilecardproperty 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 732671a5c968b13796113affa403d7c44a9691f9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080745"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="76796-103">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="76796-103">List profileCardProperties</span></span>

<span data-ttu-id="76796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76796-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76796-105">获取组织的[profileCardProperty](../resources/profilecardproperty.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="76796-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="76796-106">每个资源都由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="76796-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="76796-107">权限</span><span class="sxs-lookup"><span data-stu-id="76796-107">Permissions</span></span>

<span data-ttu-id="76796-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="76796-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="76796-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76796-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76796-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76796-110">Permission type</span></span>                        | <span data-ttu-id="76796-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76796-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76796-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76796-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76796-113">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="76796-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="76796-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76796-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76796-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76796-115">Not supported.</span></span>                              |
| <span data-ttu-id="76796-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="76796-116">Application</span></span>                            | <span data-ttu-id="76796-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="76796-117">Not supported.</span></span>                              |

><span data-ttu-id="76796-118">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="76796-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="76796-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76796-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76796-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76796-120">Optional query parameters</span></span>

<span data-ttu-id="76796-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76796-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="76796-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="76796-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="76796-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="76796-123">Request headers</span></span>

| <span data-ttu-id="76796-124">名称</span><span class="sxs-lookup"><span data-stu-id="76796-124">Name</span></span>          |<span data-ttu-id="76796-125">说明</span><span class="sxs-lookup"><span data-stu-id="76796-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="76796-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="76796-126">Authorization</span></span> | <span data-ttu-id="76796-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="76796-127">Bearer {token}.</span></span> <span data-ttu-id="76796-128">Required.</span><span class="sxs-lookup"><span data-stu-id="76796-128">Required.</span></span>   |
| <span data-ttu-id="76796-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76796-129">Content-Type</span></span>  | <span data-ttu-id="76796-130">application/json.</span><span class="sxs-lookup"><span data-stu-id="76796-130">application/json.</span></span> <span data-ttu-id="76796-131">Required.</span><span class="sxs-lookup"><span data-stu-id="76796-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76796-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="76796-132">Request body</span></span>

<span data-ttu-id="76796-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76796-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76796-134">响应</span><span class="sxs-lookup"><span data-stu-id="76796-134">Response</span></span>

<span data-ttu-id="76796-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[profileCardProperty](../resources/profilecardproperty.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="76796-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76796-136">示例</span><span class="sxs-lookup"><span data-stu-id="76796-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76796-137">请求</span><span class="sxs-lookup"><span data-stu-id="76796-137">Request</span></span>

<span data-ttu-id="76796-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76796-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76796-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="76796-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```
# <a name="c"></a>[<span data-ttu-id="76796-140">C#</span><span class="sxs-lookup"><span data-stu-id="76796-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76796-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76796-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76796-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76796-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76796-143">响应</span><span class="sxs-lookup"><span data-stu-id="76796-143">Response</span></span>

<span data-ttu-id="76796-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76796-144">The following is an example of the response.</span></span>

> <span data-ttu-id="76796-145">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="76796-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76796-146">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="76796-146">All the properties will be returned from an actual call.</span></span>

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
