---
title: 将组添加到 incompatibleGroups
description: 添加一个链接以指示组与指定的访问包不兼容。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2f599d5fc389040f7f711a08dce04c1c54ef5b3a
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401031"
---
# <a name="add-group-to-incompatiblegroups"></a><span data-ttu-id="d6ee8-103">将组添加到 incompatibleGroups</span><span class="sxs-lookup"><span data-stu-id="d6ee8-103">Add group to incompatibleGroups</span></span>

<span data-ttu-id="d6ee8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ee8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6ee8-105">将 [组](../resources/group.md) 添加到已在 [accessPackage](../resources/accesspackage.md)上标记为不兼容的组列表。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-105">Add a [group](../resources/group.md) to the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="d6ee8-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6ee8-106">Permissions</span></span>

<span data-ttu-id="d6ee8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6ee8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6ee8-109">Permission type</span></span>                        | <span data-ttu-id="d6ee8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6ee8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6ee8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6ee8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6ee8-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ee8-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d6ee8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6ee8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ee8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-114">Not supported.</span></span> |
| <span data-ttu-id="d6ee8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6ee8-115">Application</span></span>                            | <span data-ttu-id="d6ee8-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ee8-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6ee8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6ee8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d6ee8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6ee8-118">Request headers</span></span>

| <span data-ttu-id="d6ee8-119">名称</span><span class="sxs-lookup"><span data-stu-id="d6ee8-119">Name</span></span>          | <span data-ttu-id="d6ee8-120">说明</span><span class="sxs-lookup"><span data-stu-id="d6ee8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d6ee8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6ee8-121">Authorization</span></span> | <span data-ttu-id="d6ee8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6ee8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6ee8-124">Content-Type</span></span>  | <span data-ttu-id="d6ee8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d6ee8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6ee8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6ee8-127">Request body</span></span>

<span data-ttu-id="d6ee8-128">在请求正文中，使用组对象的 URI 的 OData ID 提供结构的 JSON [表示](../resources/group.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-128">In the request body, supply a JSON representation of a structure with the OData id of the URI of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d6ee8-129">响应</span><span class="sxs-lookup"><span data-stu-id="d6ee8-129">Response</span></span>

<span data-ttu-id="d6ee8-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6ee8-132">示例</span><span class="sxs-lookup"><span data-stu-id="d6ee8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6ee8-133">请求</span><span class="sxs-lookup"><span data-stu-id="d6ee8-133">Request</span></span>

<span data-ttu-id="d6ee8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6ee8-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_incompatiblegroup_to_accesspackage"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/$ref
Content-type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/groups/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}

### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Created
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

