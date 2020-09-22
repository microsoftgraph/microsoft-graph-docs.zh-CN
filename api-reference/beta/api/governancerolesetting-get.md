---
title: 获取 governanceRoleSetting
description: 检索 governanceRoleSetting 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 619bc7e17d8f1d6501191a8d7f7fe4d50a60166e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991024"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="eed2b-103">获取 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="eed2b-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="eed2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eed2b-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eed2b-105">检索 [governanceRoleSetting](../resources/governancerolesetting.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eed2b-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eed2b-106">权限</span><span class="sxs-lookup"><span data-stu-id="eed2b-106">Permissions</span></span>
<span data-ttu-id="eed2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eed2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed2b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eed2b-109">Permission type</span></span>      | <span data-ttu-id="eed2b-110">权限</span><span class="sxs-lookup"><span data-stu-id="eed2b-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eed2b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eed2b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eed2b-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eed2b-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eed2b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eed2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eed2b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eed2b-114">Not supported.</span></span>    |
|<span data-ttu-id="eed2b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eed2b-115">Application</span></span> | <span data-ttu-id="eed2b-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="eed2b-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="eed2b-117">除了权限范围之外，此 API 还要求请求者在资源上至少具有一个角色分配， [governanceRoleSetting](../resources/governancerolesetting.md) 属于该资源。</span><span class="sxs-lookup"><span data-stu-id="eed2b-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="eed2b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eed2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eed2b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eed2b-119">Optional query parameters</span></span>
<span data-ttu-id="eed2b-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eed2b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eed2b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="eed2b-121">Request headers</span></span>
| <span data-ttu-id="eed2b-122">名称</span><span class="sxs-lookup"><span data-stu-id="eed2b-122">Name</span></span>      |<span data-ttu-id="eed2b-123">说明</span><span class="sxs-lookup"><span data-stu-id="eed2b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eed2b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eed2b-124">Authorization</span></span>  | <span data-ttu-id="eed2b-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eed2b-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed2b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eed2b-126">Request body</span></span>
<span data-ttu-id="eed2b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eed2b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eed2b-128">响应</span><span class="sxs-lookup"><span data-stu-id="eed2b-128">Response</span></span>
<span data-ttu-id="eed2b-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [governanceRoleSetting](../resources/governancerolesetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eed2b-129">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eed2b-130">示例</span><span class="sxs-lookup"><span data-stu-id="eed2b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eed2b-131">请求</span><span class="sxs-lookup"><span data-stu-id="eed2b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eed2b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="eed2b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="eed2b-133">C#</span><span class="sxs-lookup"><span data-stu-id="eed2b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eed2b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eed2b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eed2b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eed2b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eed2b-136">响应</span><span class="sxs-lookup"><span data-stu-id="eed2b-136">Response</span></span>
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
    "lastUpdatedBy": "Vishal Seri",
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
            "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Vishal Seri\",\"Email\":\"viseri@fimdev.net\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"viseri\",\"Email\":\"viseri@microsoft.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
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


