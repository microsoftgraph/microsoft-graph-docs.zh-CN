---
title: 从 incompatibleGroups 中删除组
description: 删除指示组与指定访问包不兼容的链接。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9dab2d0aa8278f932648106e2db87eef513aeebd
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401033"
---
# <a name="remove-group-from-incompatiblegroups"></a><span data-ttu-id="5dc70-103">从 incompatibleGroups 中删除组</span><span class="sxs-lookup"><span data-stu-id="5dc70-103">Remove group from incompatibleGroups</span></span>

<span data-ttu-id="5dc70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dc70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc70-105">从[](../resources/group.md)[accessPackage](../resources/accesspackage.md)上标记为不兼容的组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="5dc70-105">Remove a [group](../resources/group.md) from the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="5dc70-106">权限</span><span class="sxs-lookup"><span data-stu-id="5dc70-106">Permissions</span></span>

<span data-ttu-id="5dc70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dc70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5dc70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dc70-109">Permission type</span></span>                        | <span data-ttu-id="5dc70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dc70-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5dc70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dc70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5dc70-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc70-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5dc70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dc70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dc70-114">Not supported.</span></span> |
| <span data-ttu-id="5dc70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dc70-115">Application</span></span>                            | <span data-ttu-id="5dc70-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc70-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dc70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dc70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5dc70-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dc70-118">Request headers</span></span>

| <span data-ttu-id="5dc70-119">名称</span><span class="sxs-lookup"><span data-stu-id="5dc70-119">Name</span></span>          | <span data-ttu-id="5dc70-120">说明</span><span class="sxs-lookup"><span data-stu-id="5dc70-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5dc70-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dc70-121">Authorization</span></span> | <span data-ttu-id="5dc70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dc70-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5dc70-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5dc70-124">Content-Type</span></span>  | <span data-ttu-id="5dc70-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5dc70-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5dc70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dc70-127">Request body</span></span>

<span data-ttu-id="5dc70-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dc70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dc70-129">响应</span><span class="sxs-lookup"><span data-stu-id="5dc70-129">Response</span></span>

<span data-ttu-id="5dc70-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5dc70-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dc70-132">示例</span><span class="sxs-lookup"><span data-stu-id="5dc70-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5dc70-133">请求</span><span class="sxs-lookup"><span data-stu-id="5dc70-133">Request</span></span>

<span data-ttu-id="5dc70-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5dc70-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatiblegroup_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="5dc70-135">响应</span><span class="sxs-lookup"><span data-stu-id="5dc70-135">Response</span></span>

<span data-ttu-id="5dc70-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5dc70-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


