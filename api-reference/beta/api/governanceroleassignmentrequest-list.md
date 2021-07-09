---
title: 列出 governanceRoleAssignmentRequests
description: '检索 governanceRoleAssignmentRequests 的集合。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 495a5bd0aeb8561532905003cc88ab0f22afd2b6
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350759"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="4580d-103">列出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4580d-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="4580d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4580d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4580d-105">检索 [governanceRoleAssignmentRequests 的集合](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="4580d-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4580d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4580d-106">Permissions</span></span>
<span data-ttu-id="4580d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="4580d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="4580d-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="4580d-109">Azure resources</span></span>

| <span data-ttu-id="4580d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4580d-110">Permission type</span></span> | <span data-ttu-id="4580d-111">权限</span><span class="sxs-lookup"><span data-stu-id="4580d-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="4580d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4580d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4580d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="4580d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4580d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4580d-115">Not supported.</span></span> |
| <span data-ttu-id="4580d-116">Application</span><span class="sxs-lookup"><span data-stu-id="4580d-116">Application</span></span> | <span data-ttu-id="4580d-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4580d-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="4580d-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="4580d-118">Azure AD</span></span>

| <span data-ttu-id="4580d-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4580d-119">Permission type</span></span> | <span data-ttu-id="4580d-120">权限</span><span class="sxs-lookup"><span data-stu-id="4580d-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="4580d-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="4580d-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4580d-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="4580d-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4580d-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4580d-124">Not supported.</span></span> |
| <span data-ttu-id="4580d-125">Application</span><span class="sxs-lookup"><span data-stu-id="4580d-125">Application</span></span> | <span data-ttu-id="4580d-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4580d-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="4580d-127">组</span><span class="sxs-lookup"><span data-stu-id="4580d-127">Groups</span></span>

|<span data-ttu-id="4580d-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="4580d-128">Permission type</span></span> | <span data-ttu-id="4580d-129">权限</span><span class="sxs-lookup"><span data-stu-id="4580d-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="4580d-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="4580d-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="4580d-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="4580d-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4580d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4580d-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="4580d-133">Not supported.</span></span> |
| <span data-ttu-id="4580d-134">Application</span><span class="sxs-lookup"><span data-stu-id="4580d-134">Application</span></span> | <span data-ttu-id="4580d-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="4580d-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

## <a name="http-request"></a><span data-ttu-id="4580d-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4580d-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4580d-137">列出资源上的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4580d-137">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="4580d-138">**注意：** 除了权限范围之外，请求还需要请求者至少具有一角色分配资源的权限。</span><span class="sxs-lookup"><span data-stu-id="4580d-138">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="4580d-139">列出 mine 的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4580d-139">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="4580d-140">列出正在等待管理员 [决策的 governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4580d-140">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="4580d-141">**注意：** 除了权限范围之外，此请求还要求请求者至少具有一个角色分配 (`Active` `owner` 或) `user access administrator` 管理员。</span><span class="sxs-lookup"><span data-stu-id="4580d-141">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4580d-142">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4580d-142">Optional query parameters</span></span>
<span data-ttu-id="4580d-143">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4580d-143">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4580d-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="4580d-144">Request headers</span></span>
| <span data-ttu-id="4580d-145">名称</span><span class="sxs-lookup"><span data-stu-id="4580d-145">Name</span></span>      |<span data-ttu-id="4580d-146">说明</span><span class="sxs-lookup"><span data-stu-id="4580d-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4580d-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="4580d-147">Authorization</span></span>  | <span data-ttu-id="4580d-148">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4580d-148">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4580d-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="4580d-149">Request body</span></span>
<span data-ttu-id="4580d-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4580d-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4580d-151">响应</span><span class="sxs-lookup"><span data-stu-id="4580d-151">Response</span></span>
<span data-ttu-id="4580d-152">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4580d-152">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4580d-153">示例</span><span class="sxs-lookup"><span data-stu-id="4580d-153">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="4580d-154">管理员查询挂起角色分配 Wingtip Toys - Prod 的请求。</span><span class="sxs-lookup"><span data-stu-id="4580d-154">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="4580d-155">请求</span><span class="sxs-lookup"><span data-stu-id="4580d-155">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="4580d-156">响应</span><span class="sxs-lookup"><span data-stu-id="4580d-156">Response</span></span>
<span data-ttu-id="4580d-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4580d-157">Here is an example of the response.</span></span> 

><span data-ttu-id="4580d-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4580d-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
                "statusDetails": [
                    {
                        "key": "EligibilityRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ExpirationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "MfaRule",
                        "value": "Grant"
                    },
                    {
                        "key": "JustificationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ActivationDayRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ApprovalRule",
                        "value": "Grant"
                    }
                ]
            },
            "schedule": {
                "type": "Once",
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
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
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


