---
title: 更新 itemInsights
description: 更新 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9678cf4b389c4e0794fecd1616d9055dd2c9941a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981716"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="d7ac2-103">更新 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="d7ac2-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="d7ac2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ac2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7ac2-105">更新指定的 [itemInsightsSettings](../resources/iteminsightssettings.md) 资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="d7ac2-106">若要了解如何为你的组织自定义项目见解隐私，请参阅 [自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d7ac2-107">权限</span><span class="sxs-lookup"><span data-stu-id="d7ac2-107">Permissions</span></span>

<span data-ttu-id="d7ac2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7ac2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7ac2-110">Permission type</span></span>      | <span data-ttu-id="d7ac2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7ac2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7ac2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7ac2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7ac2-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7ac2-113">User.ReadWrite</span></span> |
|<span data-ttu-id="d7ac2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7ac2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7ac2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-115">Not supported.</span></span>    |
|<span data-ttu-id="d7ac2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7ac2-116">Application</span></span> | <span data-ttu-id="d7ac2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-117">Not supported.</span></span> |

><span data-ttu-id="d7ac2-118">**注意：** 对此操作使用委派权限时，需要已登录用户拥有全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="d7ac2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7ac2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="d7ac2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7ac2-120">Request headers</span></span>

| <span data-ttu-id="d7ac2-121">标头</span><span class="sxs-lookup"><span data-stu-id="d7ac2-121">Header</span></span>       | <span data-ttu-id="d7ac2-122">值</span><span class="sxs-lookup"><span data-stu-id="d7ac2-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d7ac2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7ac2-123">Authorization</span></span>  | <span data-ttu-id="d7ac2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7ac2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7ac2-126">Content-Type</span></span>  | <span data-ttu-id="d7ac2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d7ac2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7ac2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7ac2-128">Request body</span></span>

<span data-ttu-id="d7ac2-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7ac2-132">属性</span><span class="sxs-lookup"><span data-stu-id="d7ac2-132">Property</span></span>     | <span data-ttu-id="d7ac2-133">类型</span><span class="sxs-lookup"><span data-stu-id="d7ac2-133">Type</span></span>   |<span data-ttu-id="d7ac2-134">说明</span><span class="sxs-lookup"><span data-stu-id="d7ac2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7ac2-135">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="d7ac2-135">isEnabledInOrganization</span></span>|<span data-ttu-id="d7ac2-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7ac2-136">Boolean</span></span>| <span data-ttu-id="d7ac2-137">`true` 如果启用了组织项目见解，则为 `false` 如果对不例外的所有用户禁用了组织项目见解。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="d7ac2-138">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-138">Default is `true`.</span></span> <span data-ttu-id="d7ac2-139">可选。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-139">Optional.</span></span>|
|<span data-ttu-id="d7ac2-140">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="d7ac2-140">disabledForGroup</span></span>|<span data-ttu-id="d7ac2-141">String</span><span class="sxs-lookup"><span data-stu-id="d7ac2-141">String</span></span>| <span data-ttu-id="d7ac2-142">Azure AD 组的 ID，其中成员的项目见解已禁用。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="d7ac2-143">默认值为 `empty`。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-143">Default is `empty`.</span></span> <span data-ttu-id="d7ac2-144">可选。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="d7ac2-145">响应</span><span class="sxs-lookup"><span data-stu-id="d7ac2-145">Response</span></span>

<span data-ttu-id="d7ac2-146">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [itemInsightsSettings](../resources/iteminsightssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="d7ac2-147">**注意：** 此操作将验证指定的 **itemInsightsSettings** 资源的属性值的有效性。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="d7ac2-148">如果设置了 **disabledForGroup** 属性，则此操作不检查是否存在相应的 Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="d7ac2-149">这意味着，如果您将 **disabledForGroup** 设置为不存在或随后删除的 Azure AD 组，则此操作将无法识别任何组成员身份并为任何特定用户禁用项目见解。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="d7ac2-150">如果将 **isEnabledInOrganization** 设置为 `true` ，该操作将为组织中的所有用户启用见解。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="d7ac2-151">示例</span><span class="sxs-lookup"><span data-stu-id="d7ac2-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="d7ac2-152">请求</span><span class="sxs-lookup"><span data-stu-id="d7ac2-152">Request</span></span>

<span data-ttu-id="d7ac2-153">以下是有关管理员更新 " **disabledForGroup** " 隐私设置以禁止显示用户的特定 Azure AD 组的项目见解的示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-153">Here is an example request on how admin updates " **disabledForGroup** " privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7ac2-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7ac2-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="d7ac2-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7ac2-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d7ac2-156">C#</span><span class="sxs-lookup"><span data-stu-id="d7ac2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7ac2-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7ac2-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7ac2-158">Java</span><span class="sxs-lookup"><span data-stu-id="d7ac2-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7ac2-159">响应</span><span class="sxs-lookup"><span data-stu-id="d7ac2-159">Response</span></span>

<span data-ttu-id="d7ac2-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7ac2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


