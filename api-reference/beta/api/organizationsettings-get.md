---
title: 获取 organizationSettings
description: 检索 organizationSettings 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 240704fd29f3950060342f4d2b8ab2efcc6f2ee0
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051039"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="dea0d-103">获取 organizationSettings</span><span class="sxs-lookup"><span data-stu-id="dea0d-103">Get organizationSettings</span></span>

<span data-ttu-id="dea0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dea0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea0d-105">检索[organizationSettings](../resources/organizationsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dea0d-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dea0d-106">权限</span><span class="sxs-lookup"><span data-stu-id="dea0d-106">Permissions</span></span>

<span data-ttu-id="dea0d-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dea0d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dea0d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dea0d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dea0d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dea0d-109">Permission type</span></span>                        | <span data-ttu-id="dea0d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dea0d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dea0d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dea0d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dea0d-112">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="dea0d-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="dea0d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dea0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dea0d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dea0d-114">Not supported.</span></span>                              |
| <span data-ttu-id="dea0d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dea0d-115">Application</span></span>                            | <span data-ttu-id="dea0d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dea0d-116">Not supported.</span></span>                              |

><span data-ttu-id="dea0d-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="dea0d-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="dea0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dea0d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dea0d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dea0d-119">Optional query parameters</span></span>

<span data-ttu-id="dea0d-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dea0d-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dea0d-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="dea0d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea0d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dea0d-122">Request headers</span></span>

| <span data-ttu-id="dea0d-123">名称</span><span class="sxs-lookup"><span data-stu-id="dea0d-123">Name</span></span>          |<span data-ttu-id="dea0d-124">说明</span><span class="sxs-lookup"><span data-stu-id="dea0d-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="dea0d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dea0d-125">Authorization</span></span> | <span data-ttu-id="dea0d-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="dea0d-126">Bearer {token}.</span></span> <span data-ttu-id="dea0d-127">Required.</span><span class="sxs-lookup"><span data-stu-id="dea0d-127">Required.</span></span>   |
| <span data-ttu-id="dea0d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dea0d-128">Content-Type</span></span>  | <span data-ttu-id="dea0d-129">application/json.</span><span class="sxs-lookup"><span data-stu-id="dea0d-129">application/json.</span></span> <span data-ttu-id="dea0d-130">Required.</span><span class="sxs-lookup"><span data-stu-id="dea0d-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dea0d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="dea0d-131">Request body</span></span>

<span data-ttu-id="dea0d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dea0d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea0d-133">响应</span><span class="sxs-lookup"><span data-stu-id="dea0d-133">Response</span></span>

<span data-ttu-id="dea0d-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[organizationSettings](../resources/organizationsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dea0d-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dea0d-135">示例</span><span class="sxs-lookup"><span data-stu-id="dea0d-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dea0d-136">请求</span><span class="sxs-lookup"><span data-stu-id="dea0d-136">Request</span></span>

<span data-ttu-id="dea0d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dea0d-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

### <a name="response"></a><span data-ttu-id="dea0d-138">响应</span><span class="sxs-lookup"><span data-stu-id="dea0d-138">Response</span></span>

<span data-ttu-id="dea0d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dea0d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dea0d-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="dea0d-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dea0d-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dea0d-141">All the properties will be returned from an actual call.</span></span>

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
