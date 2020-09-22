---
title: 列出 provisioningObjectSummary
description: 获取租户中发生的所有设置事件。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 031cbeffbd600f86d2d5878f3fb5b6582eda8c2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047180"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="0abae-103">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="0abae-103">List provisioningObjectSummary</span></span>

<span data-ttu-id="0abae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0abae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0abae-105">获取在你的租户中发生的所有设置事件，例如，删除目标应用程序中的组或在从 HR 系统设置用户帐户时创建用户。</span><span class="sxs-lookup"><span data-stu-id="0abae-105">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0abae-106">权限</span><span class="sxs-lookup"><span data-stu-id="0abae-106">Permissions</span></span>

<span data-ttu-id="0abae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0abae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0abae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0abae-109">Permission type</span></span> | <span data-ttu-id="0abae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0abae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0abae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0abae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0abae-112">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="0abae-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="0abae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0abae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0abae-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0abae-114">Not supported</span></span>   |
|<span data-ttu-id="0abae-115">应用</span><span class="sxs-lookup"><span data-stu-id="0abae-115">Application</span></span> | <span data-ttu-id="0abae-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="0abae-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0abae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0abae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/provisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0abae-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0abae-118">Optional query parameters</span></span>

<span data-ttu-id="0abae-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0abae-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="0abae-120">请注意，除了状态之外，筛选器都是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="0abae-120">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="0abae-121">名称</span><span class="sxs-lookup"><span data-stu-id="0abae-121">Name</span></span>     |<span data-ttu-id="0abae-122">说明</span><span class="sxs-lookup"><span data-stu-id="0abae-122">Description</span></span>                            |<span data-ttu-id="0abae-123">示例</span><span class="sxs-lookup"><span data-stu-id="0abae-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="0abae-124">$filter</span><span class="sxs-lookup"><span data-stu-id="0abae-124">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="0abae-125">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="0abae-125">Filters results (rows).</span></span> |/`auditLogs/provisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`
|[<span data-ttu-id="0abae-126">$top</span><span class="sxs-lookup"><span data-stu-id="0abae-126">$top</span></span>](/graph/query-parameters#top-parameter)|<span data-ttu-id="0abae-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="0abae-127">Sets the page size of results.</span></span>|`/auditLogs/provisioning?$top=20`|
|[<span data-ttu-id="0abae-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0abae-128">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter)|<span data-ttu-id="0abae-129">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="0abae-129">Retrieves the next page of results from result sets that span multiple pages.</span></span> <span data-ttu-id="0abae-130">您必须传递查询中的 top 筛选器来生成令牌。</span><span class="sxs-lookup"><span data-stu-id="0abae-130">You must pass the top filter in the query to generate the token.</span></span> <span data-ttu-id="0abae-131">您不能指定要跳过的结果数。</span><span class="sxs-lookup"><span data-stu-id="0abae-131">You cannot specify the number of results to be skipped.</span></span>|`/auditLogs/provisioning?$top=20&$skiptoken=g822a72df43b19c8ce94b71d153981b680a08800bc3e35f239dffb378ff72c25"`|

<span data-ttu-id="0abae-132">若要了解一般信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="0abae-132">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="0abae-133">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="0abae-133">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="0abae-134">属性名</span><span class="sxs-lookup"><span data-stu-id="0abae-134">Attribute name</span></span> |<span data-ttu-id="0abae-135">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="0abae-135">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="0abae-136">id</span><span class="sxs-lookup"><span data-stu-id="0abae-136">id</span></span>| <span data-ttu-id="0abae-137">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-137">eq, contains</span></span>|
|<span data-ttu-id="0abae-138">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="0abae-138">activityDateTime</span></span>| <span data-ttu-id="0abae-139">eq</span><span class="sxs-lookup"><span data-stu-id="0abae-139">eq</span></span>|
|<span data-ttu-id="0abae-140">tenantid</span><span class="sxs-lookup"><span data-stu-id="0abae-140">tenantid</span></span>|<span data-ttu-id="0abae-141">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-141">eq, contains</span></span>|
|<span data-ttu-id="0abae-142">jobid</span><span class="sxs-lookup"><span data-stu-id="0abae-142">jobid</span></span>|<span data-ttu-id="0abae-143">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-143">eq, contains</span></span>|
|<span data-ttu-id="0abae-144">changeid</span><span class="sxs-lookup"><span data-stu-id="0abae-144">changeid</span></span>|<span data-ttu-id="0abae-145">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-145">eq, contains</span></span>|
|<span data-ttu-id="0abae-146">cycleid</span><span class="sxs-lookup"><span data-stu-id="0abae-146">cycleid</span></span>|<span data-ttu-id="0abae-147">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-147">eq, contains</span></span>|
|<span data-ttu-id="0abae-148">action</span><span class="sxs-lookup"><span data-stu-id="0abae-148">action</span></span>|<span data-ttu-id="0abae-149">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-149">eq, contains</span></span>|
|<span data-ttu-id="0abae-150">statusInfo/状态</span><span class="sxs-lookup"><span data-stu-id="0abae-150">statusInfo/status</span></span>|<span data-ttu-id="0abae-151">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-151">eq, contains</span></span>|
|<span data-ttu-id="0abae-152">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="0abae-152">sourceSystem/displayName</span></span>|<span data-ttu-id="0abae-153">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-153">eq, contains</span></span>|
|<span data-ttu-id="0abae-154">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="0abae-154">targetSystem/displayName</span></span>|<span data-ttu-id="0abae-155">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-155">eq, contains</span></span>|
|<span data-ttu-id="0abae-156">sourceIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="0abae-156">sourceIdentity/identityType</span></span>|<span data-ttu-id="0abae-157">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-157">eq, contains</span></span>|
|<span data-ttu-id="0abae-158">targetIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="0abae-158">targetIdentity/identityType</span></span>|<span data-ttu-id="0abae-159">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-159">eq, contains</span></span>|
|<span data-ttu-id="0abae-160">sourceIdentity/id</span><span class="sxs-lookup"><span data-stu-id="0abae-160">sourceIdentity/id</span></span>|<span data-ttu-id="0abae-161">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-161">eq, contains</span></span>|
|<span data-ttu-id="0abae-162">servicePrincipal/id</span><span class="sxs-lookup"><span data-stu-id="0abae-162">servicePrincipal/id</span></span>|<span data-ttu-id="0abae-163">eq</span><span class="sxs-lookup"><span data-stu-id="0abae-163">eq</span></span>|
|<span data-ttu-id="0abae-164">servicePrincipal/名称</span><span class="sxs-lookup"><span data-stu-id="0abae-164">servicePrincipal/name</span></span>|<span data-ttu-id="0abae-165">eq</span><span class="sxs-lookup"><span data-stu-id="0abae-165">eq</span></span>|
|<span data-ttu-id="0abae-166">targetIdentity/id</span><span class="sxs-lookup"><span data-stu-id="0abae-166">targetIdentity/id</span></span>|<span data-ttu-id="0abae-167">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-167">eq, contains</span></span>|
|<span data-ttu-id="0abae-168">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="0abae-168">sourceIdentity/displayName</span></span>|<span data-ttu-id="0abae-169">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-169">eq, contains</span></span>|
|<span data-ttu-id="0abae-170">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="0abae-170">targetIdentity/displayName</span></span>|<span data-ttu-id="0abae-171">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-171">eq, contains</span></span>|
|<span data-ttu-id="0abae-172">initiatedBy/displayName</span><span class="sxs-lookup"><span data-stu-id="0abae-172">initiatedBy/displayName</span></span>|<span data-ttu-id="0abae-173">eq，包含</span><span class="sxs-lookup"><span data-stu-id="0abae-173">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0abae-174">请求标头</span><span class="sxs-lookup"><span data-stu-id="0abae-174">Request headers</span></span>

| <span data-ttu-id="0abae-175">标头</span><span class="sxs-lookup"><span data-stu-id="0abae-175">Header</span></span>        | <span data-ttu-id="0abae-176">值</span><span class="sxs-lookup"><span data-stu-id="0abae-176">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0abae-177">Authorization</span><span class="sxs-lookup"><span data-stu-id="0abae-177">Authorization</span></span> | <span data-ttu-id="0abae-178">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="0abae-178">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0abae-179">请求正文</span><span class="sxs-lookup"><span data-stu-id="0abae-179">Request body</span></span>

<span data-ttu-id="0abae-180">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0abae-180">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0abae-181">响应</span><span class="sxs-lookup"><span data-stu-id="0abae-181">Response</span></span>

<span data-ttu-id="0abae-182">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [provisioningObjectSummary](../resources/provisioningobjectsummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0abae-182">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0abae-183">示例</span><span class="sxs-lookup"><span data-stu-id="0abae-183">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="0abae-184">示例1：成功请求</span><span class="sxs-lookup"><span data-stu-id="0abae-184">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="0abae-185">请求</span><span class="sxs-lookup"><span data-stu-id="0abae-185">Request</span></span>

<span data-ttu-id="0abae-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0abae-186">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0abae-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="0abae-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="0abae-188">C#</span><span class="sxs-lookup"><span data-stu-id="0abae-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0abae-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0abae-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0abae-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0abae-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0abae-191">响应</span><span class="sxs-lookup"><span data-stu-id="0abae-191">Response</span></span>

<span data-ttu-id="0abae-192">下面是一个成功事件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="0abae-192">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="0abae-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0abae-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0abae-194">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0abae-194">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
         {
            "id": "75b5b0ae-9fc5-8d0e-e0a9-7y6a4728de56",
            "activityDateTime": "2019-05-04T03:00:54Z",
            "tenantId": "74beb175-3b80-7b63-b9d5-6f0b76082b16",
            "jobId": "aws.74beb1753b704b63b8d56f0b76082b16.10a7a801-7101-4c69-ae00-ce9f75f8460a",
            "cycleId": "b6502552-018d-79bd-8869-j47194dc65c1",
            "changeId": "b6502552-018d-89bd-9969-b49194dc65c1",
            "action": "EntryExportUpdate",
            "durationInMilliseconds": 3236,
            "statusInfo": {
                "status": "success"
            },
            "provisioningSteps": [
                {
                    "name": "EntryImport",
                    "provisioningStepType": "Import",
                    "status": "success",
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Contoso",
                    "details": {}
                },
                {
                    "name": "EntryExportUpdate",
                    "provisioningStepType": "Export",
                    "status": "success",
                    "description": "RolesCompound '60a7a801-7101-4c69-ae00-ce9f75f8460a' was updated in Azure Active Directory",
                    "details": {
                        "ReportableIdentifier": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "appId",
                    "oldValue": null,
                    "newValue": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                },
                {
                    "displayName": "Roles",
                    "oldValue": null,
                    "newValue": "jaws-prod-role2,jaws-prod-saml2, jayaws-role,jayaws-saml, TestRole,super-saml"
                },
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "6nn37b93-185a-4485-a519-50c09549f3ad"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Contoso"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.contoso.com/saml?metadata=contoso|ISV9.1|primary|z"
                },
            ],
            "servicePrincipal": {
                "id": "6cc35b93-185a-4485-a519-50c09549g3ad",
                "displayName": "Contoso"
            },
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Contoso",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "initiatingType": "System",
                "id": "",
                "displayName": "Azure AD Provisioning Service"
            },
            "sourceIdentity": {
                "identityType": "RolesCompound",
                "id": "60a7a801-7101-4c69-ae00-ce9f75f8460a",
                "displayName": "",
                "details": {}
            },
            "targetIdentity": {
                "identityType": "ServicePrincipal",
                "id": "6nn35b93-185a-4485-a519-50c09549f3ad",
                "displayName": "",
                "details": {}
            }
          }
    ]
}

```
### <a name="example-2-error-reponse"></a><span data-ttu-id="0abae-195">示例2：错误响应</span><span class="sxs-lookup"><span data-stu-id="0abae-195">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="0abae-196">请求</span><span class="sxs-lookup"><span data-stu-id="0abae-196">Request</span></span>

<span data-ttu-id="0abae-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0abae-197">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0abae-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="0abae-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="0abae-199">C#</span><span class="sxs-lookup"><span data-stu-id="0abae-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0abae-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0abae-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0abae-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0abae-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0abae-202">响应</span><span class="sxs-lookup"><span data-stu-id="0abae-202">Response</span></span>

<span data-ttu-id="0abae-203">下面的示例演示了失败的设置事件的响应。</span><span class="sxs-lookup"><span data-stu-id="0abae-203">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="0abae-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0abae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "ContosoOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
            "cycleId": "44576n58-v14b-70fj-8404-3d22tt46ed93",
            "changeId": "eaad2f8b-e6e3-409b-83bd-e4e2e57177d5",
            "action": "Create",
            "durationInMilliseconds": 2785,
            "sourceSystem": {
                "id": "0404601d-a9c0-4ec7-bbcd-02660120d8c9",
                "displayName": "Azure Active Directory",
                "details": {}
            },
            "targetSystem": {
                "id": "cd22f60b-5f2d-1adg-adb4-76ef31db996b",
                "displayName": "Contoso",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Contoso"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "servicePrincipal": {
                "id": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                "displayName": "Contoso"
            },
            "sourceIdentity": {
                "id": "5e6c9rae-ab4d-5239-8ad0-174391d110eb",
                "displayName": "Self-service Pilot",
                "identityType": "Group",
                "details": {}
            },
            "targetIdentity": {
                "id": "",
                "displayName": "",
                "identityType": "Group",
                "details": {}
            },
            "statusInfo": {
                "@odata.type": "#microsoft.graph.statusDetails",
                "status": "failure",
                "errorCode": "ContosoEntryConflict",
                "reason": "Message: Contoso returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Contoso via the Contoso administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Contoso application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "NonServiceFailure",
                "recommendedAction": null
            },
            "provisioningSteps": [
                {
                    "name": "EntryImportAdd",
                    "provisioningStepType": "import",
                    "status": "success",
                    "description": "Received Group 'Self-service Pilot' change of type (Add) from Azure Active Directory",
                    "details": {}
                },
                {
                    "name": "EntrySynchronizationAdd",
                    "provisioningStepType": "matching",
                    "status": "success",
                    "description": "Group 'Self-service Pilot' will be created in Contoso (Group is active and assigned in Azure Active Directory, but no matching Group was found in Contoso)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Contoso",
                    "details": {
                        "ReportableIdentifier": "Self-service Pilot"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "5e0c9eae-ad3d-4139-5ad0-174391d110eb"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                },
                {
                    "displayName": "mailEnabled",
                    "oldValue": null,
                    "newValue": "False"
                },
                {
                    "displayName": "mailNickname",
                    "oldValue": null,
                    "newValue": "5ce25n9a-4c5f-45c9-8362-ef3da29c66c5"
                },
                {
                    "displayName": "securityEnabled",
                    "oldValue": null,
                    "newValue": "True"
                },
                {
                    "displayName": "Name",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                }
            ]
       }
    ]
}

```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get provisioningObjectSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


