---
title: 列出 provisioningObjectSummary
description: 获取租户中发生的所有预配事件。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: ad5ff716396a2971c4112e98239484be97c2cfce
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055188"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="e2e6e-103">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="e2e6e-103">List provisioningObjectSummary</span></span>

<span data-ttu-id="e2e6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2e6e-105">获取租户中发生的所有预配事件，例如删除目标应用程序中的组或在从 HR 系统中预配用户帐户时创建用户。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-105">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e2e6e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2e6e-106">Permissions</span></span>

<span data-ttu-id="e2e6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e6e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2e6e-109">Permission type</span></span> | <span data-ttu-id="e2e6e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2e6e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2e6e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2e6e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2e6e-112">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2e6e-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="e2e6e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2e6e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2e6e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="e2e6e-114">Not supported</span></span>   |
|<span data-ttu-id="e2e6e-115">应用</span><span class="sxs-lookup"><span data-stu-id="e2e6e-115">Application</span></span> | <span data-ttu-id="e2e6e-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2e6e-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2e6e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2e6e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/provisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2e6e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2e6e-118">Optional query parameters</span></span>

<span data-ttu-id="e2e6e-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e2e6e-120">请注意，筛选器除状态外均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-120">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="e2e6e-121">名称</span><span class="sxs-lookup"><span data-stu-id="e2e6e-121">Name</span></span>     |<span data-ttu-id="e2e6e-122">说明</span><span class="sxs-lookup"><span data-stu-id="e2e6e-122">Description</span></span>                            |<span data-ttu-id="e2e6e-123">示例</span><span class="sxs-lookup"><span data-stu-id="e2e6e-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="e2e6e-124">$filter</span><span class="sxs-lookup"><span data-stu-id="e2e6e-124">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="e2e6e-125">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-125">Filters results (rows).</span></span> |/`auditLogs/provisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`
|[<span data-ttu-id="e2e6e-126">$top</span><span class="sxs-lookup"><span data-stu-id="e2e6e-126">$top</span></span>](/graph/query-parameters#top-parameter)|<span data-ttu-id="e2e6e-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-127">Sets the page size of results.</span></span>|`/auditLogs/provisioning?$top=20`|
|[<span data-ttu-id="e2e6e-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e2e6e-128">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter)|<span data-ttu-id="e2e6e-129">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-129">Retrieves the next page of results from result sets that span multiple pages.</span></span> <span data-ttu-id="e2e6e-130">必须在查询中传递顶部筛选器以生成令牌。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-130">You must pass the top filter in the query to generate the token.</span></span> <span data-ttu-id="e2e6e-131">不能指定要跳过的结果数。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-131">You cannot specify the number of results to be skipped.</span></span>|`/auditLogs/provisioning?$top=20&$skiptoken=g822a72df43b19c8ce94b71d153981b680a08800bc3e35f239dffb378ff72c25"`|

<span data-ttu-id="e2e6e-132">若要了解一般信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-132">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="e2e6e-133">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="e2e6e-133">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="e2e6e-134">属性名</span><span class="sxs-lookup"><span data-stu-id="e2e6e-134">Attribute name</span></span> |<span data-ttu-id="e2e6e-135">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="e2e6e-135">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="e2e6e-136">id</span><span class="sxs-lookup"><span data-stu-id="e2e6e-136">id</span></span>| <span data-ttu-id="e2e6e-137">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-137">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-138">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="e2e6e-138">activityDateTime</span></span>| <span data-ttu-id="e2e6e-139">eq</span><span class="sxs-lookup"><span data-stu-id="e2e6e-139">eq</span></span>|
|<span data-ttu-id="e2e6e-140">tenantid</span><span class="sxs-lookup"><span data-stu-id="e2e6e-140">tenantid</span></span>|<span data-ttu-id="e2e6e-141">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-141">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-142">jobid</span><span class="sxs-lookup"><span data-stu-id="e2e6e-142">jobid</span></span>|<span data-ttu-id="e2e6e-143">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-143">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-144">changeid</span><span class="sxs-lookup"><span data-stu-id="e2e6e-144">changeid</span></span>|<span data-ttu-id="e2e6e-145">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-145">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-146">cycleid</span><span class="sxs-lookup"><span data-stu-id="e2e6e-146">cycleid</span></span>|<span data-ttu-id="e2e6e-147">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-147">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-148">action</span><span class="sxs-lookup"><span data-stu-id="e2e6e-148">action</span></span>|<span data-ttu-id="e2e6e-149">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-149">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-150">statusInfo/status</span><span class="sxs-lookup"><span data-stu-id="e2e6e-150">statusInfo/status</span></span>|<span data-ttu-id="e2e6e-151">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-151">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-152">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="e2e6e-152">sourceSystem/displayName</span></span>|<span data-ttu-id="e2e6e-153">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-153">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-154">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="e2e6e-154">targetSystem/displayName</span></span>|<span data-ttu-id="e2e6e-155">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-155">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-156">sourceIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="e2e6e-156">sourceIdentity/identityType</span></span>|<span data-ttu-id="e2e6e-157">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-157">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-158">targetIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="e2e6e-158">targetIdentity/identityType</span></span>|<span data-ttu-id="e2e6e-159">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-159">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-160">sourceIdentity/id</span><span class="sxs-lookup"><span data-stu-id="e2e6e-160">sourceIdentity/id</span></span>|<span data-ttu-id="e2e6e-161">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-161">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-162">servicePrincipal/id</span><span class="sxs-lookup"><span data-stu-id="e2e6e-162">servicePrincipal/id</span></span>|<span data-ttu-id="e2e6e-163">eq</span><span class="sxs-lookup"><span data-stu-id="e2e6e-163">eq</span></span>|
|<span data-ttu-id="e2e6e-164">servicePrincipal/name</span><span class="sxs-lookup"><span data-stu-id="e2e6e-164">servicePrincipal/name</span></span>|<span data-ttu-id="e2e6e-165">eq</span><span class="sxs-lookup"><span data-stu-id="e2e6e-165">eq</span></span>|
|<span data-ttu-id="e2e6e-166">targetIdentity/id</span><span class="sxs-lookup"><span data-stu-id="e2e6e-166">targetIdentity/id</span></span>|<span data-ttu-id="e2e6e-167">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-167">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-168">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="e2e6e-168">sourceIdentity/displayName</span></span>|<span data-ttu-id="e2e6e-169">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-169">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-170">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="e2e6e-170">targetIdentity/displayName</span></span>|<span data-ttu-id="e2e6e-171">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-171">eq, contains</span></span>|
|<span data-ttu-id="e2e6e-172">initiatedBy/displayName</span><span class="sxs-lookup"><span data-stu-id="e2e6e-172">initiatedBy/displayName</span></span>|<span data-ttu-id="e2e6e-173">eq， contains</span><span class="sxs-lookup"><span data-stu-id="e2e6e-173">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e2e6e-174">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2e6e-174">Request headers</span></span>

| <span data-ttu-id="e2e6e-175">标头</span><span class="sxs-lookup"><span data-stu-id="e2e6e-175">Header</span></span>        | <span data-ttu-id="e2e6e-176">值</span><span class="sxs-lookup"><span data-stu-id="e2e6e-176">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="e2e6e-177">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2e6e-177">Authorization</span></span> | <span data-ttu-id="e2e6e-178">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="e2e6e-178">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2e6e-179">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2e6e-179">Request body</span></span>

<span data-ttu-id="e2e6e-180">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-180">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2e6e-181">响应</span><span class="sxs-lookup"><span data-stu-id="e2e6e-181">Response</span></span>

<span data-ttu-id="e2e6e-182">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [provisioningObjectSummary](../resources/provisioningobjectsummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-182">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2e6e-183">示例</span><span class="sxs-lookup"><span data-stu-id="e2e6e-183">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="e2e6e-184">示例 1：成功请求</span><span class="sxs-lookup"><span data-stu-id="e2e6e-184">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="e2e6e-185">请求</span><span class="sxs-lookup"><span data-stu-id="e2e6e-185">Request</span></span>

<span data-ttu-id="e2e6e-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-186">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2e6e-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2e6e-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="e2e6e-188">C#</span><span class="sxs-lookup"><span data-stu-id="e2e6e-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2e6e-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2e6e-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2e6e-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2e6e-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2e6e-191">Java</span><span class="sxs-lookup"><span data-stu-id="e2e6e-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-provisioningobjectsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2e6e-192">响应</span><span class="sxs-lookup"><span data-stu-id="e2e6e-192">Response</span></span>

<span data-ttu-id="e2e6e-193">下面是成功事件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-193">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="e2e6e-194">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-194">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-error-reponse"></a><span data-ttu-id="e2e6e-195">示例 2：错误返回</span><span class="sxs-lookup"><span data-stu-id="e2e6e-195">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="e2e6e-196">请求</span><span class="sxs-lookup"><span data-stu-id="e2e6e-196">Request</span></span>

<span data-ttu-id="e2e6e-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-197">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2e6e-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2e6e-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
# <a name="c"></a>[<span data-ttu-id="e2e6e-199">C#</span><span class="sxs-lookup"><span data-stu-id="e2e6e-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2e6e-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2e6e-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2e6e-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2e6e-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2e6e-202">Java</span><span class="sxs-lookup"><span data-stu-id="e2e6e-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-provisioningobjectsummary-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2e6e-203">响应</span><span class="sxs-lookup"><span data-stu-id="e2e6e-203">Response</span></span>

<span data-ttu-id="e2e6e-204">下面是失败的预配事件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-204">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="e2e6e-205">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2e6e-205">**Note:** The response object shown here might be shortened for readability.</span></span>

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


