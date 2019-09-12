---
title: 设备： checkMemberObjects
description: 检查指定的设备对象的组、目录角色或管理单位列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 094b3734babd69aa46e8c703ebddb592ff46307d
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853845"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="a71e0-103">设备： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a71e0-103">device: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a71e0-104">检查指定的设备对象的组列表或管理单元的成员资格。</span><span class="sxs-lookup"><span data-stu-id="a71e0-104">Check for membership in a list of groups or administrative units for the specified device object.</span></span> <span data-ttu-id="a71e0-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a71e0-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a71e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="a71e0-106">Permissions</span></span>

<span data-ttu-id="a71e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a71e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a71e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a71e0-109">Permission type</span></span>                        | <span data-ttu-id="a71e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a71e0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a71e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a71e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a71e0-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a71e0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a71e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a71e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a71e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a71e0-114">Not supported.</span></span> |
| <span data-ttu-id="a71e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a71e0-115">Application</span></span>                            | <span data-ttu-id="a71e0-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71e0-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a71e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a71e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="a71e0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a71e0-118">Request headers</span></span>

| <span data-ttu-id="a71e0-119">名称</span><span class="sxs-lookup"><span data-stu-id="a71e0-119">Name</span></span>          | <span data-ttu-id="a71e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="a71e0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a71e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a71e0-121">Authorization</span></span> | <span data-ttu-id="a71e0-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a71e0-122">Bearer {token}</span></span> |
| <span data-ttu-id="a71e0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a71e0-123">Content-Type</span></span>  | <span data-ttu-id="a71e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a71e0-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a71e0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a71e0-125">Request body</span></span>

<span data-ttu-id="a71e0-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a71e0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a71e0-127">参数</span><span class="sxs-lookup"><span data-stu-id="a71e0-127">Parameter</span></span>    | <span data-ttu-id="a71e0-128">类型</span><span class="sxs-lookup"><span data-stu-id="a71e0-128">Type</span></span>        | <span data-ttu-id="a71e0-129">说明</span><span class="sxs-lookup"><span data-stu-id="a71e0-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a71e0-130">ids</span><span class="sxs-lookup"><span data-stu-id="a71e0-130">ids</span></span> | <span data-ttu-id="a71e0-131">String collection</span><span class="sxs-lookup"><span data-stu-id="a71e0-131">String collection</span></span> | <span data-ttu-id="a71e0-132">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="a71e0-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="a71e0-133">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="a71e0-133">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="a71e0-134">响应</span><span class="sxs-lookup"><span data-stu-id="a71e0-134">Response</span></span>

<span data-ttu-id="a71e0-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="a71e0-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a71e0-136">示例</span><span class="sxs-lookup"><span data-stu-id="a71e0-136">Examples</span></span>

<span data-ttu-id="a71e0-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a71e0-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a71e0-138">请求</span><span class="sxs-lookup"><span data-stu-id="a71e0-138">Request</span></span>

<span data-ttu-id="a71e0-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a71e0-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/devices/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="a71e0-140">响应</span><span class="sxs-lookup"><span data-stu-id="a71e0-140">Response</span></span>

<span data-ttu-id="a71e0-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a71e0-141">The following is an example of the response.</span></span> 

> <span data-ttu-id="a71e0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a71e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "device: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->