---
title: 列出 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 54407dcbc45d2a14011ec50aba81bc7ddd759383
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989862"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="0fa95-103">列出 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0fa95-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0fa95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa95-105">获取 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0fa95-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="0fa95-106">使用此项可在 Microsoft Intune 中获取角色分配的列表。</span><span class="sxs-lookup"><span data-stu-id="0fa95-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="0fa95-107">对于其他 Micrsoft 365 应用程序 (如 Azure AD) ，请使用 [unifiedRoleAssignment](../resources/unifiedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa95-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa95-108">权限</span><span class="sxs-lookup"><span data-stu-id="0fa95-108">Permissions</span></span>

<span data-ttu-id="0fa95-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fa95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fa95-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fa95-111">Permission type</span></span> | <span data-ttu-id="0fa95-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fa95-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0fa95-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa95-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa95-114">Devicemanagementrbac.readwrite.all、Devicemanagementrbac.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="0fa95-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0fa95-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa95-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa95-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fa95-116">Not supported.</span></span> |
| <span data-ttu-id="0fa95-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fa95-117">Application</span></span> | <span data-ttu-id="0fa95-118">Devicemanagementrbac.readwrite.all、Devicemanagementrbac.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="0fa95-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa95-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fa95-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fa95-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0fa95-120">Optional query parameters</span></span>
<span data-ttu-id="0fa95-121">您可以对 `roleDefinitionId` 或属性进行筛选 `principalId` 。</span><span class="sxs-lookup"><span data-stu-id="0fa95-121">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="0fa95-122">该 `roleDefinitionId` 属性可以是角色对象 id，也可以是角色模板对象 id。</span><span class="sxs-lookup"><span data-stu-id="0fa95-122">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="0fa95-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0fa95-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fa95-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fa95-124">Request headers</span></span>

| <span data-ttu-id="0fa95-125">名称</span><span class="sxs-lookup"><span data-stu-id="0fa95-125">Name</span></span> | <span data-ttu-id="0fa95-126">说明</span><span class="sxs-lookup"><span data-stu-id="0fa95-126">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0fa95-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa95-127">Authorization</span></span> | <span data-ttu-id="0fa95-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fa95-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa95-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fa95-130">Request body</span></span>

<span data-ttu-id="0fa95-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fa95-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fa95-132">响应</span><span class="sxs-lookup"><span data-stu-id="0fa95-132">Response</span></span>

<span data-ttu-id="0fa95-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0fa95-133">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa95-134">示例</span><span class="sxs-lookup"><span data-stu-id="0fa95-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa95-135">请求</span><span class="sxs-lookup"><span data-stu-id="0fa95-135">Request</span></span>

<span data-ttu-id="0fa95-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0fa95-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="0fa95-137">响应</span><span class="sxs-lookup"><span data-stu-id="0fa95-137">Response</span></span>

<span data-ttu-id="0fa95-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0fa95-138">The following is an example of the response.</span></span>
> <span data-ttu-id="0fa95-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0fa95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


