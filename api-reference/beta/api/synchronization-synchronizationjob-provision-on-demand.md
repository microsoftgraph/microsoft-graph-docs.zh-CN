---
title: synchronizationJob：provisionOnDemand
description: 选择用户并按需设置帐户。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3e1007dfd7bce9ff64f54651104de943348c10dc
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240561"
---
# <a name="synchronizationjob-provisionondemand"></a><span data-ttu-id="0df26-103">synchronizationJob：provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="0df26-103">synchronizationJob: provisionOnDemand</span></span>

<span data-ttu-id="0df26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0df26-105">选择用户并按需设置帐户。</span><span class="sxs-lookup"><span data-stu-id="0df26-105">Select a user and provision the account on-demand.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df26-106">权限</span><span class="sxs-lookup"><span data-stu-id="0df26-106">Permissions</span></span>
<span data-ttu-id="0df26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0df26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0df26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0df26-109">Permission type</span></span>                        | <span data-ttu-id="0df26-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0df26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0df26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0df26-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="0df26-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0df26-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0df26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0df26-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0df26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0df26-114">Not supported.</span></span> |
|<span data-ttu-id="0df26-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0df26-115">Application</span></span>                            |<span data-ttu-id="0df26-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0df26-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0df26-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0df26-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
```

## <a name="request-headers"></a><span data-ttu-id="0df26-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0df26-118">Request headers</span></span>
|<span data-ttu-id="0df26-119">名称</span><span class="sxs-lookup"><span data-stu-id="0df26-119">Name</span></span>|<span data-ttu-id="0df26-120">说明</span><span class="sxs-lookup"><span data-stu-id="0df26-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0df26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0df26-121">Authorization</span></span>|<span data-ttu-id="0df26-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0df26-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0df26-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0df26-124">Content-Type</span></span>|<span data-ttu-id="0df26-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0df26-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0df26-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0df26-127">Request body</span></span>
<span data-ttu-id="0df26-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0df26-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0df26-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0df26-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0df26-130">参数</span><span class="sxs-lookup"><span data-stu-id="0df26-130">Parameter</span></span>|<span data-ttu-id="0df26-131">类型</span><span class="sxs-lookup"><span data-stu-id="0df26-131">Type</span></span>|<span data-ttu-id="0df26-132">说明</span><span class="sxs-lookup"><span data-stu-id="0df26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df26-133">parameters</span><span class="sxs-lookup"><span data-stu-id="0df26-133">parameters</span></span>|<span data-ttu-id="0df26-134">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0df26-134">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="0df26-135">表示将设置的对象和执行的同步规则。</span><span class="sxs-lookup"><span data-stu-id="0df26-135">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="0df26-136">资源主要用于按需预配。</span><span class="sxs-lookup"><span data-stu-id="0df26-136">The resource is primarily used for on-demand provisioning.</span></span> |



## <a name="response"></a><span data-ttu-id="0df26-137">响应</span><span class="sxs-lookup"><span data-stu-id="0df26-137">Response</span></span>

<span data-ttu-id="0df26-138">如果成功，此方法将返回 `200 OK` 响应代码和 stringKeyStringValuePair。</span><span class="sxs-lookup"><span data-stu-id="0df26-138">If successful, this method returns a `200 OK` response code and a stringKeyStringValuePair.</span></span>

## <a name="examples"></a><span data-ttu-id="0df26-139">示例</span><span class="sxs-lookup"><span data-stu-id="0df26-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0df26-140">请求</span><span class="sxs-lookup"><span data-stu-id="0df26-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0df26-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0df26-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
Content-Type: application/json
Content-length: 122

{
    "parameters": [{
      "subjects": [{
          "objectId": "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          "objectTypeName": "User"
      }],
      "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  }
```
# <a name="javascript"></a>[<span data-ttu-id="0df26-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0df26-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-provisionondemand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0df26-143">C#</span><span class="sxs-lookup"><span data-stu-id="0df26-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-provisionondemand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0df26-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0df26-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-provisionondemand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0df26-145">Java</span><span class="sxs-lookup"><span data-stu-id="0df26-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-provisionondemand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0df26-146">响应</span><span class="sxs-lookup"><span data-stu-id="0df26-146">Response</span></span>
<span data-ttu-id="0df26-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0df26-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
```
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.stringKeyStringValuePair",
    "key": "{\"result\":\"Skipped\",\"details\":{\"errorCode\":\"RedundantExport\",\"errorMessage\":\"The state of the user in both the source and target systems already match.\"}}",
    "value": "{\"action\":\"Other\",\"changeId\":\"g8ba3be8-1d7f-4a60-ae31-a8980da0a389\",\"endTime\":\"2020-06-26T13:58:24.7682084Z\",\"modifiedProperties\":[{\"displayName\":\"objectId\",\"oldValue\":null,\"newValue\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\"},{\"displayName\":\"accountEnabled\",\"oldValue\":null,\"newValue\":\"True\"},{\"displayName\":\"displayName\",\"oldValue\":null,\"newValue\":\"Bill Bob\"},{\"displayName\":\"mailNickname\",\"oldValue\":null,\"newValue\":\"Bill\"},{\"displayName\":\"userPrincipalName\",\"oldValue\":null,\"newValue\":\"BillBob@scimreftest.onmicrosoft.com\"},{\"displayName\":\"IsSoftDeleted\",\"oldValue\":null,\"newValue\":\"False\"},{\"displayName\":\"appRoleAssignments\",\"oldValue\":null,\"newValue\":\"User\"}],\"provisioningSteps\":[{\"name\":\"EntryImport\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Retrieved User 'BillBob@scimreftest.onmicrosoft.com' from Azure Active Directory\",\"timestamp\":\"2020-06-26T13:58:24.5494971Z\",\"details\":{\"objectId\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\",\"accountEnabled\":\"True\",\"displayName\":\"Fill Bob\",\"mailNickname\":\"Bill\",\"userPrincipalName\":\"BillBob@scimreftest.onmicrosoft.com\",\"IsSoftDeleted\":\"False\",\"appRoleAssignments\":\"User\"}},{\"name\":\"EntryImport\",\"type\":\"Matching\",\"status\":\"Success\",\"description\":\"Retrieved  'BillBob@scimreftest.onmicrosoft.com' from customappsso\",\"timestamp\":\"2020-06-26T13:58:24.7214072Z\",\"details\":{\"active\":\"True\",\"displayName\":\"Bill Bob\",\"externalId\":\"Bill\",\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"userName\":\"BillBob@scimreftest.onmicrosoft.com\"}},{\"name\":\"EntrySynchronizationScoping\",\"type\":\"Scoping\",\"status\":\"Success\",\"description\":\"Determine if User in scope by evaluating against each scoping filter\",\"timestamp\":\"2020-06-26T13:58:24.7526181Z\",\"details\":{\"IsActive\":\"True\",\"Assigned\":\"True\",\"IsEffectivelyEntitledForProvisioning\":\"True\",\"IsInProvisioningScopeDisplayName\":\"True\",\"ScopeEvaluationResult\":\"{}\"}},{\"name\":\"EntrySynchronizationSkip\",\"type\":\"Export\",\"status\":\"Skipped\",\"description\":\"The state of the user in both the source and target systems already match. No change to the User 'BillBob@scimreftest.onmicrosoft.com' currently needs to be made.\",\"timestamp\":\"2020-06-26T13:58:24.7682084Z\",\"details\":{\"SkipReason\":\"RedundantExport\"}}],\"reportableIdentifier\":\"BillBob@scimreftest.onmicrosoft.com\",\"startTime\":\"2020-06-26T13:58:24.5494971Z\",\"statusInfo\":{\"status\":\"Skipped\",\"errorCode\":null,\"reason\":null,\"additionalDetails\":null,\"errorCategory\":null,\"recommendedAction\":null},\"sourceIdentity\":{\"id\":\"62cf7b7a-52be-4a9b-9c69-e5d4a4a14f67\",\"type\":\"User\",\"displayName\":null,\"details\":null},\"sourceSystem\":{\"id\":null,\"name\":\"Azure Active Directory\",\"details\":null},\"targetIdentity\":{\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"type\":\"urn:ietf:params:scim:schemas:extension:enterprise:2.0:User\",\"displayName\":null,\"details\":null},\"targetSystem\":{\"id\":null,\"name\":\"customappsso\",\"details\":null}}"
}
```
