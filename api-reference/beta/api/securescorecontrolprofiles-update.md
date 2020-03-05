---
title: 更新 secureScoreControlProfiles
description: 在任何集成的解决方案中更新可编辑的 secureScoreControlProfiles 属性以更改各种属性，如 "分配给/分配" 或 "tenantNote"。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7778a6a8760c368a261154b53b138ec3801701dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453620"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="6948b-103">更新 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6948b-103">Update secureScoreControlProfiles</span></span>

<span data-ttu-id="6948b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6948b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6948b-105">在任何集成的解决方案中更新可编辑的**secureScoreControlProfiles**属性以更改各种属性，如 "**分配给/分配**" 或 " **tenantNote**"。</span><span class="sxs-lookup"><span data-stu-id="6948b-105">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6948b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6948b-106">Permissions</span></span>

<span data-ttu-id="6948b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6948b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6948b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6948b-109">Permission type</span></span>      | <span data-ttu-id="6948b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6948b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6948b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6948b-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="6948b-112">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="6948b-112">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="6948b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6948b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6948b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6948b-114">Not supported.</span></span>  |
|<span data-ttu-id="6948b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6948b-115">Application</span></span> | <span data-ttu-id="6948b-116">Securityevents.readwrite.all。</span><span class="sxs-lookup"><span data-stu-id="6948b-116">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6948b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6948b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6948b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6948b-118">Request headers</span></span>

| <span data-ttu-id="6948b-119">名称</span><span class="sxs-lookup"><span data-stu-id="6948b-119">Name</span></span>       | <span data-ttu-id="6948b-120">说明</span><span class="sxs-lookup"><span data-stu-id="6948b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6948b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6948b-121">Authorization</span></span>  | <span data-ttu-id="6948b-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="6948b-122">Bearer {code}.</span></span> <span data-ttu-id="6948b-123">必需。</span><span class="sxs-lookup"><span data-stu-id="6948b-123">Required.</span></span>|
|<span data-ttu-id="6948b-124">Prefer</span><span class="sxs-lookup"><span data-stu-id="6948b-124">Prefer</span></span> | <span data-ttu-id="6948b-125">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="6948b-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6948b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6948b-126">Request body</span></span>

<span data-ttu-id="6948b-127">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6948b-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6948b-128">下表列出了可为 secureScoreControlProfile 更新的字段。</span><span class="sxs-lookup"><span data-stu-id="6948b-128">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="6948b-129">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="6948b-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="6948b-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6948b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6948b-131">属性</span><span class="sxs-lookup"><span data-stu-id="6948b-131">Property</span></span>   | <span data-ttu-id="6948b-132">类型</span><span class="sxs-lookup"><span data-stu-id="6948b-132">Type</span></span> |<span data-ttu-id="6948b-133">说明</span><span class="sxs-lookup"><span data-stu-id="6948b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6948b-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="6948b-134">assignedTo</span></span>|<span data-ttu-id="6948b-135">String</span><span class="sxs-lookup"><span data-stu-id="6948b-135">String</span></span>|<span data-ttu-id="6948b-136">为会审、实现或修正分配的控制分析员的名称。</span><span class="sxs-lookup"><span data-stu-id="6948b-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="6948b-137">tenantNote</span><span class="sxs-lookup"><span data-stu-id="6948b-137">tenantNote</span></span>|<span data-ttu-id="6948b-138">String</span><span class="sxs-lookup"><span data-stu-id="6948b-138">String</span></span>|<span data-ttu-id="6948b-139">控件上的分析师注释（针对客户控制管理）。</span><span class="sxs-lookup"><span data-stu-id="6948b-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="6948b-140">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="6948b-140">controlStateUpdates</span></span>| <span data-ttu-id="6948b-141">String</span><span class="sxs-lookup"><span data-stu-id="6948b-141">String</span></span>|<span data-ttu-id="6948b-142">控件上的分析导向设置。</span><span class="sxs-lookup"><span data-stu-id="6948b-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="6948b-143">可取值为：`ignore`、`thirdParty`、`reviewed`。</span><span class="sxs-lookup"><span data-stu-id="6948b-143">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="6948b-144">响应</span><span class="sxs-lookup"><span data-stu-id="6948b-144">Response</span></span>

<span data-ttu-id="6948b-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6948b-145">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6948b-146">如果使用可选请求标头，则该方法将在`200 OK`响应正文中返回响应代码和更新的[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6948b-146">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6948b-147">示例</span><span class="sxs-lookup"><span data-stu-id="6948b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6948b-148">请求</span><span class="sxs-lookup"><span data-stu-id="6948b-148">Request</span></span>

<span data-ttu-id="6948b-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6948b-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6948b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6948b-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6948b-151">C#</span><span class="sxs-lookup"><span data-stu-id="6948b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6948b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6948b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6948b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6948b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6948b-154">响应</span><span class="sxs-lookup"><span data-stu-id="6948b-154">Response</span></span>

<span data-ttu-id="6948b-155">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="6948b-155">The following is an example of a successful response.</span></span>
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
