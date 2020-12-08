---
title: 更新 identityUserFlowAttributeAssignment
description: 更新 userAttributeAssignments 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9b5e39cd8d7462b678608ae74727eacdf101cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581326"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="89293-103">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="89293-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="89293-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89293-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89293-105">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89293-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89293-106">权限</span><span class="sxs-lookup"><span data-stu-id="89293-106">Permissions</span></span>

<span data-ttu-id="89293-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89293-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89293-109">Permission type</span></span>|<span data-ttu-id="89293-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89293-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89293-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89293-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89293-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="89293-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="89293-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89293-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89293-114">不支持</span><span class="sxs-lookup"><span data-stu-id="89293-114">Not supported</span></span>|
|<span data-ttu-id="89293-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89293-115">Application</span></span>|<span data-ttu-id="89293-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="89293-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89293-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89293-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89293-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="89293-118">Request headers</span></span>

|<span data-ttu-id="89293-119">名称</span><span class="sxs-lookup"><span data-stu-id="89293-119">Name</span></span>|<span data-ttu-id="89293-120">说明</span><span class="sxs-lookup"><span data-stu-id="89293-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89293-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89293-121">Authorization</span></span>|<span data-ttu-id="89293-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89293-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="89293-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89293-124">Content-Type</span></span>|<span data-ttu-id="89293-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="89293-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89293-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89293-127">Request body</span></span>

<span data-ttu-id="89293-128">在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89293-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="89293-129">下表显示了可在 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)中更新的属性。</span><span class="sxs-lookup"><span data-stu-id="89293-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="89293-130">属性</span><span class="sxs-lookup"><span data-stu-id="89293-130">Property</span></span>|<span data-ttu-id="89293-131">类型</span><span class="sxs-lookup"><span data-stu-id="89293-131">Type</span></span>|<span data-ttu-id="89293-132">说明</span><span class="sxs-lookup"><span data-stu-id="89293-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89293-133">displayName</span><span class="sxs-lookup"><span data-stu-id="89293-133">displayName</span></span>|<span data-ttu-id="89293-134">String</span><span class="sxs-lookup"><span data-stu-id="89293-134">String</span></span>|<span data-ttu-id="89293-135">用户流中的 identityUserFlowAttribute 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="89293-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="89293-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="89293-136">isOptional</span></span>|<span data-ttu-id="89293-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="89293-137">Boolean</span></span>|<span data-ttu-id="89293-138">确定 identityUserFlowAttribute 是否为可选。</span><span class="sxs-lookup"><span data-stu-id="89293-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="89293-139">`true` 表示用户不必提供值。</span><span class="sxs-lookup"><span data-stu-id="89293-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="89293-140">`false` 表示用户不能完成注册，而无需提供值。</span><span class="sxs-lookup"><span data-stu-id="89293-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="89293-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="89293-141">requiresVerification</span></span>|<span data-ttu-id="89293-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="89293-142">Boolean</span></span>|<span data-ttu-id="89293-143">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="89293-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="89293-144">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="89293-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="89293-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="89293-145">userAttributeValues</span></span>|<span data-ttu-id="89293-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89293-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="89293-147">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="89293-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="89293-148">仅当 userInputType 为、或时才适用 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="89293-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="89293-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="89293-149">userInputType</span></span>|<span data-ttu-id="89293-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="89293-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="89293-151">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="89293-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="89293-152">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="89293-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="89293-153">响应</span><span class="sxs-lookup"><span data-stu-id="89293-153">Response</span></span>

<span data-ttu-id="89293-154">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89293-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89293-155">示例</span><span class="sxs-lookup"><span data-stu-id="89293-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89293-156">请求</span><span class="sxs-lookup"><span data-stu-id="89293-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a><span data-ttu-id="89293-157">响应</span><span class="sxs-lookup"><span data-stu-id="89293-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
