---
title: 列出 provisioningObjectSummary
description: 获取租户中发生的所有设置事件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a165ea63e5f2a5c99ba0f76702b0bd266bcd3835
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417757"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="89dc0-103">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="89dc0-103">List provisioningObjectSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89dc0-104">获取在你的租户中发生的所有设置事件, 例如, 删除目标应用程序中的组或在从 HR 系统设置用户帐户时创建用户。</span><span class="sxs-lookup"><span data-stu-id="89dc0-104">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="89dc0-105">权限</span><span class="sxs-lookup"><span data-stu-id="89dc0-105">Permissions</span></span>

<span data-ttu-id="89dc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89dc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="89dc0-108">Permission type</span></span>      | <span data-ttu-id="89dc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89dc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89dc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89dc0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89dc0-111">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="89dc0-111">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="89dc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89dc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89dc0-113">不支持</span><span class="sxs-lookup"><span data-stu-id="89dc0-113">Not supported</span></span>   |
|<span data-ttu-id="89dc0-114">应用</span><span class="sxs-lookup"><span data-stu-id="89dc0-114">Application</span></span> | <span data-ttu-id="89dc0-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="89dc0-115">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89dc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89dc0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryProvisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89dc0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89dc0-117">Optional query parameters</span></span>

<span data-ttu-id="89dc0-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="89dc0-118">This method supports the following OData query parameter to help customize the response.</span></span> <span data-ttu-id="89dc0-119">请注意, 除了状态之外, 筛选器都是区分大小写的。</span><span class="sxs-lookup"><span data-stu-id="89dc0-119">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="89dc0-120">名称</span><span class="sxs-lookup"><span data-stu-id="89dc0-120">Name</span></span>     |<span data-ttu-id="89dc0-121">说明</span><span class="sxs-lookup"><span data-stu-id="89dc0-121">Description</span></span>                            |<span data-ttu-id="89dc0-122">示例</span><span class="sxs-lookup"><span data-stu-id="89dc0-122">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="89dc0-123">$filter</span><span class="sxs-lookup"><span data-stu-id="89dc0-123">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="89dc0-124">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="89dc0-124">Filters results (rows).</span></span> |/`auditLogs/directoryProvisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`

<span data-ttu-id="89dc0-125">有关一般信息, 请参阅[OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="89dc0-125">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="89dc0-126">$Filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="89dc0-126">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="89dc0-127">属性名</span><span class="sxs-lookup"><span data-stu-id="89dc0-127">Attribute name</span></span> |<span data-ttu-id="89dc0-128">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="89dc0-128">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="89dc0-129">id</span><span class="sxs-lookup"><span data-stu-id="89dc0-129">id</span></span>| <span data-ttu-id="89dc0-130">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-130">eq, contains</span></span>|
|<span data-ttu-id="89dc0-131">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="89dc0-131">activityDateTime</span></span>| <span data-ttu-id="89dc0-132">eq</span><span class="sxs-lookup"><span data-stu-id="89dc0-132">eq</span></span>|
|<span data-ttu-id="89dc0-133">tenantid</span><span class="sxs-lookup"><span data-stu-id="89dc0-133">tenantid</span></span>|<span data-ttu-id="89dc0-134">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-134">eq, contains</span></span>|
|<span data-ttu-id="89dc0-135">jobid</span><span class="sxs-lookup"><span data-stu-id="89dc0-135">jobid</span></span>|<span data-ttu-id="89dc0-136">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-136">eq, contains</span></span>|
|<span data-ttu-id="89dc0-137">changeid</span><span class="sxs-lookup"><span data-stu-id="89dc0-137">changeid</span></span>|<span data-ttu-id="89dc0-138">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-138">eq, contains</span></span>|
|<span data-ttu-id="89dc0-139">cycleid</span><span class="sxs-lookup"><span data-stu-id="89dc0-139">cycleid</span></span>|<span data-ttu-id="89dc0-140">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-140">eq, contains</span></span>|
|<span data-ttu-id="89dc0-141">action</span><span class="sxs-lookup"><span data-stu-id="89dc0-141">action</span></span>|<span data-ttu-id="89dc0-142">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-142">eq, contains</span></span>|
|<span data-ttu-id="89dc0-143">statusInfo/状态</span><span class="sxs-lookup"><span data-stu-id="89dc0-143">statusInfo/status</span></span>|<span data-ttu-id="89dc0-144">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-144">eq, contains</span></span>|
|<span data-ttu-id="89dc0-145">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="89dc0-145">sourceSystem/displayName</span></span>|<span data-ttu-id="89dc0-146">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-146">eq, contains</span></span>|
|<span data-ttu-id="89dc0-147">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="89dc0-147">targetSystem/displayName</span></span>|<span data-ttu-id="89dc0-148">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-148">eq, contains</span></span>|
|<span data-ttu-id="89dc0-149">sourceIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="89dc0-149">sourceIdentity/identityType</span></span>|<span data-ttu-id="89dc0-150">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-150">eq, contains</span></span>|
|<span data-ttu-id="89dc0-151">targetIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="89dc0-151">targetIdentity/identityType</span></span>|<span data-ttu-id="89dc0-152">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-152">eq, contains</span></span>|
|<span data-ttu-id="89dc0-153">sourceIdentity/id</span><span class="sxs-lookup"><span data-stu-id="89dc0-153">sourceIdentity/id</span></span>|<span data-ttu-id="89dc0-154">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-154">eq, contains</span></span>|
|<span data-ttu-id="89dc0-155">targetIdentity/id</span><span class="sxs-lookup"><span data-stu-id="89dc0-155">targetIdentity/id</span></span>|<span data-ttu-id="89dc0-156">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-156">eq, contains</span></span>|
|<span data-ttu-id="89dc0-157">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="89dc0-157">sourceIdentity/displayName</span></span>|<span data-ttu-id="89dc0-158">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-158">eq, contains</span></span>|
|<span data-ttu-id="89dc0-159">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="89dc0-159">targetIdentity/displayName</span></span>|<span data-ttu-id="89dc0-160">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-160">eq, contains</span></span>|
|<span data-ttu-id="89dc0-161">initiatedBy/displayName</span><span class="sxs-lookup"><span data-stu-id="89dc0-161">initiatedBy/displayName</span></span>|<span data-ttu-id="89dc0-162">eq, 包含</span><span class="sxs-lookup"><span data-stu-id="89dc0-162">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="89dc0-163">请求标头</span><span class="sxs-lookup"><span data-stu-id="89dc0-163">Request headers</span></span>

| <span data-ttu-id="89dc0-164">标头</span><span class="sxs-lookup"><span data-stu-id="89dc0-164">Header</span></span>        | <span data-ttu-id="89dc0-165">值</span><span class="sxs-lookup"><span data-stu-id="89dc0-165">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="89dc0-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="89dc0-166">Authorization</span></span> | <span data-ttu-id="89dc0-167">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="89dc0-167">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89dc0-168">请求正文</span><span class="sxs-lookup"><span data-stu-id="89dc0-168">Request body</span></span>

<span data-ttu-id="89dc0-169">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89dc0-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89dc0-170">响应</span><span class="sxs-lookup"><span data-stu-id="89dc0-170">Response</span></span>

<span data-ttu-id="89dc0-171">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[provisioningObjectSummary](../resources/provisioningobjectsummary.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="89dc0-171">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89dc0-172">示例</span><span class="sxs-lookup"><span data-stu-id="89dc0-172">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="89dc0-173">示例 1: 成功请求</span><span class="sxs-lookup"><span data-stu-id="89dc0-173">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="89dc0-174">请求</span><span class="sxs-lookup"><span data-stu-id="89dc0-174">Request</span></span>

<span data-ttu-id="89dc0-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89dc0-175">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```

### <a name="response"></a><span data-ttu-id="89dc0-176">响应</span><span class="sxs-lookup"><span data-stu-id="89dc0-176">Response</span></span>

<span data-ttu-id="89dc0-177">下面是一个成功事件的响应示例。</span><span class="sxs-lookup"><span data-stu-id="89dc0-177">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="89dc0-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89dc0-178">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89dc0-179">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89dc0-179">All the properties will be returned from an actual call.</span></span>

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
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
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
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Amazon Web Services",
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
                    "newValue": "Amazon Web Services (AWS)"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z"
                },
            ],
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Amazon Web Services",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Amazon Web Services (AWS)"
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
### <a name="example-2-error-reponse"></a><span data-ttu-id="89dc0-180">示例 2: 错误响应</span><span class="sxs-lookup"><span data-stu-id="89dc0-180">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="89dc0-181">请求</span><span class="sxs-lookup"><span data-stu-id="89dc0-181">Request</span></span>

<span data-ttu-id="89dc0-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89dc0-182">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```

### <a name="response"></a><span data-ttu-id="89dc0-183">响应</span><span class="sxs-lookup"><span data-stu-id="89dc0-183">Response</span></span>

<span data-ttu-id="89dc0-184">下面的示例演示了失败的设置事件的响应。</span><span class="sxs-lookup"><span data-stu-id="89dc0-184">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="89dc0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89dc0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "BoxOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
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
                "displayName": "Box",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Box"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
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
                "errorCode": "BoxEntryConflict",
                "reason": "Message: Box returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Box via the Box administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Box application in Azure Active Directory or adding a scoping filter to exclude the user.",
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
                    "description": "Group 'Self-service Pilot' will be created in Box (Group is active and assigned in Azure Active Directory, but no matching Group was found in Box)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Box",
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
