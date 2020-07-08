---
title: 创建 profileCardProperty
description: 使用此 API 创建新的 profileCardProperty。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 24fe1a2f4257475849ecb3c057843d7cd0661a21
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080632"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="931f9-103">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="931f9-103">Create profileCardProperty</span></span>

<span data-ttu-id="931f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="931f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="931f9-105">为组织创建新的[profileCardProperty](../resources/profilecardproperty.md) 。</span><span class="sxs-lookup"><span data-stu-id="931f9-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="931f9-106">新属性由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="931f9-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="931f9-107">有关向组织的配置文件卡片添加属性的详细信息，请参阅[自定义配置文件卡片](/graph/add-properties-profilecard)。</span><span class="sxs-lookup"><span data-stu-id="931f9-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="931f9-108">权限</span><span class="sxs-lookup"><span data-stu-id="931f9-108">Permissions</span></span>

<span data-ttu-id="931f9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="931f9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="931f9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="931f9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="931f9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="931f9-111">Permission type</span></span>                        | <span data-ttu-id="931f9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="931f9-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="931f9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="931f9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="931f9-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="931f9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="931f9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="931f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="931f9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="931f9-116">Not supported.</span></span>                              |
| <span data-ttu-id="931f9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="931f9-117">Application</span></span>                            | <span data-ttu-id="931f9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="931f9-118">Not supported.</span></span>                              |

><span data-ttu-id="931f9-119">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="931f9-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="931f9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="931f9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="931f9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="931f9-121">Request headers</span></span>

| <span data-ttu-id="931f9-122">名称</span><span class="sxs-lookup"><span data-stu-id="931f9-122">Name</span></span>          |<span data-ttu-id="931f9-123">说明</span><span class="sxs-lookup"><span data-stu-id="931f9-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="931f9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="931f9-124">Authorization</span></span> | <span data-ttu-id="931f9-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="931f9-125">Bearer {token}.</span></span> <span data-ttu-id="931f9-126">Required.</span><span class="sxs-lookup"><span data-stu-id="931f9-126">Required.</span></span>   |
| <span data-ttu-id="931f9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="931f9-127">Content-Type</span></span>  | <span data-ttu-id="931f9-128">application/json.</span><span class="sxs-lookup"><span data-stu-id="931f9-128">application/json.</span></span> <span data-ttu-id="931f9-129">Required.</span><span class="sxs-lookup"><span data-stu-id="931f9-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="931f9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="931f9-130">Request body</span></span>

<span data-ttu-id="931f9-131">在请求正文中，提供[profileCardProperty](../resources/profilecardproperty.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="931f9-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="931f9-132">响应</span><span class="sxs-lookup"><span data-stu-id="931f9-132">Response</span></span>

<span data-ttu-id="931f9-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="931f9-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="931f9-134">示例</span><span class="sxs-lookup"><span data-stu-id="931f9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="931f9-135">请求</span><span class="sxs-lookup"><span data-stu-id="931f9-135">Request</span></span>

<span data-ttu-id="931f9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="931f9-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="931f9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="931f9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
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
# <a name="javascript"></a>[<span data-ttu-id="931f9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="931f9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="931f9-139">响应</span><span class="sxs-lookup"><span data-stu-id="931f9-139">Response</span></span>

<span data-ttu-id="931f9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="931f9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="931f9-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="931f9-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="931f9-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="931f9-142">All the properties will be returned from an actual call.</span></span>

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
