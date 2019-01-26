---
title: 更新 secureScoreControlProfiles
description: 更新中更改各种属性，如 assignedTo 或 tenantNote 任何集成的解决方案的可编辑 secureScoreControlProfiles 属性。
localization_priority: Normal
ms.openlocfilehash: 2be11c6b369d9dc411afa5af2219c3bfa8605c8a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573359"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="9f88f-103">更新 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="9f88f-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f88f-104">更新中更改各种属性，如**assignedTo**或**tenantNote**任何集成的解决方案的可编辑**secureScoreControlProfiles**属性。</span><span class="sxs-lookup"><span data-stu-id="9f88f-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f88f-105">权限</span><span class="sxs-lookup"><span data-stu-id="9f88f-105">Permissions</span></span>

<span data-ttu-id="9f88f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f88f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f88f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f88f-108">Permission type</span></span>      | <span data-ttu-id="9f88f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f88f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f88f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f88f-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="9f88f-111">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="9f88f-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="9f88f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f88f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9f88f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f88f-113">Not supported.</span></span>  |
|<span data-ttu-id="9f88f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f88f-114">Application</span></span> | <span data-ttu-id="9f88f-115">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="9f88f-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f88f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f88f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f88f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f88f-117">Request headers</span></span>

| <span data-ttu-id="9f88f-118">名称</span><span class="sxs-lookup"><span data-stu-id="9f88f-118">Name</span></span>       | <span data-ttu-id="9f88f-119">说明</span><span class="sxs-lookup"><span data-stu-id="9f88f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f88f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f88f-120">Authorization</span></span>  | <span data-ttu-id="9f88f-p102">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f88f-p102">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="9f88f-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="9f88f-123">Prefer</span></span> | <span data-ttu-id="9f88f-124">返回 = 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f88f-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f88f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f88f-125">Request body</span></span>

<span data-ttu-id="9f88f-126">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f88f-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9f88f-127">下表列出了可以为 secureScoreControlProfile 更新字段。</span><span class="sxs-lookup"><span data-stu-id="9f88f-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="9f88f-128">不包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="9f88f-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="9f88f-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9f88f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f88f-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f88f-130">Property</span></span>   | <span data-ttu-id="9f88f-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f88f-131">Type</span></span> |<span data-ttu-id="9f88f-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f88f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f88f-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="9f88f-133">assignedTo</span></span>|<span data-ttu-id="9f88f-134">String</span><span class="sxs-lookup"><span data-stu-id="9f88f-134">String</span></span>|<span data-ttu-id="9f88f-135">分析师控件的名称分配给进行会审、 实施或修复。</span><span class="sxs-lookup"><span data-stu-id="9f88f-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="9f88f-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="9f88f-136">tenantNote</span></span>|<span data-ttu-id="9f88f-137">String</span><span class="sxs-lookup"><span data-stu-id="9f88f-137">String</span></span>|<span data-ttu-id="9f88f-138">分析师评论 （用于客户控件管理） 的控件。</span><span class="sxs-lookup"><span data-stu-id="9f88f-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="9f88f-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="9f88f-139">controlStateUpdates</span></span>| <span data-ttu-id="9f88f-140">String</span><span class="sxs-lookup"><span data-stu-id="9f88f-140">String</span></span>|<span data-ttu-id="9f88f-141">分析师驱动控件上的设置。</span><span class="sxs-lookup"><span data-stu-id="9f88f-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="9f88f-142">可取值为：`ignore`、`thirdParty`、`reviewed`。</span><span class="sxs-lookup"><span data-stu-id="9f88f-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="9f88f-143">响应</span><span class="sxs-lookup"><span data-stu-id="9f88f-143">Response</span></span>

<span data-ttu-id="9f88f-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9f88f-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9f88f-145">如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f88f-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f88f-146">示例</span><span class="sxs-lookup"><span data-stu-id="9f88f-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f88f-147">请求</span><span class="sxs-lookup"><span data-stu-id="9f88f-147">Request</span></span>

<span data-ttu-id="9f88f-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f88f-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a><span data-ttu-id="9f88f-149">响应</span><span class="sxs-lookup"><span data-stu-id="9f88f-149">Response</span></span>

<span data-ttu-id="9f88f-150">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="9f88f-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
