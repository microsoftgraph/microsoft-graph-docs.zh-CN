---
title: 更新 secureScoreControlProfile
description: 更新任何集成解决方案中的可编辑 secureScoreControlProfile 对象，以更改各种属性，如 assignedTo 或 tenantNote。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a429e08171c90b1e8c3307eaf1696c6f3016bbda
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786655"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="20c56-103">更新 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="20c56-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="20c56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20c56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20c56-105">更新任何集成解决方案中的可编辑 **secureScoreControlProfile** 对象，以更改各种属性，例如 **assignedTo** 或 **tenantNote**。</span><span class="sxs-lookup"><span data-stu-id="20c56-105">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="20c56-106">权限</span><span class="sxs-lookup"><span data-stu-id="20c56-106">Permissions</span></span>

<span data-ttu-id="20c56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20c56-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20c56-109">Permission type</span></span>      | <span data-ttu-id="20c56-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20c56-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20c56-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20c56-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="20c56-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20c56-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="20c56-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20c56-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="20c56-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20c56-114">Not supported.</span></span>  |
|<span data-ttu-id="20c56-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20c56-115">Application</span></span> | <span data-ttu-id="20c56-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20c56-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20c56-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20c56-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20c56-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="20c56-118">Request headers</span></span>

| <span data-ttu-id="20c56-119">名称</span><span class="sxs-lookup"><span data-stu-id="20c56-119">Name</span></span>       | <span data-ttu-id="20c56-120">说明</span><span class="sxs-lookup"><span data-stu-id="20c56-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="20c56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20c56-121">Authorization</span></span>  | <span data-ttu-id="20c56-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="20c56-122">Bearer {code}.</span></span> <span data-ttu-id="20c56-123">必需。</span><span class="sxs-lookup"><span data-stu-id="20c56-123">Required.</span></span>|
|<span data-ttu-id="20c56-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="20c56-124">Prefer</span></span> | <span data-ttu-id="20c56-125">return=representation。</span><span class="sxs-lookup"><span data-stu-id="20c56-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20c56-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="20c56-126">Request body</span></span>

<span data-ttu-id="20c56-127">在请求正文中，提供应更新的相关字段值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20c56-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="20c56-128">正文 **必须** 包含具有 `vendorInformation` 有效 和 字段 `provider` `vendor` 的属性。</span><span class="sxs-lookup"><span data-stu-id="20c56-128">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="20c56-129">下表列出了可以针对 **secureScoreControlProfile 更新的字段**。</span><span class="sxs-lookup"><span data-stu-id="20c56-129">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="20c56-130">请求正文中不包含的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="20c56-130">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="20c56-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="20c56-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="20c56-132">属性</span><span class="sxs-lookup"><span data-stu-id="20c56-132">Property</span></span>   | <span data-ttu-id="20c56-133">类型</span><span class="sxs-lookup"><span data-stu-id="20c56-133">Type</span></span> |<span data-ttu-id="20c56-134">说明</span><span class="sxs-lookup"><span data-stu-id="20c56-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20c56-135">assignedTo</span><span class="sxs-lookup"><span data-stu-id="20c56-135">assignedTo</span></span>|<span data-ttu-id="20c56-136">String</span><span class="sxs-lookup"><span data-stu-id="20c56-136">String</span></span>|<span data-ttu-id="20c56-137">分配了该控件的分析员的姓名，用于会审、实施或修正。</span><span class="sxs-lookup"><span data-stu-id="20c56-137">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="20c56-138">注释</span><span class="sxs-lookup"><span data-stu-id="20c56-138">comment</span></span>|<span data-ttu-id="20c56-139">String</span><span class="sxs-lookup"><span data-stu-id="20c56-139">String</span></span>|<span data-ttu-id="20c56-140">针对客户控制管理的 (分析员意见) 。</span><span class="sxs-lookup"><span data-stu-id="20c56-140">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="20c56-141">state</span><span class="sxs-lookup"><span data-stu-id="20c56-141">state</span></span>| <span data-ttu-id="20c56-142">String</span><span class="sxs-lookup"><span data-stu-id="20c56-142">String</span></span>|<span data-ttu-id="20c56-143">分析员驱动的控件设置。</span><span class="sxs-lookup"><span data-stu-id="20c56-143">Analyst driven setting on the control.</span></span> <span data-ttu-id="20c56-144">可取值为：`Default`、`Ignored`、`ThirdParty`、`Reviewed`。</span><span class="sxs-lookup"><span data-stu-id="20c56-144">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="20c56-145">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="20c56-145">vendorInformation</span></span> | [<span data-ttu-id="20c56-146">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="20c56-146">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="20c56-147">复杂类型，包含有关安全产品/服务供应商、提供程序和子 (的详细信息，例如，vendor=Microsoft;provider=SecureScore;) 。</span><span class="sxs-lookup"><span data-stu-id="20c56-147">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="20c56-148">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="20c56-148">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="20c56-149">响应</span><span class="sxs-lookup"><span data-stu-id="20c56-149">Response</span></span>

<span data-ttu-id="20c56-150">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="20c56-150">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="20c56-151">如果使用可选请求标头，则该方法在响应正文中返回 响应代码和更新的 `200 OK` [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20c56-151">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20c56-152">示例</span><span class="sxs-lookup"><span data-stu-id="20c56-152">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="20c56-153">示例 1：不带 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="20c56-153">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="20c56-154">请求</span><span class="sxs-lookup"><span data-stu-id="20c56-154">Request</span></span>

<span data-ttu-id="20c56-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20c56-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20c56-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="20c56-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_1"
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
# <a name="c"></a>[<span data-ttu-id="20c56-157">C#</span><span class="sxs-lookup"><span data-stu-id="20c56-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20c56-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20c56-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20c56-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20c56-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20c56-160">Java</span><span class="sxs-lookup"><span data-stu-id="20c56-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20c56-161">响应</span><span class="sxs-lookup"><span data-stu-id="20c56-161">Response</span></span>

<span data-ttu-id="20c56-162">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="20c56-162">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="20c56-163">示例 2：具有 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="20c56-163">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="20c56-164">请求</span><span class="sxs-lookup"><span data-stu-id="20c56-164">Request</span></span>

<span data-ttu-id="20c56-165">以下示例显示包含请求标头 `Prefer` 的请求。</span><span class="sxs-lookup"><span data-stu-id="20c56-165">The following example shows a request that includes the `Prefer` request header.</span></span>


# <a name="http"></a>[<span data-ttu-id="20c56-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="20c56-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update_2"
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
# <a name="c"></a>[<span data-ttu-id="20c56-167">C#</span><span class="sxs-lookup"><span data-stu-id="20c56-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20c56-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20c56-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20c56-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20c56-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="20c56-170">响应</span><span class="sxs-lookup"><span data-stu-id="20c56-170">Response</span></span>

<span data-ttu-id="20c56-171">下面是使用可选请求标头 `Prefer: return=representation` 时的响应示例。</span><span class="sxs-lookup"><span data-stu-id="20c56-171">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="20c56-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20c56-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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

