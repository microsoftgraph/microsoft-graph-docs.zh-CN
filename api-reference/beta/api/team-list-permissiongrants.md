---
title: 列出团队的权限管理
description: 检索团队的权限管理。
author: jecha
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 30439fab877a2de7152c7d85a81cdfb5aa818f1e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993653"
---
# <a name="list-permissiongrants-of-a-team"></a><span data-ttu-id="72119-103">列出团队的权限管理</span><span class="sxs-lookup"><span data-stu-id="72119-103">List permissionGrants of a team</span></span>

<span data-ttu-id="72119-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72119-p101">列出[团队](../resources/team.md)中[特定于资源的权限管理](../resources/resourcespecificpermissiongrant.md)。这是 Azure AD 应用列表，这些应用有权访问团队以及每个应用具有的访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="72119-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [team](../resources/team.md). This is a list of Azure AD apps that have access to the team along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="72119-107">权限</span><span class="sxs-lookup"><span data-stu-id="72119-107">Permissions</span></span>

<span data-ttu-id="72119-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72119-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72119-110">Permission Type</span></span>                        | <span data-ttu-id="72119-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72119-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                                                                                              |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="72119-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72119-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72119-113">TeamsAppInstallation.ReadForTeam、TeamsAppInstallation.ReadWriteSelfForTeam、TeamsAppInstallation.ReadWriteForTeam</span><span class="sxs-lookup"><span data-stu-id="72119-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadWriteForTeam</span></span>                                                                     |
| <span data-ttu-id="72119-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72119-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72119-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72119-115">Not supported.</span></span>                                                                                                                                                                                                                                                           |
| <span data-ttu-id="72119-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72119-116">Application</span></span>                            | <span data-ttu-id="72119-117">TeamsAppInstallation.Read.Group *、TeamsAppInstallation.ReadForTeam.All、TeamsAppInstallation.ReadWriteSelfForTeam.All、TeamsAppInstallation.ReadWriteForTeam.All、TeamsApp.Read.Group*</span><span class="sxs-lookup"><span data-stu-id="72119-117">TeamsAppInstallation.Read.Group *, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteSelfForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, TeamsApp.Read.Group*</span></span> |

> <span data-ttu-id="72119-118">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="72119-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="72119-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72119-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72119-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72119-120">Optional query parameters</span></span>

<span data-ttu-id="72119-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72119-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72119-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="72119-122">Request headers</span></span>

| <span data-ttu-id="72119-123">标头</span><span class="sxs-lookup"><span data-stu-id="72119-123">Header</span></span>           | <span data-ttu-id="72119-124">值</span><span class="sxs-lookup"><span data-stu-id="72119-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="72119-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72119-125">Authorization</span></span>    | <span data-ttu-id="72119-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72119-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72119-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72119-128">Request body</span></span>

<span data-ttu-id="72119-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72119-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72119-130">响应</span><span class="sxs-lookup"><span data-stu-id="72119-130">Response</span></span>

<span data-ttu-id="72119-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72119-131">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72119-132">示例</span><span class="sxs-lookup"><span data-stu-id="72119-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72119-133">请求</span><span class="sxs-lookup"><span data-stu-id="72119-133">Request</span></span>

<span data-ttu-id="72119-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72119-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "team_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```

---

### <a name="response"></a><span data-ttu-id="72119-135">响应</span><span class="sxs-lookup"><span data-stu-id="72119-135">Response</span></span>

<span data-ttu-id="72119-136">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="72119-136">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#permissionGrants",
    "value": [
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="72119-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="72119-137">See also</span></span>
- [<span data-ttu-id="72119-138">列出组的权限管理</span><span class="sxs-lookup"><span data-stu-id="72119-138">List permission grants of a group</span></span>](group-list-permissionGrants.md)
- [<span data-ttu-id="72119-139">列出聊天的权限管理</span><span class="sxs-lookup"><span data-stu-id="72119-139">List permission grants of a chat</span></span>](chat-list-permissionGrants.md)