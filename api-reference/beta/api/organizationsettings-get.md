---
title: 获取 organizationSettings
description: 检索 organizationSettings 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53bf7e03d56ad949683b0c363af3d4aa017502d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052066"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="550ee-103">获取 organizationSettings</span><span class="sxs-lookup"><span data-stu-id="550ee-103">Get organizationSettings</span></span>

<span data-ttu-id="550ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="550ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="550ee-105">检索 [organizationSettings](../resources/organizationsettings.md) 对象的属性和关系，包括 **profileCardProperties**。</span><span class="sxs-lookup"><span data-stu-id="550ee-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object, including **profileCardProperties**.</span></span>

<span data-ttu-id="550ee-106">此操作不会通过 [itemInsights](../resources/iteminsightssettings.md)导航属性返回 **itemInsightsSettings。**</span><span class="sxs-lookup"><span data-stu-id="550ee-106">This operation does not return [itemInsightsSettings](../resources/iteminsightssettings.md) through the **itemInsights** navigation property.</span></span> <span data-ttu-id="550ee-107">请[改为使用 get itemInsightsSettings。](iteminsightssettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="550ee-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="550ee-108">权限</span><span class="sxs-lookup"><span data-stu-id="550ee-108">Permissions</span></span>

<span data-ttu-id="550ee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="550ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="550ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="550ee-111">Permission type</span></span>                        | <span data-ttu-id="550ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="550ee-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="550ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="550ee-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="550ee-114">User.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="550ee-114">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="550ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="550ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="550ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="550ee-116">Not supported.</span></span>                              |
| <span data-ttu-id="550ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="550ee-117">Application</span></span>                            | <span data-ttu-id="550ee-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="550ee-118">Not supported.</span></span>                              |

><span data-ttu-id="550ee-119">**注意：** 对此操作使用委派权限要求登录用户具有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="550ee-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="550ee-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="550ee-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="550ee-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="550ee-121">Optional query parameters</span></span>

<span data-ttu-id="550ee-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="550ee-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="550ee-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="550ee-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="550ee-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="550ee-124">Request headers</span></span>

| <span data-ttu-id="550ee-125">名称</span><span class="sxs-lookup"><span data-stu-id="550ee-125">Name</span></span>          |<span data-ttu-id="550ee-126">说明</span><span class="sxs-lookup"><span data-stu-id="550ee-126">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="550ee-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="550ee-127">Authorization</span></span> | <span data-ttu-id="550ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="550ee-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="550ee-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="550ee-130">Content-Type</span></span>  | <span data-ttu-id="550ee-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="550ee-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="550ee-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="550ee-133">Request body</span></span>

<span data-ttu-id="550ee-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="550ee-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="550ee-135">响应</span><span class="sxs-lookup"><span data-stu-id="550ee-135">Response</span></span>

<span data-ttu-id="550ee-136">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [organizationSettings](../resources/organizationsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="550ee-136">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="550ee-137">示例</span><span class="sxs-lookup"><span data-stu-id="550ee-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="550ee-138">请求</span><span class="sxs-lookup"><span data-stu-id="550ee-138">Request</span></span>

<span data-ttu-id="550ee-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="550ee-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="550ee-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="550ee-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="550ee-141">C#</span><span class="sxs-lookup"><span data-stu-id="550ee-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="550ee-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="550ee-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="550ee-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="550ee-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="550ee-144">Java</span><span class="sxs-lookup"><span data-stu-id="550ee-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="550ee-145">响应</span><span class="sxs-lookup"><span data-stu-id="550ee-145">Response</span></span>

<span data-ttu-id="550ee-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="550ee-146">The following is an example of the response.</span></span>

> <span data-ttu-id="550ee-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="550ee-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


