---
title: 组的列表权限管理
description: 检索组的权限权限。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 136cfd8c663526882efa32ce837d2d292cf0ff5e
ms.sourcegitcommit: 8b1a6d7b0516f936ce4626246408f067527f5082
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "51594888"
---
# <a name="list-permissiongrants-of-a-group"></a><span data-ttu-id="cb85d-103">组的列表权限管理</span><span class="sxs-lookup"><span data-stu-id="cb85d-103">List permissionGrants of a group</span></span>

<span data-ttu-id="cb85d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb85d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb85d-105">列出 [组或组上](../resources/resourcespecificpermissiongrant.md) 特定 [权限](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="cb85d-105">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [group](../resources/group.md).</span></span> <span data-ttu-id="cb85d-106">这是 Azure AD 应用列表，这些应用有权访问聊天以及每个应用具有的访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="cb85d-106">This is a list of Azure AD apps that have access to the chat along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb85d-107">权限</span><span class="sxs-lookup"><span data-stu-id="cb85d-107">Permissions</span></span>

<span data-ttu-id="cb85d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb85d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb85d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb85d-110">Permission Type</span></span>                        | <span data-ttu-id="cb85d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb85d-111">Permissions (from least to most privileged)</span></span>                                          |
| :------------------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="cb85d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb85d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb85d-113">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb85d-113">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cb85d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb85d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb85d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb85d-115">Not supported.</span></span>                                                                       |
| <span data-ttu-id="cb85d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb85d-116">Application</span></span>                            | <span data-ttu-id="cb85d-117">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb85d-117">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb85d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb85d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb85d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb85d-119">Optional query parameters</span></span>

<span data-ttu-id="cb85d-120">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb85d-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb85d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb85d-121">Request headers</span></span>

| <span data-ttu-id="cb85d-122">标头</span><span class="sxs-lookup"><span data-stu-id="cb85d-122">Header</span></span>           | <span data-ttu-id="cb85d-123">值</span><span class="sxs-lookup"><span data-stu-id="cb85d-123">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="cb85d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb85d-124">Authorization</span></span>    | <span data-ttu-id="cb85d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb85d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb85d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb85d-127">Request body</span></span>

<span data-ttu-id="cb85d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb85d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb85d-129">响应</span><span class="sxs-lookup"><span data-stu-id="cb85d-129">Response</span></span>

<span data-ttu-id="cb85d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cb85d-130">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb85d-131">示例</span><span class="sxs-lookup"><span data-stu-id="cb85d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb85d-132">请求</span><span class="sxs-lookup"><span data-stu-id="cb85d-132">Request</span></span>

<span data-ttu-id="cb85d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb85d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```

---

### <a name="response"></a><span data-ttu-id="cb85d-134">响应</span><span class="sxs-lookup"><span data-stu-id="cb85d-134">Response</span></span>

<span data-ttu-id="cb85d-135">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="cb85d-135">The following example shows the response.</span></span>

><span data-ttu-id="cb85d-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb85d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#permissionGrants",
    "value": [
        {
            "id": "ZfwbxSIj9OGOBxsBmwY555mOHr_W6qN7LEbFYIIcM5A",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "WsYCHhlwjliiK19ONpJiWq6rtFy-Tg1q8h9-f-DATto",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "wtAZautz7ilRA0kgHYWr2Ss2FTK3jPkf-HPhj3FS1wo",
            "deletedDateTime": null,
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```