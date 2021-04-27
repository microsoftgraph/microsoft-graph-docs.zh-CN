---
title: 列出 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 062cd1d5c39c64eab9018289127eb5c6e691bd44
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054754"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="e572d-103">列出 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e572d-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e572d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e572d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e572d-105">获取 [unifiedRoleAssignmentMultiple 对象](../resources/unifiedroleassignmentmultiple.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="e572d-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="e572d-106">使用此名称获取角色分配列表中Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="e572d-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="e572d-107">For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e572d-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e572d-108">权限</span><span class="sxs-lookup"><span data-stu-id="e572d-108">Permissions</span></span>

<span data-ttu-id="e572d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e572d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e572d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e572d-111">Permission type</span></span> | <span data-ttu-id="e572d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e572d-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e572d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e572d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e572d-114">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e572d-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e572d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e572d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e572d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e572d-116">Not supported.</span></span> |
| <span data-ttu-id="e572d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e572d-117">Application</span></span> | <span data-ttu-id="e572d-118">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e572d-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e572d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e572d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e572d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e572d-120">Optional query parameters</span></span>
<span data-ttu-id="e572d-121">可以筛选 或 `roleDefinitionId` `principalId` 属性。</span><span class="sxs-lookup"><span data-stu-id="e572d-121">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="e572d-122">属性 `roleDefinitionId` 可以是角色对象 ID 或角色模板对象 ID。</span><span class="sxs-lookup"><span data-stu-id="e572d-122">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="e572d-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e572d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e572d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e572d-124">Request headers</span></span>

| <span data-ttu-id="e572d-125">名称</span><span class="sxs-lookup"><span data-stu-id="e572d-125">Name</span></span> | <span data-ttu-id="e572d-126">说明</span><span class="sxs-lookup"><span data-stu-id="e572d-126">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e572d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e572d-127">Authorization</span></span> | <span data-ttu-id="e572d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e572d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e572d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e572d-130">Request body</span></span>

<span data-ttu-id="e572d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e572d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e572d-132">响应</span><span class="sxs-lookup"><span data-stu-id="e572d-132">Response</span></span>

<span data-ttu-id="e572d-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e572d-133">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e572d-134">示例</span><span class="sxs-lookup"><span data-stu-id="e572d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e572d-135">请求</span><span class="sxs-lookup"><span data-stu-id="e572d-135">Request</span></span>

<span data-ttu-id="e572d-136">下面是一个请求示例：</span><span class="sxs-lookup"><span data-stu-id="e572d-136">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="e572d-137">响应</span><span class="sxs-lookup"><span data-stu-id="e572d-137">Response</span></span>

<span data-ttu-id="e572d-138">下面是一个响应示例：</span><span class="sxs-lookup"><span data-stu-id="e572d-138">The following is an example of the response:</span></span>
> <span data-ttu-id="e572d-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e572d-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


