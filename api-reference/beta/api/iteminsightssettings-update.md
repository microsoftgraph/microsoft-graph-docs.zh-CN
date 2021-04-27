---
title: 更新 itemInsights
description: 更新 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0eb17d9e0a4f3285858800f32e6954bbd344dc27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053032"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="6d228-103">更新 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="6d228-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="6d228-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d228-105">更新指定 [itemInsightsSettings 资源](../resources/iteminsightssettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6d228-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="6d228-106">若要了解如何为组织自定义项目见解隐私，请参阅 [自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="6d228-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6d228-107">权限</span><span class="sxs-lookup"><span data-stu-id="6d228-107">Permissions</span></span>

<span data-ttu-id="6d228-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d228-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d228-110">Permission type</span></span>      | <span data-ttu-id="6d228-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d228-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d228-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d228-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d228-113">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d228-113">User.ReadWrite.All</span></span> |
|<span data-ttu-id="6d228-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d228-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d228-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d228-115">Not supported.</span></span>    |
|<span data-ttu-id="6d228-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d228-116">Application</span></span> | <span data-ttu-id="6d228-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d228-117">Not supported.</span></span> |

><span data-ttu-id="6d228-118">**注意：** 对此操作使用委派权限要求登录用户拥有全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6d228-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d228-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d228-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="6d228-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d228-120">Request headers</span></span>

| <span data-ttu-id="6d228-121">标头</span><span class="sxs-lookup"><span data-stu-id="6d228-121">Header</span></span>       | <span data-ttu-id="6d228-122">值</span><span class="sxs-lookup"><span data-stu-id="6d228-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6d228-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d228-123">Authorization</span></span>  | <span data-ttu-id="6d228-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d228-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d228-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d228-126">Content-Type</span></span>  | <span data-ttu-id="6d228-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6d228-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d228-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d228-128">Request body</span></span>

<span data-ttu-id="6d228-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6d228-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d228-132">属性</span><span class="sxs-lookup"><span data-stu-id="6d228-132">Property</span></span>     | <span data-ttu-id="6d228-133">类型</span><span class="sxs-lookup"><span data-stu-id="6d228-133">Type</span></span>   |<span data-ttu-id="6d228-134">说明</span><span class="sxs-lookup"><span data-stu-id="6d228-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d228-135">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="6d228-135">isEnabledInOrganization</span></span>|<span data-ttu-id="6d228-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="6d228-136">Boolean</span></span>| <span data-ttu-id="6d228-137">`true` 如果已启用组织项目见解; `false` 如果为所有用户禁用组织项目见解，则无例外。</span><span class="sxs-lookup"><span data-stu-id="6d228-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="6d228-138">默认值为“`true`”。</span><span class="sxs-lookup"><span data-stu-id="6d228-138">Default is `true`.</span></span> <span data-ttu-id="6d228-139">可选。</span><span class="sxs-lookup"><span data-stu-id="6d228-139">Optional.</span></span>|
|<span data-ttu-id="6d228-140">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="6d228-140">disabledForGroup</span></span>|<span data-ttu-id="6d228-141">String</span><span class="sxs-lookup"><span data-stu-id="6d228-141">String</span></span>| <span data-ttu-id="6d228-142">已禁用成员的项见解的 Azure AD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="6d228-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="6d228-143">默认值为“`empty`”。</span><span class="sxs-lookup"><span data-stu-id="6d228-143">Default is `empty`.</span></span> <span data-ttu-id="6d228-144">可选。</span><span class="sxs-lookup"><span data-stu-id="6d228-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="6d228-145">响应</span><span class="sxs-lookup"><span data-stu-id="6d228-145">Response</span></span>

<span data-ttu-id="6d228-146">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [itemInsightsSettings](../resources/iteminsightssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d228-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="6d228-147">**注意：** 此操作验证指定 **itemInsightsSettings** 资源的属性值的有效性。</span><span class="sxs-lookup"><span data-stu-id="6d228-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="6d228-148">如果 **设置了 disabledForGroup** 属性，则此操作不会检查是否存在相应的 Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="6d228-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="6d228-149">这意味着，如果将 **disabledForGroup** 设置为不存在或之后已删除的 Azure AD 组，则此操作将无法识别任何组成员身份，并禁用对特定用户的项目见解。</span><span class="sxs-lookup"><span data-stu-id="6d228-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="6d228-150">如果 **isEnabledInOrganization** 设置为 ，则操作将为组织中所有用户 `true` 启用见解。</span><span class="sxs-lookup"><span data-stu-id="6d228-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="6d228-151">示例</span><span class="sxs-lookup"><span data-stu-id="6d228-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="6d228-152">请求</span><span class="sxs-lookup"><span data-stu-id="6d228-152">Request</span></span>

<span data-ttu-id="6d228-153">下面是管理员如何更新 **"disabledForGroup"** 隐私设置以禁止显示用户对特定 Azure AD 组的项目见解的示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d228-153">Here is an example request on how admin updates "**disabledForGroup**" privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d228-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d228-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6d228-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d228-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6d228-156">C#</span><span class="sxs-lookup"><span data-stu-id="6d228-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d228-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d228-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d228-158">Java</span><span class="sxs-lookup"><span data-stu-id="6d228-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d228-159">响应</span><span class="sxs-lookup"><span data-stu-id="6d228-159">Response</span></span>

<span data-ttu-id="6d228-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6d228-160">Here is an example of the response.</span></span> <span data-ttu-id="6d228-161">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6d228-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


