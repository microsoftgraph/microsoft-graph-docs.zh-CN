---
title: 获取 unifiedRoleDefinition
description: 检索 unifiedRoleDefinition 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c211c1e632538bb7e703baeb2eabd6398e5ae875
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181138"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="eb630-103">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="eb630-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="eb630-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb630-105">检索[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb630-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="eb630-106">当前 "目录" 是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb630-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb630-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb630-107">Permissions</span></span>

<span data-ttu-id="eb630-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb630-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb630-110">Permission type</span></span>      | <span data-ttu-id="eb630-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb630-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb630-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb630-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb630-113">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="eb630-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb630-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb630-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb630-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb630-115">Not supported.</span></span>    |
|<span data-ttu-id="eb630-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb630-116">Application</span></span> | <span data-ttu-id="eb630-117">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="eb630-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb630-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb630-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/{rbacApplication}/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb630-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb630-119">Optional query parameters</span></span>

<span data-ttu-id="eb630-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb630-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb630-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="eb630-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb630-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb630-122">Request headers</span></span>

| <span data-ttu-id="eb630-123">名称</span><span class="sxs-lookup"><span data-stu-id="eb630-123">Name</span></span>      |<span data-ttu-id="eb630-124">说明</span><span class="sxs-lookup"><span data-stu-id="eb630-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb630-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb630-125">Authorization</span></span> | <span data-ttu-id="eb630-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="eb630-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb630-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb630-127">Request body</span></span>

<span data-ttu-id="eb630-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb630-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb630-129">响应</span><span class="sxs-lookup"><span data-stu-id="eb630-129">Response</span></span>

<span data-ttu-id="eb630-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb630-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb630-131">示例</span><span class="sxs-lookup"><span data-stu-id="eb630-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb630-132">请求</span><span class="sxs-lookup"><span data-stu-id="eb630-132">Request</span></span>

<span data-ttu-id="eb630-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb630-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb630-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb630-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="eb630-135">C#</span><span class="sxs-lookup"><span data-stu-id="eb630-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb630-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb630-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb630-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb630-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb630-138">响应</span><span class="sxs-lookup"><span data-stu-id="eb630-138">Response</span></span>

<span data-ttu-id="eb630-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb630-139">The following is an example of the response.</span></span>

> <span data-ttu-id="eb630-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb630-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "f189965f-f560-4c59-9101-933d4c87a91a",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
            ],
            "condition": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
