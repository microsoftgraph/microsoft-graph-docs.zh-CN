---
title: 获取 unifiedRoleDefinition
description: 检索 unifiedRoleDefinition 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5c4eb302ce22678b28490caedacecfac9896dd61
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437760"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="0209b-103">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0209b-103">Get unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0209b-104">检索[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0209b-104">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="0209b-105">当前 "目录" 是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0209b-105">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="0209b-106">权限</span><span class="sxs-lookup"><span data-stu-id="0209b-106">Permissions</span></span>

<span data-ttu-id="0209b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0209b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0209b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0209b-109">Permission type</span></span>      | <span data-ttu-id="0209b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0209b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0209b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0209b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0209b-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="0209b-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0209b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0209b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0209b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0209b-114">Not supported.</span></span>    |
|<span data-ttu-id="0209b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0209b-115">Application</span></span> | <span data-ttu-id="0209b-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="0209b-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0209b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0209b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/{rbacApplication}/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0209b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0209b-118">Optional query parameters</span></span>

<span data-ttu-id="0209b-119">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0209b-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="0209b-120">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0209b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0209b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0209b-121">Request headers</span></span>

| <span data-ttu-id="0209b-122">名称</span><span class="sxs-lookup"><span data-stu-id="0209b-122">Name</span></span>      |<span data-ttu-id="0209b-123">说明</span><span class="sxs-lookup"><span data-stu-id="0209b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0209b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0209b-124">Authorization</span></span> | <span data-ttu-id="0209b-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0209b-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0209b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0209b-126">Request body</span></span>

<span data-ttu-id="0209b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0209b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0209b-128">响应</span><span class="sxs-lookup"><span data-stu-id="0209b-128">Response</span></span>

<span data-ttu-id="0209b-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0209b-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0209b-130">示例</span><span class="sxs-lookup"><span data-stu-id="0209b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0209b-131">请求</span><span class="sxs-lookup"><span data-stu-id="0209b-131">Request</span></span>

<span data-ttu-id="0209b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0209b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="0209b-133">响应</span><span class="sxs-lookup"><span data-stu-id="0209b-133">Response</span></span>

<span data-ttu-id="0209b-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0209b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0209b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0209b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "resourceScopes": [
        "/"
    ],
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