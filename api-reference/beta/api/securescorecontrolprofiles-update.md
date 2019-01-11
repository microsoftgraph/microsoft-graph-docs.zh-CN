---
title: 更新 secureScoreControlProfiles
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: b89a5e147d4882dbe25456cd2acc42b56924d12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817652"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="668ff-104">更新 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="668ff-104">Update secureScoreControlProfiles</span></span>

 > <span data-ttu-id="668ff-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="668ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="668ff-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="668ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="668ff-107">更新中更改各种属性，如**assignedTo**或**tenantNote**任何集成的解决方案的可编辑**secureScoreControlProfiles**属性。</span><span class="sxs-lookup"><span data-stu-id="668ff-107">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="668ff-108">权限</span><span class="sxs-lookup"><span data-stu-id="668ff-108">Permissions</span></span>

<span data-ttu-id="668ff-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="668ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="668ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="668ff-111">Permission type</span></span>      | <span data-ttu-id="668ff-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="668ff-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="668ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="668ff-113">Delegated (work or school account)</span></span> |   <span data-ttu-id="668ff-114">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="668ff-114">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="668ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="668ff-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="668ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="668ff-116">Not supported.</span></span>  |
|<span data-ttu-id="668ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="668ff-117">Application</span></span> | <span data-ttu-id="668ff-118">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="668ff-118">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="668ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="668ff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="668ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="668ff-120">Request headers</span></span>

| <span data-ttu-id="668ff-121">名称</span><span class="sxs-lookup"><span data-stu-id="668ff-121">Name</span></span>       | <span data-ttu-id="668ff-122">说明</span><span class="sxs-lookup"><span data-stu-id="668ff-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="668ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="668ff-123">Authorization</span></span>  | <span data-ttu-id="668ff-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="668ff-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="668ff-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="668ff-126">Prefer</span></span> | <span data-ttu-id="668ff-127">返回 = 表示形式。</span><span class="sxs-lookup"><span data-stu-id="668ff-127">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="668ff-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="668ff-128">Request body</span></span>

<span data-ttu-id="668ff-129">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="668ff-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="668ff-130">下表列出了可以为 secureScoreControlProfile 更新字段。</span><span class="sxs-lookup"><span data-stu-id="668ff-130">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="668ff-131">不包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="668ff-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="668ff-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="668ff-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="668ff-133">属性</span><span class="sxs-lookup"><span data-stu-id="668ff-133">Property</span></span>   | <span data-ttu-id="668ff-134">类型</span><span class="sxs-lookup"><span data-stu-id="668ff-134">Type</span></span> |<span data-ttu-id="668ff-135">Description</span><span class="sxs-lookup"><span data-stu-id="668ff-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="668ff-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="668ff-136">assignedTo</span></span>|<span data-ttu-id="668ff-137">字符串</span><span class="sxs-lookup"><span data-stu-id="668ff-137">String</span></span>|<span data-ttu-id="668ff-138">分析师控件的名称分配给进行会审、 实施或修复。</span><span class="sxs-lookup"><span data-stu-id="668ff-138">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="668ff-139">tenantNote</span><span class="sxs-lookup"><span data-stu-id="668ff-139">tenantNote</span></span>|<span data-ttu-id="668ff-140">字符串</span><span class="sxs-lookup"><span data-stu-id="668ff-140">String</span></span>|<span data-ttu-id="668ff-141">分析师评论 （用于客户控件管理） 的控件。</span><span class="sxs-lookup"><span data-stu-id="668ff-141">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="668ff-142">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="668ff-142">controlStateUpdates</span></span>| <span data-ttu-id="668ff-143">字符串</span><span class="sxs-lookup"><span data-stu-id="668ff-143">String</span></span>|<span data-ttu-id="668ff-144">分析师驱动控件上的设置。</span><span class="sxs-lookup"><span data-stu-id="668ff-144">Analyst driven setting on the control.</span></span> <span data-ttu-id="668ff-145">可取值为：`ignore`、`thirdParty`、`reviewed`。</span><span class="sxs-lookup"><span data-stu-id="668ff-145">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="668ff-146">响应</span><span class="sxs-lookup"><span data-stu-id="668ff-146">Response</span></span>

<span data-ttu-id="668ff-147">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="668ff-147">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="668ff-148">如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象。</span><span class="sxs-lookup"><span data-stu-id="668ff-148">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668ff-149">示例</span><span class="sxs-lookup"><span data-stu-id="668ff-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="668ff-150">请求</span><span class="sxs-lookup"><span data-stu-id="668ff-150">Request</span></span>

<span data-ttu-id="668ff-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="668ff-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="668ff-152">响应</span><span class="sxs-lookup"><span data-stu-id="668ff-152">Response</span></span>

<span data-ttu-id="668ff-153">以下是响应的成功的示例。</span><span class="sxs-lookup"><span data-stu-id="668ff-153">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
