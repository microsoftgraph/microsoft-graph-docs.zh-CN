---
title: 获取 governanceRoleSetting
description: 检索 governanceRoleSetting 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 76600ce851c0319a47bfbf4450c52a895a1b7ee5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435803"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="72fe0-103">获取 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="72fe0-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="72fe0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72fe0-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72fe0-105">检索 [governanceRoleSetting](../resources/governancerolesetting.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72fe0-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72fe0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="72fe0-106">Permissions</span></span>
<span data-ttu-id="72fe0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="72fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="72fe0-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="72fe0-109">Azure resources</span></span>

| <span data-ttu-id="72fe0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72fe0-110">Permission type</span></span> | <span data-ttu-id="72fe0-111">权限</span><span class="sxs-lookup"><span data-stu-id="72fe0-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="72fe0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72fe0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72fe0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="72fe0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72fe0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fe0-115">Not supported.</span></span> |
| <span data-ttu-id="72fe0-116">Application</span><span class="sxs-lookup"><span data-stu-id="72fe0-116">Application</span></span> | <span data-ttu-id="72fe0-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72fe0-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="72fe0-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="72fe0-118">Azure AD</span></span>

| <span data-ttu-id="72fe0-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="72fe0-119">Permission type</span></span> | <span data-ttu-id="72fe0-120">权限</span><span class="sxs-lookup"><span data-stu-id="72fe0-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="72fe0-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-121">Delegated (work or school account)</span></span> | <span data-ttu-id="72fe0-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="72fe0-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="72fe0-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72fe0-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fe0-124">Not supported.</span></span> |
| <span data-ttu-id="72fe0-125">Application</span><span class="sxs-lookup"><span data-stu-id="72fe0-125">Application</span></span> | <span data-ttu-id="72fe0-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="72fe0-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="72fe0-127">组</span><span class="sxs-lookup"><span data-stu-id="72fe0-127">Groups</span></span>

|<span data-ttu-id="72fe0-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="72fe0-128">Permission type</span></span> | <span data-ttu-id="72fe0-129">权限</span><span class="sxs-lookup"><span data-stu-id="72fe0-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="72fe0-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-130">Delegated (work or school account)</span></span> | <span data-ttu-id="72fe0-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="72fe0-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="72fe0-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72fe0-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72fe0-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fe0-133">Not supported.</span></span> |
| <span data-ttu-id="72fe0-134">Application</span><span class="sxs-lookup"><span data-stu-id="72fe0-134">Application</span></span> | <span data-ttu-id="72fe0-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="72fe0-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="72fe0-136">除了权限范围之外，此 API 要求请求者至少角色分配 [governanceRoleSetting](../resources/governancerolesetting.md) 所属的资源具有一个权限。</span><span class="sxs-lookup"><span data-stu-id="72fe0-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="72fe0-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72fe0-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72fe0-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72fe0-138">Optional query parameters</span></span>
<span data-ttu-id="72fe0-139">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72fe0-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72fe0-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="72fe0-140">Request headers</span></span>
| <span data-ttu-id="72fe0-141">名称</span><span class="sxs-lookup"><span data-stu-id="72fe0-141">Name</span></span>      |<span data-ttu-id="72fe0-142">说明</span><span class="sxs-lookup"><span data-stu-id="72fe0-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72fe0-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fe0-143">Authorization</span></span>  | <span data-ttu-id="72fe0-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="72fe0-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="72fe0-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="72fe0-145">Request body</span></span>
<span data-ttu-id="72fe0-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72fe0-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="72fe0-147">响应</span><span class="sxs-lookup"><span data-stu-id="72fe0-147">Response</span></span>
<span data-ttu-id="72fe0-148">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [governanceRoleSetting](../resources/governancerolesetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fe0-148">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72fe0-149">示例</span><span class="sxs-lookup"><span data-stu-id="72fe0-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72fe0-150">请求</span><span class="sxs-lookup"><span data-stu-id="72fe0-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72fe0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="72fe0-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="72fe0-152">C#</span><span class="sxs-lookup"><span data-stu-id="72fe0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72fe0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72fe0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72fe0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72fe0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72fe0-155">Java</span><span class="sxs-lookup"><span data-stu-id="72fe0-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72fe0-156">响应</span><span class="sxs-lookup"><span data-stu-id="72fe0-156">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


