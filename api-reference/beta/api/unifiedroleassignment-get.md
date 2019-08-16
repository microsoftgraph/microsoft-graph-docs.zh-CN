---
title: 获取 unifiedRoleAssignment
description: 检索 unifiedRoleAssignment 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9e73fa6c299589aaf4865a547b600ba59d6e211
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437767"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="7efc1-103">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7efc1-103">Get unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7efc1-104">检索[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7efc1-104">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7efc1-105">权限</span><span class="sxs-lookup"><span data-stu-id="7efc1-105">Permissions</span></span>

<span data-ttu-id="7efc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7efc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7efc1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7efc1-108">Permission type</span></span>      | <span data-ttu-id="7efc1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7efc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7efc1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7efc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7efc1-111">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="7efc1-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7efc1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7efc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7efc1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7efc1-113">Not supported.</span></span>    |
|<span data-ttu-id="7efc1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7efc1-114">Application</span></span> | <span data-ttu-id="7efc1-115">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="7efc1-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7efc1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7efc1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7efc1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7efc1-117">Optional query parameters</span></span>

<span data-ttu-id="7efc1-118">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7efc1-118">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="7efc1-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7efc1-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7efc1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7efc1-120">Request headers</span></span>

| <span data-ttu-id="7efc1-121">名称</span><span class="sxs-lookup"><span data-stu-id="7efc1-121">Name</span></span>      |<span data-ttu-id="7efc1-122">说明</span><span class="sxs-lookup"><span data-stu-id="7efc1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7efc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7efc1-123">Authorization</span></span> | <span data-ttu-id="7efc1-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7efc1-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7efc1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7efc1-125">Request body</span></span>

<span data-ttu-id="7efc1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7efc1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7efc1-127">响应</span><span class="sxs-lookup"><span data-stu-id="7efc1-127">Response</span></span>

<span data-ttu-id="7efc1-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7efc1-128">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7efc1-129">示例</span><span class="sxs-lookup"><span data-stu-id="7efc1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7efc1-130">请求</span><span class="sxs-lookup"><span data-stu-id="7efc1-130">Request</span></span>

<span data-ttu-id="7efc1-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7efc1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="7efc1-132">响应</span><span class="sxs-lookup"><span data-stu-id="7efc1-132">Response</span></span>

<span data-ttu-id="7efc1-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7efc1-133">The following is an example of the response.</span></span>

> <span data-ttu-id="7efc1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7efc1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "resourceScope": "/",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->