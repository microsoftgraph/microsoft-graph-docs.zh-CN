---
title: 更新 userInsightsSettings
description: 更新 userInsightsSettings 对象的属性。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: a422a106d1371e8e39fdfa314658b8e77d0f5a9a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210657"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="d2c19-103">更新 userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="d2c19-103">Update userInsightsSettings</span></span>

<span data-ttu-id="d2c19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2c19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2c19-105">更新用户 [itemInsights](../resources/iteminsights.md) 和 [会议时间见解](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="d2c19-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2c19-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2c19-106">Permissions</span></span>

<span data-ttu-id="d2c19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2c19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c19-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2c19-109">Permission type</span></span>      | <span data-ttu-id="d2c19-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2c19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2c19-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2c19-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2c19-112">User.ReadWrite</span></span> |
|<span data-ttu-id="d2c19-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2c19-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2c19-114">Not supported.</span></span>    |
|<span data-ttu-id="d2c19-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2c19-115">Application</span></span> | <span data-ttu-id="d2c19-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2c19-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d2c19-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2c19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="d2c19-118">**注意：** 具有 或 的请求仅可供用户或具有 `userId` `userPrincipalName` User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="d2c19-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="d2c19-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2c19-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2c19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2c19-120">Request headers</span></span>

| <span data-ttu-id="d2c19-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2c19-121">Header</span></span>       | <span data-ttu-id="d2c19-122">值</span><span class="sxs-lookup"><span data-stu-id="d2c19-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d2c19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2c19-123">Authorization</span></span>  | <span data-ttu-id="d2c19-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2c19-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2c19-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2c19-126">Content-Type</span></span>  | <span data-ttu-id="d2c19-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d2c19-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2c19-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2c19-129">Request body</span></span>

<span data-ttu-id="d2c19-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d2c19-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2c19-133">属性</span><span class="sxs-lookup"><span data-stu-id="d2c19-133">Property</span></span>     | <span data-ttu-id="d2c19-134">类型</span><span class="sxs-lookup"><span data-stu-id="d2c19-134">Type</span></span>   |<span data-ttu-id="d2c19-135">说明</span><span class="sxs-lookup"><span data-stu-id="d2c19-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2c19-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d2c19-136">isEnabled</span></span>|<span data-ttu-id="d2c19-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2c19-137">Boolean</span></span>| <span data-ttu-id="d2c19-138">`true` 如果用户的 **itemInsights** 和会议时间见解已启用; `false` 如果禁用了 **用户的 itemInsights** 和会议小时数见解。</span><span class="sxs-lookup"><span data-stu-id="d2c19-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="d2c19-139">默认值为“`true`”。</span><span class="sxs-lookup"><span data-stu-id="d2c19-139">Default is `true`.</span></span> <span data-ttu-id="d2c19-140">可选。</span><span class="sxs-lookup"><span data-stu-id="d2c19-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="d2c19-141">响应</span><span class="sxs-lookup"><span data-stu-id="d2c19-141">Response</span></span>

<span data-ttu-id="d2c19-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userInsightsSettings](../resources/userinsightssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2c19-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2c19-143">示例</span><span class="sxs-lookup"><span data-stu-id="d2c19-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="d2c19-144">请求</span><span class="sxs-lookup"><span data-stu-id="d2c19-144">Request</span></span>

<span data-ttu-id="d2c19-145">下面是有关用户如何更新"**isEnabled"** 隐私设置以禁用其项目见解和会议时间见解的示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2c19-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2c19-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2c19-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userInsightsSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{userId}/settings/itemInsights
Content-type: application/json

{
  "isEnabled": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="d2c19-147">C#</span><span class="sxs-lookup"><span data-stu-id="d2c19-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2c19-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2c19-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2c19-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2c19-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2c19-150">Java</span><span class="sxs-lookup"><span data-stu-id="d2c19-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d2c19-151">响应</span><span class="sxs-lookup"><span data-stu-id="d2c19-151">Response</span></span>

<span data-ttu-id="d2c19-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2c19-152">The following is an example of the response.</span></span> 

><span data-ttu-id="d2c19-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d2c19-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "update_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": false,
}
```
