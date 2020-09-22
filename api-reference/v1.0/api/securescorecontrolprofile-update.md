---
title: 更新 secureScoreControlProfile
description: 在任何集成的解决方案中更新可编辑的 secureScoreControlProfile 对象，以更改各种属性，如 "分配给" 或 "tenantNote"。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 9e8dbf79d704e9872073812502a4f414fe68397d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971033"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="4c5d4-103">更新 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="4c5d4-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="4c5d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c5d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c5d4-105">在任何集成的解决方案中更新可编辑的 **secureScoreControlProfile** 对象，以更改各种属性，如 " **分配给** " 或 " **tenantNote**"。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-105">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c5d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c5d4-106">Permissions</span></span>

<span data-ttu-id="4c5d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c5d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c5d4-109">Permission type</span></span>      | <span data-ttu-id="4c5d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c5d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c5d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c5d4-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="4c5d4-112">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-112">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="4c5d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c5d4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c5d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-114">Not supported.</span></span>  |
|<span data-ttu-id="4c5d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c5d4-115">Application</span></span> | <span data-ttu-id="4c5d4-116">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-116">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c5d4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c5d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c5d4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c5d4-118">Request headers</span></span>

| <span data-ttu-id="4c5d4-119">名称</span><span class="sxs-lookup"><span data-stu-id="4c5d4-119">Name</span></span>       | <span data-ttu-id="4c5d4-120">说明</span><span class="sxs-lookup"><span data-stu-id="4c5d4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4c5d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c5d4-121">Authorization</span></span>  | <span data-ttu-id="4c5d4-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-122">Bearer {code}.</span></span> <span data-ttu-id="4c5d4-123">必需。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-123">Required.</span></span>|
|<span data-ttu-id="4c5d4-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="4c5d4-124">Prefer</span></span> | <span data-ttu-id="4c5d4-125">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c5d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c5d4-126">Request body</span></span>

<span data-ttu-id="4c5d4-127">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c5d4-128">正文 **必须** 包含 `vendorInformation` 具有有效 `provider` 和字段的属性 `vendor` 。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-128">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="4c5d4-129">下表列出了可为 **secureScoreControlProfile**更新的字段。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-129">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="4c5d4-130">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-130">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="4c5d4-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c5d4-132">属性</span><span class="sxs-lookup"><span data-stu-id="4c5d4-132">Property</span></span>   | <span data-ttu-id="4c5d4-133">类型</span><span class="sxs-lookup"><span data-stu-id="4c5d4-133">Type</span></span> |<span data-ttu-id="4c5d4-134">说明</span><span class="sxs-lookup"><span data-stu-id="4c5d4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c5d4-135">assignedTo</span><span class="sxs-lookup"><span data-stu-id="4c5d4-135">assignedTo</span></span>|<span data-ttu-id="4c5d4-136">String</span><span class="sxs-lookup"><span data-stu-id="4c5d4-136">String</span></span>|<span data-ttu-id="4c5d4-137">为会审、实现或修正分配的控制分析员的名称。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-137">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="4c5d4-138">注释</span><span class="sxs-lookup"><span data-stu-id="4c5d4-138">comment</span></span>|<span data-ttu-id="4c5d4-139">String</span><span class="sxs-lookup"><span data-stu-id="4c5d4-139">String</span></span>|<span data-ttu-id="4c5d4-140">针对客户控件管理) 的控件 (的分析师注释。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-140">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="4c5d4-141">state</span><span class="sxs-lookup"><span data-stu-id="4c5d4-141">state</span></span>| <span data-ttu-id="4c5d4-142">String</span><span class="sxs-lookup"><span data-stu-id="4c5d4-142">String</span></span>|<span data-ttu-id="4c5d4-143">控件上的分析导向设置。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-143">Analyst driven setting on the control.</span></span> <span data-ttu-id="4c5d4-144">可取值为：`Default`、`Ignored`、`ThirdParty`、`Reviewed`。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-144">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="4c5d4-145">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="4c5d4-145">vendorInformation</span></span> | [<span data-ttu-id="4c5d4-146">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="4c5d4-146">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="4c5d4-147">包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft;provider = SecureScore; ) 。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-147">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="4c5d4-148">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="4c5d4-148">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="4c5d4-149">响应</span><span class="sxs-lookup"><span data-stu-id="4c5d4-149">Response</span></span>

<span data-ttu-id="4c5d4-150">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-150">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="4c5d4-151">如果使用可选请求标头，则该方法将 `200 OK` 在响应正文中返回响应代码和更新的 [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-151">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c5d4-152">示例</span><span class="sxs-lookup"><span data-stu-id="4c5d4-152">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="4c5d4-153">示例1：不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="4c5d4-153">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="4c5d4-154">请求</span><span class="sxs-lookup"><span data-stu-id="4c5d4-154">Request</span></span>

<span data-ttu-id="4c5d4-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c5d4-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c5d4-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4c5d4-157">C#</span><span class="sxs-lookup"><span data-stu-id="4c5d4-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c5d4-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c5d4-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c5d4-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c5d4-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c5d4-160">Java</span><span class="sxs-lookup"><span data-stu-id="4c5d4-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c5d4-161">响应</span><span class="sxs-lookup"><span data-stu-id="4c5d4-161">Response</span></span>

<span data-ttu-id="4c5d4-162">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-162">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="4c5d4-163">示例2：具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="4c5d4-163">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="4c5d4-164">请求</span><span class="sxs-lookup"><span data-stu-id="4c5d4-164">Request</span></span>

<span data-ttu-id="4c5d4-165">下面的示例演示包含 `Prefer` 请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-165">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

#### <a name="response"></a><span data-ttu-id="4c5d4-166">响应</span><span class="sxs-lookup"><span data-stu-id="4c5d4-166">Response</span></span>

<span data-ttu-id="4c5d4-167">以下是 `Prefer: return=representation` 使用可选请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-167">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="4c5d4-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4c5d4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

