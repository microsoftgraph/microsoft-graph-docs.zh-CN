---
title: 创建 userAttributeAssignments
description: 创建新的 identityUserFlowAttributeAssignment 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52e459d65820ca1225e5aefe2eafff0f5a044ecc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944683"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="64cad-103">创建 userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="64cad-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="64cad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64cad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64cad-105">在 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)中创建新的 identityUserFlowAttributeAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="64cad-105">Create a new identityUserFlowAttributeAssignment object in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64cad-106">权限</span><span class="sxs-lookup"><span data-stu-id="64cad-106">Permissions</span></span>

<span data-ttu-id="64cad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64cad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64cad-109">Permission type</span></span>|<span data-ttu-id="64cad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64cad-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64cad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64cad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64cad-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cad-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="64cad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64cad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64cad-114">不支持</span><span class="sxs-lookup"><span data-stu-id="64cad-114">Not supported</span></span>|
|<span data-ttu-id="64cad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64cad-115">Application</span></span>|<span data-ttu-id="64cad-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cad-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64cad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64cad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="64cad-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="64cad-118">Request headers</span></span>

|<span data-ttu-id="64cad-119">名称</span><span class="sxs-lookup"><span data-stu-id="64cad-119">Name</span></span>|<span data-ttu-id="64cad-120">说明</span><span class="sxs-lookup"><span data-stu-id="64cad-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64cad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64cad-121">Authorization</span></span>|<span data-ttu-id="64cad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64cad-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64cad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64cad-124">Content-Type</span></span>|<span data-ttu-id="64cad-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="64cad-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64cad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64cad-127">Request body</span></span>

<span data-ttu-id="64cad-128">在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64cad-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="64cad-129">下表显示创建 [identityUserFlowAttributeAssignment 时所需的属性](../resources/identityuserflowattributeassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="64cad-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="64cad-130">属性</span><span class="sxs-lookup"><span data-stu-id="64cad-130">Property</span></span>|<span data-ttu-id="64cad-131">类型</span><span class="sxs-lookup"><span data-stu-id="64cad-131">Type</span></span>|<span data-ttu-id="64cad-132">说明</span><span class="sxs-lookup"><span data-stu-id="64cad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64cad-133">displayName</span><span class="sxs-lookup"><span data-stu-id="64cad-133">displayName</span></span>|<span data-ttu-id="64cad-134">String</span><span class="sxs-lookup"><span data-stu-id="64cad-134">String</span></span>|<span data-ttu-id="64cad-135">用户显示名称中的 identityUserFlowAttribute 的组。</span><span class="sxs-lookup"><span data-stu-id="64cad-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="64cad-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="64cad-136">isOptional</span></span>|<span data-ttu-id="64cad-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="64cad-137">Boolean</span></span>|<span data-ttu-id="64cad-138">确定 identityUserFlowAttribute 是否可选。</span><span class="sxs-lookup"><span data-stu-id="64cad-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="64cad-139">`true` 表示用户不必提供值。</span><span class="sxs-lookup"><span data-stu-id="64cad-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="64cad-140">`false` 表示用户无法在未提供值的情况下完成注册。</span><span class="sxs-lookup"><span data-stu-id="64cad-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="64cad-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="64cad-141">requiresVerification</span></span>|<span data-ttu-id="64cad-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="64cad-142">Boolean</span></span>|<span data-ttu-id="64cad-143">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="64cad-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="64cad-144">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="64cad-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="64cad-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="64cad-145">userAttributeValues</span></span>|<span data-ttu-id="64cad-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64cad-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="64cad-147">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="64cad-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="64cad-148">仅在 userInputType 为 `radioSingleSelect` 、 `dropdownSingleSelect` 或 时适用 `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="64cad-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="64cad-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="64cad-149">userInputType</span></span>|<span data-ttu-id="64cad-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="64cad-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="64cad-151">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="64cad-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="64cad-152">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="64cad-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="64cad-153">userAttribute</span><span class="sxs-lookup"><span data-stu-id="64cad-153">userAttribute</span></span>|[<span data-ttu-id="64cad-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="64cad-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="64cad-155">要包括在用户流分配中的用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="64cad-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="64cad-156">响应</span><span class="sxs-lookup"><span data-stu-id="64cad-156">Response</span></span>

<span data-ttu-id="64cad-157">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64cad-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64cad-158">示例</span><span class="sxs-lookup"><span data-stu-id="64cad-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64cad-159">请求</span><span class="sxs-lookup"><span data-stu-id="64cad-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="64cad-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cad-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="64cad-161">C#</span><span class="sxs-lookup"><span data-stu-id="64cad-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64cad-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64cad-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64cad-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64cad-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64cad-164">Java</span><span class="sxs-lookup"><span data-stu-id="64cad-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64cad-165">响应</span><span class="sxs-lookup"><span data-stu-id="64cad-165">Response</span></span>

<span data-ttu-id="64cad-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64cad-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2C_1_Consumer/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
