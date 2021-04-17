---
title: 更新 identityUserFlowAttributeAssignment
description: 更新 userAttributeAssignments 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 42ca1bd9d646e99fb254ad01c0c00512fbba441e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882915"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="7b881-103">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7b881-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="7b881-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b881-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b881-105">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b881-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b881-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b881-106">Permissions</span></span>

<span data-ttu-id="7b881-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b881-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b881-109">Permission type</span></span>|<span data-ttu-id="7b881-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b881-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b881-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b881-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b881-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b881-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7b881-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b881-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b881-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7b881-114">Not supported</span></span>|
|<span data-ttu-id="7b881-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b881-115">Application</span></span>|<span data-ttu-id="7b881-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b881-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b881-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b881-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b881-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b881-118">Request headers</span></span>

|<span data-ttu-id="7b881-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b881-119">Name</span></span>|<span data-ttu-id="7b881-120">说明</span><span class="sxs-lookup"><span data-stu-id="7b881-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b881-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b881-121">Authorization</span></span>|<span data-ttu-id="7b881-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b881-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7b881-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b881-124">Content-Type</span></span>|<span data-ttu-id="7b881-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7b881-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b881-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b881-127">Request body</span></span>

<span data-ttu-id="7b881-128">在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b881-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="7b881-129">下表显示了可在 [identityUserFlowAttributeAssignment 中更新的属性](../resources/identityuserflowattributeassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7b881-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="7b881-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b881-130">Property</span></span>|<span data-ttu-id="7b881-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b881-131">Type</span></span>|<span data-ttu-id="7b881-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b881-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b881-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7b881-133">displayName</span></span>|<span data-ttu-id="7b881-134">String</span><span class="sxs-lookup"><span data-stu-id="7b881-134">String</span></span>|<span data-ttu-id="7b881-135">用户显示名称中的 identityUserFlowAttribute 的组。</span><span class="sxs-lookup"><span data-stu-id="7b881-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="7b881-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="7b881-136">isOptional</span></span>|<span data-ttu-id="7b881-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b881-137">Boolean</span></span>|<span data-ttu-id="7b881-138">确定 identityUserFlowAttribute 是否可选。</span><span class="sxs-lookup"><span data-stu-id="7b881-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="7b881-139">`true` 表示用户无需提供值。</span><span class="sxs-lookup"><span data-stu-id="7b881-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="7b881-140">`false` 表示用户无法在未提供值的情况下完成注册。</span><span class="sxs-lookup"><span data-stu-id="7b881-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="7b881-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="7b881-141">requiresVerification</span></span>|<span data-ttu-id="7b881-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b881-142">Boolean</span></span>|<span data-ttu-id="7b881-143">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="7b881-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="7b881-144">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7b881-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="7b881-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="7b881-145">userAttributeValues</span></span>|<span data-ttu-id="7b881-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b881-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="7b881-147">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="7b881-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="7b881-148">仅在 userInputType 为 `radioSingleSelect` 、 `dropdownSingleSelect` 或 时适用 `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="7b881-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="7b881-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="7b881-149">userInputType</span></span>|<span data-ttu-id="7b881-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="7b881-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="7b881-151">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="7b881-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="7b881-152">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="7b881-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="7b881-153">响应</span><span class="sxs-lookup"><span data-stu-id="7b881-153">Response</span></span>

<span data-ttu-id="7b881-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b881-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b881-155">示例</span><span class="sxs-lookup"><span data-stu-id="7b881-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b881-156">请求</span><span class="sxs-lookup"><span data-stu-id="7b881-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a><span data-ttu-id="7b881-157">响应</span><span class="sxs-lookup"><span data-stu-id="7b881-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
