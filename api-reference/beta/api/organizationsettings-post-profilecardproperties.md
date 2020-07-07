---
title: 创建 profileCardProperty
description: 使用此 API 创建新的 profileCardProperty。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1bbdb77ea7d9cd9d76f63198b449b4f03181bc62
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051037"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="548b8-103">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="548b8-103">Create profileCardProperty</span></span>

<span data-ttu-id="548b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="548b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="548b8-105">为组织创建新的[profileCardProperty](../resources/profilecardproperty.md) 。</span><span class="sxs-lookup"><span data-stu-id="548b8-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="548b8-106">新属性由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="548b8-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="548b8-107">有关向组织的配置文件卡片添加属性的详细信息，请参阅自定义配置文件卡片。</span><span class="sxs-lookup"><span data-stu-id="548b8-107">For more information on adding properties to the profile card for an organization, see customize the profile card.</span></span>

## <a name="permissions"></a><span data-ttu-id="548b8-108">权限</span><span class="sxs-lookup"><span data-stu-id="548b8-108">Permissions</span></span>

<span data-ttu-id="548b8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="548b8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="548b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="548b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="548b8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="548b8-111">Permission type</span></span>                        | <span data-ttu-id="548b8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="548b8-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="548b8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="548b8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="548b8-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="548b8-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="548b8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="548b8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="548b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="548b8-116">Not supported.</span></span>                              |
| <span data-ttu-id="548b8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="548b8-117">Application</span></span>                            | <span data-ttu-id="548b8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="548b8-118">Not supported.</span></span>                              |

><span data-ttu-id="548b8-119">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="548b8-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="548b8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="548b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="548b8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="548b8-121">Request headers</span></span>

| <span data-ttu-id="548b8-122">名称</span><span class="sxs-lookup"><span data-stu-id="548b8-122">Name</span></span>          |<span data-ttu-id="548b8-123">说明</span><span class="sxs-lookup"><span data-stu-id="548b8-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="548b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="548b8-124">Authorization</span></span> | <span data-ttu-id="548b8-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="548b8-125">Bearer {token}.</span></span> <span data-ttu-id="548b8-126">Required.</span><span class="sxs-lookup"><span data-stu-id="548b8-126">Required.</span></span>   |
| <span data-ttu-id="548b8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="548b8-127">Content-Type</span></span>  | <span data-ttu-id="548b8-128">application/json.</span><span class="sxs-lookup"><span data-stu-id="548b8-128">application/json.</span></span> <span data-ttu-id="548b8-129">Required.</span><span class="sxs-lookup"><span data-stu-id="548b8-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="548b8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="548b8-130">Request body</span></span>

<span data-ttu-id="548b8-131">在请求正文中，提供[profileCardProperty](../resources/profilecardproperty.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="548b8-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="548b8-132">响应</span><span class="sxs-lookup"><span data-stu-id="548b8-132">Response</span></span>

<span data-ttu-id="548b8-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="548b8-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="548b8-134">示例</span><span class="sxs-lookup"><span data-stu-id="548b8-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="548b8-135">请求</span><span class="sxs-lookup"><span data-stu-id="548b8-135">Request</span></span>

<span data-ttu-id="548b8-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="548b8-136">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="548b8-137">响应</span><span class="sxs-lookup"><span data-stu-id="548b8-137">Response</span></span>

<span data-ttu-id="548b8-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="548b8-138">The following is an example of the response.</span></span>

> <span data-ttu-id="548b8-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="548b8-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="548b8-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="548b8-140">All the properties will be returned from an actual call.</span></span>

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
