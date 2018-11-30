---
title: 列表 governanceRoleSettings
description: 检索 governanceRoleSettings 对资源的集合。
ms.openlocfilehash: 81aa141cecdfce65f8ca2934b2464f5978b96eac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042269"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="69af6-103">列表 governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="69af6-103">List governanceRoleSettings</span></span>

> <span data-ttu-id="69af6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69af6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69af6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69af6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69af6-106">检索[governanceRoleSettings](../resources/governancerolesetting.md)对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="69af6-106">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="69af6-107">权限</span><span class="sxs-lookup"><span data-stu-id="69af6-107">Permissions</span></span>
<span data-ttu-id="69af6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69af6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69af6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69af6-110">Permission type</span></span>      | <span data-ttu-id="69af6-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="69af6-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69af6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69af6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69af6-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="69af6-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="69af6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69af6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69af6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69af6-115">Not supported.</span></span>    |
|<span data-ttu-id="69af6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69af6-116">Application</span></span> | <span data-ttu-id="69af6-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="69af6-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="69af6-118">除了权限范围，此 API 要求具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="69af6-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="69af6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69af6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69af6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69af6-120">Optional query parameters</span></span>
<span data-ttu-id="69af6-121">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="69af6-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69af6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="69af6-122">Request headers</span></span>
| <span data-ttu-id="69af6-123">名称</span><span class="sxs-lookup"><span data-stu-id="69af6-123">Name</span></span>      |<span data-ttu-id="69af6-124">说明</span><span class="sxs-lookup"><span data-stu-id="69af6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69af6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="69af6-125">Authorization</span></span>  | <span data-ttu-id="69af6-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="69af6-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="69af6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69af6-127">Request body</span></span>
<span data-ttu-id="69af6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69af6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69af6-129">响应</span><span class="sxs-lookup"><span data-stu-id="69af6-129">Response</span></span>
<span data-ttu-id="69af6-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleSetting](../resources/governancerolesetting.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="69af6-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69af6-131">示例</span><span class="sxs-lookup"><span data-stu-id="69af6-131">Example</span></span>
<span data-ttu-id="69af6-132">本示例演示如何管理员列出资源 Wingtip Toys-prod 移角色设置。</span><span class="sxs-lookup"><span data-stu-id="69af6-132">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="69af6-133">请求</span><span class="sxs-lookup"><span data-stu-id="69af6-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="69af6-134">响应</span><span class="sxs-lookup"><span data-stu-id="69af6-134">Response</span></span>
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
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Debashis Choudhury",
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
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Debashis Choudhury\",\"Email\":\"debac@fimdev.net\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
