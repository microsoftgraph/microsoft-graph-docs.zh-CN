---
title: 获取 profileCardProperty
description: 检索 profileCardProperty 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f7dcde9a4aeed38bd4891d425b1a174f9ad3d549
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051035"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="0b514-103">获取 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="0b514-103">Get profileCardProperty</span></span>

<span data-ttu-id="0b514-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b514-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b514-105">检索[profileCardProperty](../resources/profilecardproperty.md)实体的属性和关系，其中包含在给定字段的 Microsoft 365 组织中存在的配置文件卡片自定义项。</span><span class="sxs-lookup"><span data-stu-id="0b514-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="0b514-106">ProfileCardProperty 由其**directoryPropertyName**属性标识。</span><span class="sxs-lookup"><span data-stu-id="0b514-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b514-107">权限</span><span class="sxs-lookup"><span data-stu-id="0b514-107">Permissions</span></span>

<span data-ttu-id="0b514-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0b514-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0b514-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b514-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b514-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b514-110">Permission type</span></span>                        | <span data-ttu-id="0b514-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b514-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b514-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b514-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b514-113">User. Read、User. All</span><span class="sxs-lookup"><span data-stu-id="0b514-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="0b514-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b514-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b514-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b514-115">Not supported.</span></span>                              |
| <span data-ttu-id="0b514-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b514-116">Application</span></span>                            | <span data-ttu-id="0b514-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b514-117">Not supported.</span></span>                              |

><span data-ttu-id="0b514-118">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="0b514-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b514-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b514-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b514-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b514-120">Optional query parameters</span></span>

<span data-ttu-id="0b514-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b514-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b514-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b514-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b514-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b514-123">Request headers</span></span>

| <span data-ttu-id="0b514-124">名称</span><span class="sxs-lookup"><span data-stu-id="0b514-124">Name</span></span>      |<span data-ttu-id="0b514-125">说明</span><span class="sxs-lookup"><span data-stu-id="0b514-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b514-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b514-126">Authorization</span></span> | <span data-ttu-id="0b514-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0b514-127">Bearer {token}.</span></span> <span data-ttu-id="0b514-128">Required.</span><span class="sxs-lookup"><span data-stu-id="0b514-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b514-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b514-129">Request body</span></span>

<span data-ttu-id="0b514-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b514-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b514-131">响应</span><span class="sxs-lookup"><span data-stu-id="0b514-131">Response</span></span>

<span data-ttu-id="0b514-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b514-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b514-133">示例</span><span class="sxs-lookup"><span data-stu-id="0b514-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b514-134">请求</span><span class="sxs-lookup"><span data-stu-id="0b514-134">Request</span></span>

<span data-ttu-id="0b514-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b514-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{id}
```

### <a name="response"></a><span data-ttu-id="0b514-136">响应</span><span class="sxs-lookup"><span data-stu-id="0b514-136">Response</span></span>

<span data-ttu-id="0b514-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b514-137">The following is an example of the response.</span></span>

> <span data-ttu-id="0b514-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0b514-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b514-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0b514-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
