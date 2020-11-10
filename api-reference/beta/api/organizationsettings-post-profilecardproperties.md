---
title: 创建 profileCardProperty
description: 使用此 API 创建新的 profileCardProperty。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 597ff7f2bafcf05e4f2827932bc29cbc98df10c1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964011"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="676c6-103">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="676c6-103">Create profileCardProperty</span></span>

<span data-ttu-id="676c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="676c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="676c6-105">为组织创建新的 [profileCardProperty](../resources/profilecardproperty.md) 。</span><span class="sxs-lookup"><span data-stu-id="676c6-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="676c6-106">新属性由其 **directoryPropertyName** 属性标识。</span><span class="sxs-lookup"><span data-stu-id="676c6-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="676c6-107">有关向组织的配置文件卡片添加属性的详细信息，请参阅 [自定义配置文件卡片](/graph/add-properties-profilecard)。</span><span class="sxs-lookup"><span data-stu-id="676c6-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="676c6-108">权限</span><span class="sxs-lookup"><span data-stu-id="676c6-108">Permissions</span></span>

<span data-ttu-id="676c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="676c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="676c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="676c6-111">Permission type</span></span>                        | <span data-ttu-id="676c6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="676c6-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="676c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="676c6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="676c6-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="676c6-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="676c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="676c6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="676c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="676c6-116">Not supported.</span></span>                              |
| <span data-ttu-id="676c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="676c6-117">Application</span></span>                            | <span data-ttu-id="676c6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="676c6-118">Not supported.</span></span>                              |

><span data-ttu-id="676c6-119">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="676c6-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="676c6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="676c6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="676c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="676c6-121">Request headers</span></span>

| <span data-ttu-id="676c6-122">名称</span><span class="sxs-lookup"><span data-stu-id="676c6-122">Name</span></span>          |<span data-ttu-id="676c6-123">说明</span><span class="sxs-lookup"><span data-stu-id="676c6-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="676c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="676c6-124">Authorization</span></span> | <span data-ttu-id="676c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="676c6-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="676c6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="676c6-127">Content-Type</span></span>  | <span data-ttu-id="676c6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="676c6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="676c6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="676c6-130">Request body</span></span>

<span data-ttu-id="676c6-131">在请求正文中，提供 [profileCardProperty](../resources/profilecardproperty.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="676c6-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="676c6-132">响应</span><span class="sxs-lookup"><span data-stu-id="676c6-132">Response</span></span>

<span data-ttu-id="676c6-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [profileCardProperty](../resources/profilecardproperty.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="676c6-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="676c6-134">示例</span><span class="sxs-lookup"><span data-stu-id="676c6-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="676c6-135">请求</span><span class="sxs-lookup"><span data-stu-id="676c6-135">Request</span></span>

<span data-ttu-id="676c6-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="676c6-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="676c6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="676c6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
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
# <a name="javascript"></a>[<span data-ttu-id="676c6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="676c6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="676c6-139">C#</span><span class="sxs-lookup"><span data-stu-id="676c6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-profilecardproperty-from-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="676c6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="676c6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-profilecardproperty-from-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="676c6-141">Java</span><span class="sxs-lookup"><span data-stu-id="676c6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-profilecardproperty-from-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="676c6-142">响应</span><span class="sxs-lookup"><span data-stu-id="676c6-142">Response</span></span>

<span data-ttu-id="676c6-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="676c6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="676c6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="676c6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


