---
title: 获取 organizationSettings
description: 检索 organizationSettings 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1de3e239f64b81a6e8f2995bfa626a0d7734ef9e
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080686"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="bc6fd-103">获取 organizationSettings</span><span class="sxs-lookup"><span data-stu-id="bc6fd-103">Get organizationSettings</span></span>

<span data-ttu-id="bc6fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc6fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc6fd-105">检索[organizationSettings](../resources/organizationsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc6fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="bc6fd-106">Permissions</span></span>

<span data-ttu-id="bc6fd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bc6fd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc6fd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc6fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc6fd-109">Permission type</span></span>                        | <span data-ttu-id="bc6fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc6fd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bc6fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc6fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc6fd-112">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="bc6fd-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="bc6fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc6fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc6fd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-114">Not supported.</span></span>                              |
| <span data-ttu-id="bc6fd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc6fd-115">Application</span></span>                            | <span data-ttu-id="bc6fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-116">Not supported.</span></span>                              |

><span data-ttu-id="bc6fd-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="bc6fd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc6fd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc6fd-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc6fd-119">Optional query parameters</span></span>

<span data-ttu-id="bc6fd-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bc6fd-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc6fd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc6fd-122">Request headers</span></span>

| <span data-ttu-id="bc6fd-123">名称</span><span class="sxs-lookup"><span data-stu-id="bc6fd-123">Name</span></span>          |<span data-ttu-id="bc6fd-124">说明</span><span class="sxs-lookup"><span data-stu-id="bc6fd-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="bc6fd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc6fd-125">Authorization</span></span> | <span data-ttu-id="bc6fd-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-126">Bearer {token}.</span></span> <span data-ttu-id="bc6fd-127">Required.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-127">Required.</span></span>   |
| <span data-ttu-id="bc6fd-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc6fd-128">Content-Type</span></span>  | <span data-ttu-id="bc6fd-129">application/json.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-129">application/json.</span></span> <span data-ttu-id="bc6fd-130">Required.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc6fd-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc6fd-131">Request body</span></span>

<span data-ttu-id="bc6fd-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc6fd-133">响应</span><span class="sxs-lookup"><span data-stu-id="bc6fd-133">Response</span></span>

<span data-ttu-id="bc6fd-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[organizationSettings](../resources/organizationsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc6fd-135">示例</span><span class="sxs-lookup"><span data-stu-id="bc6fd-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc6fd-136">请求</span><span class="sxs-lookup"><span data-stu-id="bc6fd-136">Request</span></span>

<span data-ttu-id="bc6fd-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc6fd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc6fd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="bc6fd-139">C#</span><span class="sxs-lookup"><span data-stu-id="bc6fd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc6fd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc6fd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc6fd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc6fd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc6fd-142">响应</span><span class="sxs-lookup"><span data-stu-id="bc6fd-142">Response</span></span>

<span data-ttu-id="bc6fd-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc6fd-143">The following is an example of the response.</span></span>

> <span data-ttu-id="bc6fd-144">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc6fd-145">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bc6fd-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "345233-676277-644334-445677-334556",
  "profileCardProperties": [
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
  "description": "Get organizationSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
