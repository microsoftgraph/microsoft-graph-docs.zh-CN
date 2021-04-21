---
title: 更新 identityUserFlowAttributeAssignment
description: 更新 userAttributeAssignments 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d0835b4f3c3fc24496cdde75ddb9d6684691c600
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920603"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="1f9ad-103">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="1f9ad-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="1f9ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f9ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f9ad-105">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f9ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f9ad-106">Permissions</span></span>

<span data-ttu-id="1f9ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f9ad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f9ad-109">Permission type</span></span>|<span data-ttu-id="1f9ad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f9ad-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f9ad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f9ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f9ad-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f9ad-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1f9ad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f9ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f9ad-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1f9ad-114">Not supported</span></span>|
|<span data-ttu-id="1f9ad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f9ad-115">Application</span></span>|<span data-ttu-id="1f9ad-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f9ad-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f9ad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f9ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f9ad-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f9ad-118">Request headers</span></span>

|<span data-ttu-id="1f9ad-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f9ad-119">Name</span></span>|<span data-ttu-id="1f9ad-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f9ad-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f9ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f9ad-121">Authorization</span></span>|<span data-ttu-id="1f9ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f9ad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f9ad-124">Content-Type</span></span>|<span data-ttu-id="1f9ad-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1f9ad-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f9ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f9ad-127">Request body</span></span>

<span data-ttu-id="1f9ad-128">在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="1f9ad-129">下表显示了可在 [identityUserFlowAttributeAssignment 中更新的属性](../resources/identityuserflowattributeassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="1f9ad-130">属性</span><span class="sxs-lookup"><span data-stu-id="1f9ad-130">Property</span></span>|<span data-ttu-id="1f9ad-131">类型</span><span class="sxs-lookup"><span data-stu-id="1f9ad-131">Type</span></span>|<span data-ttu-id="1f9ad-132">说明</span><span class="sxs-lookup"><span data-stu-id="1f9ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f9ad-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1f9ad-133">displayName</span></span>|<span data-ttu-id="1f9ad-134">String</span><span class="sxs-lookup"><span data-stu-id="1f9ad-134">String</span></span>|<span data-ttu-id="1f9ad-135">用户显示名称中的 identityUserFlowAttribute 的组。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="1f9ad-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="1f9ad-136">isOptional</span></span>|<span data-ttu-id="1f9ad-137">布尔</span><span class="sxs-lookup"><span data-stu-id="1f9ad-137">Boolean</span></span>|<span data-ttu-id="1f9ad-138">确定 identityUserFlowAttribute 是否可选。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="1f9ad-139">`true` 表示用户无需提供值。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="1f9ad-140">`false` 表示用户无法在未提供值的情况下完成注册。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="1f9ad-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="1f9ad-141">requiresVerification</span></span>|<span data-ttu-id="1f9ad-142">布尔</span><span class="sxs-lookup"><span data-stu-id="1f9ad-142">Boolean</span></span>|<span data-ttu-id="1f9ad-143">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="1f9ad-144">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="1f9ad-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="1f9ad-145">userAttributeValues</span></span>|<span data-ttu-id="1f9ad-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1f9ad-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="1f9ad-147">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="1f9ad-148">仅在 userInputType 为 `radioSingleSelect` 、 `dropdownSingleSelect` 或 时适用 `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="1f9ad-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="1f9ad-149">userInputType</span></span>|<span data-ttu-id="1f9ad-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="1f9ad-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="1f9ad-151">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="1f9ad-152">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="1f9ad-153">响应</span><span class="sxs-lookup"><span data-stu-id="1f9ad-153">Response</span></span>

<span data-ttu-id="1f9ad-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f9ad-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f9ad-155">示例</span><span class="sxs-lookup"><span data-stu-id="1f9ad-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f9ad-156">请求</span><span class="sxs-lookup"><span data-stu-id="1f9ad-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f9ad-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f9ad-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f9ad-158">C#</span><span class="sxs-lookup"><span data-stu-id="1f9ad-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userattributeassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f9ad-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f9ad-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userattributeassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f9ad-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f9ad-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userattributeassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f9ad-161">Java</span><span class="sxs-lookup"><span data-stu-id="1f9ad-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userattributeassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f9ad-162">响应</span><span class="sxs-lookup"><span data-stu-id="1f9ad-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
