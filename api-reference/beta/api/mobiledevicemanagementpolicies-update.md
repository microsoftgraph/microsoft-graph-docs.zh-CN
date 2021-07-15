---
title: 更新 mobileDeviceManagementPolicy
description: 更新移动设备管理对象的属性。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 44c3424e3b2b179d3342b06ff4f40824e8055c89
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440671"
---
# <a name="update-mobiledevicemanagementpolicy"></a><span data-ttu-id="d6e57-103">更新 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d6e57-103">Update mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="d6e57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e57-105">更新 [mobilityManagementPolicy 对象](../resources/mobilitymanagementpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d6e57-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6e57-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6e57-106">Permissions</span></span>

<span data-ttu-id="d6e57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e57-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6e57-109">Permission type</span></span>|<span data-ttu-id="d6e57-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6e57-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6e57-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6e57-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="d6e57-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="d6e57-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e57-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6e57-114">Not supported.</span></span>|
|<span data-ttu-id="d6e57-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6e57-115">Application</span></span> | <span data-ttu-id="d6e57-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6e57-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6e57-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6e57-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6e57-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6e57-118">Request headers</span></span>

|<span data-ttu-id="d6e57-119">名称</span><span class="sxs-lookup"><span data-stu-id="d6e57-119">Name</span></span>|<span data-ttu-id="d6e57-120">说明</span><span class="sxs-lookup"><span data-stu-id="d6e57-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6e57-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6e57-121">Authorization</span></span>|<span data-ttu-id="d6e57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6e57-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6e57-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6e57-124">Content-Type</span></span>|<span data-ttu-id="d6e57-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d6e57-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6e57-127">Request body</span></span>

<span data-ttu-id="d6e57-128">在请求正文中，提供 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6e57-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="d6e57-129">在请求正文中，提供下面列出的应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="d6e57-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="d6e57-130">**注意：** 不能将 `PATCH` 操作用于 `appliesTo` 其他属性。</span><span class="sxs-lookup"><span data-stu-id="d6e57-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="d6e57-131">属性</span><span class="sxs-lookup"><span data-stu-id="d6e57-131">Property</span></span>|<span data-ttu-id="d6e57-132">类型</span><span class="sxs-lookup"><span data-stu-id="d6e57-132">Type</span></span>|<span data-ttu-id="d6e57-133">说明</span><span class="sxs-lookup"><span data-stu-id="d6e57-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e57-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d6e57-134">appliesTo</span></span>|<span data-ttu-id="d6e57-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="d6e57-135">policyScope</span></span>|<span data-ttu-id="d6e57-136">确定此策略设置应用于的组。</span><span class="sxs-lookup"><span data-stu-id="d6e57-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="d6e57-137">可能的值是 `none` `all` `selected` **：、、重要：** `selected` 指定此属性时不能使用。</span><span class="sxs-lookup"><span data-stu-id="d6e57-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="d6e57-138">使用 [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) 添加特定组。</span><span class="sxs-lookup"><span data-stu-id="d6e57-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) to add specific groups.</span></span> <span data-ttu-id="d6e57-139">使用 `all` 将删除任何现有组。</span><span class="sxs-lookup"><span data-stu-id="d6e57-139">Using `all` will remove any existing groups.</span></span>|
|<span data-ttu-id="d6e57-140">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="d6e57-140">complianceUrl</span></span>|<span data-ttu-id="d6e57-141">String</span><span class="sxs-lookup"><span data-stu-id="d6e57-141">String</span></span>|<span data-ttu-id="d6e57-142">移动管理应用程序的合规性 URL</span><span class="sxs-lookup"><span data-stu-id="d6e57-142">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="d6e57-143">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="d6e57-143">discoveryUrl</span></span>|<span data-ttu-id="d6e57-144">String</span><span class="sxs-lookup"><span data-stu-id="d6e57-144">String</span></span>|<span data-ttu-id="d6e57-145">移动管理应用程序的发现 URL</span><span class="sxs-lookup"><span data-stu-id="d6e57-145">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="d6e57-146">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="d6e57-146">termsOfUseUrl</span></span>|<span data-ttu-id="d6e57-147">String</span><span class="sxs-lookup"><span data-stu-id="d6e57-147">String</span></span>|<span data-ttu-id="d6e57-148">移动管理应用程序的使用条款 URL</span><span class="sxs-lookup"><span data-stu-id="d6e57-148">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="d6e57-149">响应</span><span class="sxs-lookup"><span data-stu-id="d6e57-149">Response</span></span>

<span data-ttu-id="d6e57-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6e57-150">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6e57-151">示例</span><span class="sxs-lookup"><span data-stu-id="d6e57-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6e57-152">请求</span><span class="sxs-lookup"><span data-stu-id="d6e57-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d6e57-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e57-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```
# <a name="c"></a>[<span data-ttu-id="d6e57-154">C#</span><span class="sxs-lookup"><span data-stu-id="d6e57-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6e57-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6e57-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6e57-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6e57-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6e57-157">Java</span><span class="sxs-lookup"><span data-stu-id="d6e57-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6e57-158">响应</span><span class="sxs-lookup"><span data-stu-id="d6e57-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
