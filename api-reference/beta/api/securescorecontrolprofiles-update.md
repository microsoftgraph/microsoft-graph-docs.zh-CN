---
title: 更新 secureScoreControlProfiles
description: 在任何集成的解决方案中更新可编辑的 secureScoreControlProfiles 属性以更改各种属性, 如 "分配给/分配" 或 "tenantNote"。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5c2060486fc5e007e8aa61751d14192d33e4d37c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410416"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="331f5-103">更新 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="331f5-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="331f5-104">在任何集成的解决方案中更新可编辑的**secureScoreControlProfiles**属性以更改各种属性, 如 "**分配给/分配**" 或 " **tenantNote**"。</span><span class="sxs-lookup"><span data-stu-id="331f5-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="331f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="331f5-105">Permissions</span></span>

<span data-ttu-id="331f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="331f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="331f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="331f5-108">Permission type</span></span>      | <span data-ttu-id="331f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="331f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="331f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="331f5-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="331f5-111">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="331f5-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="331f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="331f5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="331f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="331f5-113">Not supported.</span></span>  |
|<span data-ttu-id="331f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="331f5-114">Application</span></span> | <span data-ttu-id="331f5-115">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="331f5-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="331f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="331f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="331f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="331f5-117">Request headers</span></span>

| <span data-ttu-id="331f5-118">名称</span><span class="sxs-lookup"><span data-stu-id="331f5-118">Name</span></span>       | <span data-ttu-id="331f5-119">说明</span><span class="sxs-lookup"><span data-stu-id="331f5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="331f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="331f5-120">Authorization</span></span>  | <span data-ttu-id="331f5-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="331f5-121">Bearer {code}.</span></span> <span data-ttu-id="331f5-122">必需。</span><span class="sxs-lookup"><span data-stu-id="331f5-122">Required.</span></span>|
|<span data-ttu-id="331f5-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="331f5-123">Prefer</span></span> | <span data-ttu-id="331f5-124">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="331f5-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="331f5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="331f5-125">Request body</span></span>

<span data-ttu-id="331f5-126">在请求正文中, 提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="331f5-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="331f5-127">下表列出了可为 secureScoreControlProfile 更新的字段。</span><span class="sxs-lookup"><span data-stu-id="331f5-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="331f5-128">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="331f5-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="331f5-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="331f5-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="331f5-130">属性</span><span class="sxs-lookup"><span data-stu-id="331f5-130">Property</span></span>   | <span data-ttu-id="331f5-131">类型</span><span class="sxs-lookup"><span data-stu-id="331f5-131">Type</span></span> |<span data-ttu-id="331f5-132">说明</span><span class="sxs-lookup"><span data-stu-id="331f5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="331f5-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="331f5-133">assignedTo</span></span>|<span data-ttu-id="331f5-134">String</span><span class="sxs-lookup"><span data-stu-id="331f5-134">String</span></span>|<span data-ttu-id="331f5-135">为会审、实现或修正分配的控制分析员的名称。</span><span class="sxs-lookup"><span data-stu-id="331f5-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="331f5-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="331f5-136">tenantNote</span></span>|<span data-ttu-id="331f5-137">String</span><span class="sxs-lookup"><span data-stu-id="331f5-137">String</span></span>|<span data-ttu-id="331f5-138">控件上的分析师注释 (针对客户控制管理)。</span><span class="sxs-lookup"><span data-stu-id="331f5-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="331f5-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="331f5-139">controlStateUpdates</span></span>| <span data-ttu-id="331f5-140">String</span><span class="sxs-lookup"><span data-stu-id="331f5-140">String</span></span>|<span data-ttu-id="331f5-141">控件上的分析导向设置。</span><span class="sxs-lookup"><span data-stu-id="331f5-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="331f5-142">可取值为：`ignore`、`thirdParty`、`reviewed`。</span><span class="sxs-lookup"><span data-stu-id="331f5-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="331f5-143">响应</span><span class="sxs-lookup"><span data-stu-id="331f5-143">Response</span></span>

<span data-ttu-id="331f5-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="331f5-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="331f5-145">如果使用可选请求标头, 则该方法将在`200 OK`响应正文中返回响应代码和更新的[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象。</span><span class="sxs-lookup"><span data-stu-id="331f5-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="331f5-146">示例</span><span class="sxs-lookup"><span data-stu-id="331f5-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="331f5-147">请求</span><span class="sxs-lookup"><span data-stu-id="331f5-147">Request</span></span>

<span data-ttu-id="331f5-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="331f5-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="331f5-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="331f5-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="331f5-150">C#</span><span class="sxs-lookup"><span data-stu-id="331f5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="331f5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="331f5-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="331f5-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="331f5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="331f5-153">响应</span><span class="sxs-lookup"><span data-stu-id="331f5-153">Response</span></span>

<span data-ttu-id="331f5-154">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="331f5-154">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
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
