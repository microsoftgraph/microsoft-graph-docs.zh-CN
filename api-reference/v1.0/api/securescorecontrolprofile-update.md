---
title: 更新 secureScoreControlProfile
description: 在任何集成的解决方案中更新可编辑的 secureScoreControlProfile 对象, 以更改各种属性, 如 "分配给" 或 "tenantNote"。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 8cf86d312d9f866c24cfc0d6fc11ba523885d627
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448300"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="f1f99-103">更新 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="f1f99-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="f1f99-104">在任何集成的解决方案中更新可编辑的**secureScoreControlProfile**对象, 以更改各种属性, 如 "**分配给**" 或 " **tenantNote**"。</span><span class="sxs-lookup"><span data-stu-id="f1f99-104">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1f99-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1f99-105">Permissions</span></span>

<span data-ttu-id="f1f99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f99-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1f99-108">Permission type</span></span>      | <span data-ttu-id="f1f99-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1f99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1f99-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1f99-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="f1f99-111">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="f1f99-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="f1f99-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1f99-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1f99-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1f99-113">Not supported.</span></span>  |
|<span data-ttu-id="f1f99-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1f99-114">Application</span></span> | <span data-ttu-id="f1f99-115">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="f1f99-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1f99-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1f99-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1f99-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1f99-117">Request headers</span></span>

| <span data-ttu-id="f1f99-118">名称</span><span class="sxs-lookup"><span data-stu-id="f1f99-118">Name</span></span>       | <span data-ttu-id="f1f99-119">说明</span><span class="sxs-lookup"><span data-stu-id="f1f99-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1f99-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1f99-120">Authorization</span></span>  | <span data-ttu-id="f1f99-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="f1f99-121">Bearer {code}.</span></span> <span data-ttu-id="f1f99-122">必需。</span><span class="sxs-lookup"><span data-stu-id="f1f99-122">Required.</span></span>|
|<span data-ttu-id="f1f99-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="f1f99-123">Prefer</span></span> | <span data-ttu-id="f1f99-124">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="f1f99-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1f99-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1f99-125">Request body</span></span>

<span data-ttu-id="f1f99-126">在请求正文中, 提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1f99-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f1f99-127">正文**必须**包含具有有效`vendorInformation` `provider`和`vendor`字段的属性。</span><span class="sxs-lookup"><span data-stu-id="f1f99-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="f1f99-128">下表列出了可为**secureScoreControlProfile**更新的字段。</span><span class="sxs-lookup"><span data-stu-id="f1f99-128">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="f1f99-129">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="f1f99-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="f1f99-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f1f99-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1f99-131">属性</span><span class="sxs-lookup"><span data-stu-id="f1f99-131">Property</span></span>   | <span data-ttu-id="f1f99-132">类型</span><span class="sxs-lookup"><span data-stu-id="f1f99-132">Type</span></span> |<span data-ttu-id="f1f99-133">说明</span><span class="sxs-lookup"><span data-stu-id="f1f99-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1f99-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f1f99-134">assignedTo</span></span>|<span data-ttu-id="f1f99-135">String</span><span class="sxs-lookup"><span data-stu-id="f1f99-135">String</span></span>|<span data-ttu-id="f1f99-136">为会审、实现或修正分配的控制分析员的名称。</span><span class="sxs-lookup"><span data-stu-id="f1f99-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="f1f99-137">注释</span><span class="sxs-lookup"><span data-stu-id="f1f99-137">comment</span></span>|<span data-ttu-id="f1f99-138">String</span><span class="sxs-lookup"><span data-stu-id="f1f99-138">String</span></span>|<span data-ttu-id="f1f99-139">控件上的分析师注释 (针对客户控制管理)。</span><span class="sxs-lookup"><span data-stu-id="f1f99-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="f1f99-140">state</span><span class="sxs-lookup"><span data-stu-id="f1f99-140">state</span></span>| <span data-ttu-id="f1f99-141">String</span><span class="sxs-lookup"><span data-stu-id="f1f99-141">String</span></span>|<span data-ttu-id="f1f99-142">控件上的分析导向设置。</span><span class="sxs-lookup"><span data-stu-id="f1f99-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="f1f99-143">可取值为：`Default`、`Ignored`、`ThirdParty`、`Reviewed`。</span><span class="sxs-lookup"><span data-stu-id="f1f99-143">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="f1f99-144">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="f1f99-144">vendorInformation</span></span> | [<span data-ttu-id="f1f99-145">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f1f99-145">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="f1f99-146">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = SecureScore;)。</span><span class="sxs-lookup"><span data-stu-id="f1f99-146">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="f1f99-147">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="f1f99-147">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="f1f99-148">响应</span><span class="sxs-lookup"><span data-stu-id="f1f99-148">Response</span></span>

<span data-ttu-id="f1f99-149">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f1f99-149">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f1f99-150">如果使用可选请求标头, 则该方法将在`200 OK`响应正文中返回响应代码和更新的[secureScoreControlProfiles](../resources/securescorecontrolprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1f99-150">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1f99-151">示例</span><span class="sxs-lookup"><span data-stu-id="f1f99-151">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="f1f99-152">示例 1: 不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="f1f99-152">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="f1f99-153">请求</span><span class="sxs-lookup"><span data-stu-id="f1f99-153">Request</span></span>

<span data-ttu-id="f1f99-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f1f99-154">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1f99-155">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f1f99-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1f99-156">C#</span><span class="sxs-lookup"><span data-stu-id="f1f99-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1f99-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1f99-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1f99-158">目标-C</span><span class="sxs-lookup"><span data-stu-id="f1f99-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1f99-159">响应</span><span class="sxs-lookup"><span data-stu-id="f1f99-159">Response</span></span>

<span data-ttu-id="f1f99-160">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="f1f99-160">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="f1f99-161">示例 2: 具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="f1f99-161">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="f1f99-162">请求</span><span class="sxs-lookup"><span data-stu-id="f1f99-162">Request</span></span>

<span data-ttu-id="f1f99-163">下面的示例演示包含`Prefer`请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="f1f99-163">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="f1f99-164">响应</span><span class="sxs-lookup"><span data-stu-id="f1f99-164">Response</span></span>

<span data-ttu-id="f1f99-165">以下是使用可选`Prefer: return=representation`请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="f1f99-165">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="f1f99-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f1f99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
