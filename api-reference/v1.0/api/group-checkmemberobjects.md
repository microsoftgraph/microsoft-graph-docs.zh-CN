---
title: 组： checkMemberObjects
description: 检查指定的组对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4f6bb2f940cd32940391799ff4a93387ab8ac32
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757307"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="60ebd-103">组： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="60ebd-103">group: checkMemberObjects</span></span>

<span data-ttu-id="60ebd-104">检查指定组的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="60ebd-104">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="60ebd-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="60ebd-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="60ebd-106">权限</span><span class="sxs-lookup"><span data-stu-id="60ebd-106">Permissions</span></span>

<span data-ttu-id="60ebd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60ebd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60ebd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60ebd-109">Permission type</span></span>                        | <span data-ttu-id="60ebd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60ebd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60ebd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60ebd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60ebd-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ebd-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="60ebd-113">并</span><span class="sxs-lookup"><span data-stu-id="60ebd-113">And:</span></span><br><ul><li><span data-ttu-id="60ebd-114">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="60ebd-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="60ebd-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60ebd-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="60ebd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60ebd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ebd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="60ebd-117">Not supported.</span></span> |
| <span data-ttu-id="60ebd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="60ebd-118">Application</span></span>                            | <span data-ttu-id="60ebd-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ebd-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="60ebd-120">并</span><span class="sxs-lookup"><span data-stu-id="60ebd-120">And:</span></span><br><ul><li><span data-ttu-id="60ebd-121">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="60ebd-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="60ebd-122">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ebd-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ebd-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60ebd-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="60ebd-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="60ebd-124">Request headers</span></span>

| <span data-ttu-id="60ebd-125">名称</span><span class="sxs-lookup"><span data-stu-id="60ebd-125">Name</span></span>          | <span data-ttu-id="60ebd-126">说明</span><span class="sxs-lookup"><span data-stu-id="60ebd-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60ebd-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ebd-127">Authorization</span></span> | <span data-ttu-id="60ebd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60ebd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60ebd-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60ebd-130">Content-Type</span></span>  | <span data-ttu-id="60ebd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="60ebd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ebd-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="60ebd-133">Request body</span></span>

<span data-ttu-id="60ebd-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="60ebd-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60ebd-135">参数</span><span class="sxs-lookup"><span data-stu-id="60ebd-135">Parameter</span></span>    | <span data-ttu-id="60ebd-136">类型</span><span class="sxs-lookup"><span data-stu-id="60ebd-136">Type</span></span>        | <span data-ttu-id="60ebd-137">说明</span><span class="sxs-lookup"><span data-stu-id="60ebd-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60ebd-138">ids</span><span class="sxs-lookup"><span data-stu-id="60ebd-138">ids</span></span>|<span data-ttu-id="60ebd-139">String collection</span><span class="sxs-lookup"><span data-stu-id="60ebd-139">String collection</span></span>| <span data-ttu-id="60ebd-140">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="60ebd-140">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="60ebd-141">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="60ebd-141">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="60ebd-142">响应</span><span class="sxs-lookup"><span data-stu-id="60ebd-142">Response</span></span>

<span data-ttu-id="60ebd-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="60ebd-143">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60ebd-144">示例</span><span class="sxs-lookup"><span data-stu-id="60ebd-144">Examples</span></span>

<span data-ttu-id="60ebd-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="60ebd-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="60ebd-146">请求</span><span class="sxs-lookup"><span data-stu-id="60ebd-146">Request</span></span>

<span data-ttu-id="60ebd-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="60ebd-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60ebd-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ebd-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="60ebd-149">响应</span><span class="sxs-lookup"><span data-stu-id="60ebd-149">Response</span></span>

<span data-ttu-id="60ebd-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60ebd-150">The following is an example of the response.</span></span> 

> <span data-ttu-id="60ebd-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="60ebd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
