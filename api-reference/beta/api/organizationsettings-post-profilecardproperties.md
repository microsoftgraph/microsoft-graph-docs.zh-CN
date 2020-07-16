---
title: 创建 profileCardProperty
description: 使用此 API 创建新的 profileCardProperty。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e273490c6e189e291722885c48bb7c0e7fb2ea2a
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123930"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="15373-103">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="15373-103">Create profileCardProperty</span></span>

<span data-ttu-id="15373-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15373-105">为组织创建新的[profileCardProperty](../resources/profilecardproperty.md) 。</span><span class="sxs-lookup"><span data-stu-id="15373-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="15373-106">新属性由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="15373-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="15373-107">有关向组织的配置文件卡片添加属性的详细信息，请参阅[自定义配置文件卡片](/graph/add-properties-profilecard)。</span><span class="sxs-lookup"><span data-stu-id="15373-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="15373-108">权限</span><span class="sxs-lookup"><span data-stu-id="15373-108">Permissions</span></span>

<span data-ttu-id="15373-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15373-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15373-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="15373-111">Permission type</span></span>                        | <span data-ttu-id="15373-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15373-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15373-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15373-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="15373-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="15373-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="15373-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15373-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15373-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15373-116">Not supported.</span></span>                              |
| <span data-ttu-id="15373-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="15373-117">Application</span></span>                            | <span data-ttu-id="15373-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="15373-118">Not supported.</span></span>                              |

><span data-ttu-id="15373-119">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="15373-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="15373-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15373-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="15373-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="15373-121">Request headers</span></span>

| <span data-ttu-id="15373-122">名称</span><span class="sxs-lookup"><span data-stu-id="15373-122">Name</span></span>          |<span data-ttu-id="15373-123">说明</span><span class="sxs-lookup"><span data-stu-id="15373-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="15373-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15373-124">Authorization</span></span> | <span data-ttu-id="15373-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15373-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="15373-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15373-127">Content-Type</span></span>  | <span data-ttu-id="15373-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="15373-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15373-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="15373-130">Request body</span></span>

<span data-ttu-id="15373-131">在请求正文中，提供[profileCardProperty](../resources/profilecardproperty.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15373-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15373-132">响应</span><span class="sxs-lookup"><span data-stu-id="15373-132">Response</span></span>

<span data-ttu-id="15373-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="15373-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15373-134">示例</span><span class="sxs-lookup"><span data-stu-id="15373-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15373-135">请求</span><span class="sxs-lookup"><span data-stu-id="15373-135">Request</span></span>

<span data-ttu-id="15373-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15373-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15373-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="15373-137">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="15373-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15373-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15373-139">响应</span><span class="sxs-lookup"><span data-stu-id="15373-139">Response</span></span>

<span data-ttu-id="15373-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15373-140">The following is an example of the response.</span></span>

> <span data-ttu-id="15373-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="15373-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
