---
title: 列出 profileCardProperties
description: 检索 profilecardproperty 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4aa23e69308d8c13cc9ceb25bcc1398c9cbb1012
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051038"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="34e68-103">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="34e68-103">List profileCardProperties</span></span>

<span data-ttu-id="34e68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34e68-105">获取组织的[profileCardProperty](../resources/profilecardproperty.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="34e68-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="34e68-106">每个资源都由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="34e68-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="34e68-107">权限</span><span class="sxs-lookup"><span data-stu-id="34e68-107">Permissions</span></span>

<span data-ttu-id="34e68-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="34e68-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="34e68-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e68-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34e68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34e68-110">Permission type</span></span>                        | <span data-ttu-id="34e68-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34e68-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34e68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34e68-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="34e68-113">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="34e68-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="34e68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34e68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34e68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34e68-115">Not supported.</span></span>                              |
| <span data-ttu-id="34e68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34e68-116">Application</span></span>                            | <span data-ttu-id="34e68-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="34e68-117">Not supported.</span></span>                              |

><span data-ttu-id="34e68-118">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="34e68-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="34e68-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34e68-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34e68-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="34e68-120">Optional query parameters</span></span>

<span data-ttu-id="34e68-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="34e68-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="34e68-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="34e68-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e68-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="34e68-123">Request headers</span></span>

| <span data-ttu-id="34e68-124">名称</span><span class="sxs-lookup"><span data-stu-id="34e68-124">Name</span></span>          |<span data-ttu-id="34e68-125">说明</span><span class="sxs-lookup"><span data-stu-id="34e68-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="34e68-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="34e68-126">Authorization</span></span> | <span data-ttu-id="34e68-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="34e68-127">Bearer {token}.</span></span> <span data-ttu-id="34e68-128">Required.</span><span class="sxs-lookup"><span data-stu-id="34e68-128">Required.</span></span>   |
| <span data-ttu-id="34e68-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34e68-129">Content-Type</span></span>  | <span data-ttu-id="34e68-130">application/json.</span><span class="sxs-lookup"><span data-stu-id="34e68-130">application/json.</span></span> <span data-ttu-id="34e68-131">Required.</span><span class="sxs-lookup"><span data-stu-id="34e68-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34e68-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="34e68-132">Request body</span></span>

<span data-ttu-id="34e68-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34e68-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34e68-134">响应</span><span class="sxs-lookup"><span data-stu-id="34e68-134">Response</span></span>

<span data-ttu-id="34e68-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[profileCardProperty](../resources/profilecardproperty.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="34e68-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34e68-136">示例</span><span class="sxs-lookup"><span data-stu-id="34e68-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34e68-137">请求</span><span class="sxs-lookup"><span data-stu-id="34e68-137">Request</span></span>

<span data-ttu-id="34e68-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="34e68-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

### <a name="response"></a><span data-ttu-id="34e68-139">响应</span><span class="sxs-lookup"><span data-stu-id="34e68-139">Response</span></span>

<span data-ttu-id="34e68-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="34e68-140">The following is an example of the response.</span></span>

> <span data-ttu-id="34e68-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="34e68-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="34e68-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="34e68-142">All the properties will be returned from an actual call.</span></span>

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
