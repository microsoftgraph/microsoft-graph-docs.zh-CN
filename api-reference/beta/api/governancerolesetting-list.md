---
title: 列出 governanceRoleSettings
description: 检索资源上的 governanceRoleSettings 集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 753ffc488c67091ae1364a8cd898b294261a7b41
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435768"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="15525-103">列出 governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="15525-103">List governanceRoleSettings</span></span>

<span data-ttu-id="15525-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15525-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15525-105">检索资源上的 [governanceRoleSettings](../resources/governancerolesetting.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="15525-105">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="15525-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="15525-106">Permissions</span></span>
<span data-ttu-id="15525-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="15525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="15525-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="15525-109">Azure resources</span></span>

| <span data-ttu-id="15525-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="15525-110">Permission type</span></span> | <span data-ttu-id="15525-111">权限</span><span class="sxs-lookup"><span data-stu-id="15525-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="15525-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15525-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15525-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="15525-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15525-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="15525-115">Not supported.</span></span> |
| <span data-ttu-id="15525-116">Application</span><span class="sxs-lookup"><span data-stu-id="15525-116">Application</span></span> | <span data-ttu-id="15525-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15525-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="15525-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="15525-118">Azure AD</span></span>

| <span data-ttu-id="15525-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="15525-119">Permission type</span></span> | <span data-ttu-id="15525-120">权限</span><span class="sxs-lookup"><span data-stu-id="15525-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="15525-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-121">Delegated (work or school account)</span></span> | <span data-ttu-id="15525-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="15525-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="15525-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15525-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="15525-124">Not supported.</span></span> |
| <span data-ttu-id="15525-125">Application</span><span class="sxs-lookup"><span data-stu-id="15525-125">Application</span></span> | <span data-ttu-id="15525-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="15525-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="15525-127">组</span><span class="sxs-lookup"><span data-stu-id="15525-127">Groups</span></span>

|<span data-ttu-id="15525-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="15525-128">Permission type</span></span> | <span data-ttu-id="15525-129">权限</span><span class="sxs-lookup"><span data-stu-id="15525-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="15525-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-130">Delegated (work or school account)</span></span> | <span data-ttu-id="15525-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="15525-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="15525-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15525-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15525-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="15525-133">Not supported.</span></span> |
| <span data-ttu-id="15525-134">Application</span><span class="sxs-lookup"><span data-stu-id="15525-134">Application</span></span> | <span data-ttu-id="15525-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="15525-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="15525-136">除了权限范围之外，此 API 要求请求者至少对资源角色分配一个权限。</span><span class="sxs-lookup"><span data-stu-id="15525-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="15525-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15525-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15525-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="15525-138">Optional query parameters</span></span>
<span data-ttu-id="15525-139">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="15525-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15525-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="15525-140">Request headers</span></span>
| <span data-ttu-id="15525-141">名称</span><span class="sxs-lookup"><span data-stu-id="15525-141">Name</span></span>      |<span data-ttu-id="15525-142">说明</span><span class="sxs-lookup"><span data-stu-id="15525-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15525-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="15525-143">Authorization</span></span>  | <span data-ttu-id="15525-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="15525-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="15525-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="15525-145">Request body</span></span>
<span data-ttu-id="15525-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="15525-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15525-147">响应</span><span class="sxs-lookup"><span data-stu-id="15525-147">Response</span></span>
<span data-ttu-id="15525-148">如果成功，此方法在响应正文中返回 `200 OK` [一个响应代码和 governanceRoleSetting](../resources/governancerolesetting.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="15525-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15525-149">示例</span><span class="sxs-lookup"><span data-stu-id="15525-149">Example</span></span>
<span data-ttu-id="15525-150">此示例显示管理员如何列出资源 Wingtip Toys - Prod 的角色设置。</span><span class="sxs-lookup"><span data-stu-id="15525-150">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="15525-151">请求</span><span class="sxs-lookup"><span data-stu-id="15525-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="15525-152">响应</span><span class="sxs-lookup"><span data-stu-id="15525-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 463

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings",
    "value": [
        {
            "id": "80dc5d6f-8d89-47b3-953f-01dc909ed3f9",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "5b8bea96-e9f6-4c63-a8e9-fb092c79f0a1",
            "isDefault": false,
            "lastUpdatedDateTime": "2018-03-26T21:21:43.113Z",
            "lastUpdatedBy": "Alex Wilber",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
                }
            ]
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Allan Deyoung",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Allan Deyoung\",\"Email\":\"AllanD@contoso.com\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


