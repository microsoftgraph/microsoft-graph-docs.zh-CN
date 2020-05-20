---
title: servicePrincipal： checkMemberObjects
description: 检查指定的服务主体对象的组、目录角色或管理单位列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad8f8b6a4b295964fad5332f86b942bfb9c8373f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289841"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="0d5b4-103">servicePrincipal： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="0d5b4-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="0d5b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d5b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d5b4-105">检查指定的[servicePrincipal](../resources/serviceprincipal.md)对象的组、目录角色或管理单位列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="0d5b4-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d5b4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d5b4-107">Permissions</span></span>

<span data-ttu-id="0d5b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d5b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d5b4-110">Permission type</span></span>                        | <span data-ttu-id="0d5b4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d5b4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d5b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d5b4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d5b4-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d5b4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="0d5b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d5b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d5b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-115">Not supported.</span></span> |
| <span data-ttu-id="0d5b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d5b4-116">Application</span></span>                            | <span data-ttu-id="0d5b4-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d5b4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d5b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d5b4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="0d5b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d5b4-119">Request headers</span></span>
| <span data-ttu-id="0d5b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="0d5b4-120">Name</span></span>       | <span data-ttu-id="0d5b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="0d5b4-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0d5b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d5b4-122">Authorization</span></span> | <span data-ttu-id="0d5b4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d5b4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d5b4-125">Content-Type</span></span> | <span data-ttu-id="0d5b4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d5b4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d5b4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d5b4-128">Request body</span></span>

<span data-ttu-id="0d5b4-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d5b4-130">参数</span><span class="sxs-lookup"><span data-stu-id="0d5b4-130">Parameter</span></span>    | <span data-ttu-id="0d5b4-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d5b4-131">Type</span></span>        | <span data-ttu-id="0d5b4-132">Description</span><span class="sxs-lookup"><span data-stu-id="0d5b4-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d5b4-133">ids</span><span class="sxs-lookup"><span data-stu-id="0d5b4-133">ids</span></span>|<span data-ttu-id="0d5b4-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0d5b4-134">String collection</span></span>|<span data-ttu-id="0d5b4-135">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-135">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="0d5b4-136">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-136">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="0d5b4-137">响应</span><span class="sxs-lookup"><span data-stu-id="0d5b4-137">Response</span></span>

<span data-ttu-id="0d5b4-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d5b4-139">示例</span><span class="sxs-lookup"><span data-stu-id="0d5b4-139">Examples</span></span>

<span data-ttu-id="0d5b4-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0d5b4-141">请求</span><span class="sxs-lookup"><span data-stu-id="0d5b4-141">Request</span></span>

<span data-ttu-id="0d5b4-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0d5b4-143">响应</span><span class="sxs-lookup"><span data-stu-id="0d5b4-143">Response</span></span>

<span data-ttu-id="0d5b4-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-144">The following is an example of the response.</span></span> 

> <span data-ttu-id="0d5b4-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d5b4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
