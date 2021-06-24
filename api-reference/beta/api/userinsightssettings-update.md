---
title: 更新 userInsightsSettings
description: 更新 userInsightsSettings 对象的属性。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5f161d5b75e862f358d07fee2347bb3f4d18bbad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107823"
---
# <a name="update-userinsightssettings"></a><span data-ttu-id="7127c-103">更新 userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7127c-103">Update userInsightsSettings</span></span>

<span data-ttu-id="7127c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7127c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7127c-105">更新用户 [itemInsights](../resources/iteminsights.md) 和 [会议时间见解](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="7127c-105">Update the privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7127c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7127c-106">Permissions</span></span>

<span data-ttu-id="7127c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7127c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7127c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7127c-109">Permission type</span></span>      | <span data-ttu-id="7127c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7127c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7127c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7127c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7127c-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7127c-112">User.ReadWrite</span></span> |
|<span data-ttu-id="7127c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7127c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7127c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7127c-114">Not supported.</span></span>    |
|<span data-ttu-id="7127c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7127c-115">Application</span></span> | <span data-ttu-id="7127c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7127c-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="7127c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7127c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

><span data-ttu-id="7127c-118">**注意：** 具有 或 的请求仅可供用户或具有 `userId` `userPrincipalName` User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="7127c-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="7127c-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7127c-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7127c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7127c-120">Request headers</span></span>

| <span data-ttu-id="7127c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7127c-121">Header</span></span>       | <span data-ttu-id="7127c-122">值</span><span class="sxs-lookup"><span data-stu-id="7127c-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7127c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7127c-123">Authorization</span></span>  | <span data-ttu-id="7127c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7127c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7127c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7127c-126">Content-Type</span></span>  | <span data-ttu-id="7127c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7127c-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7127c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7127c-129">Request body</span></span>

<span data-ttu-id="7127c-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7127c-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7127c-133">属性</span><span class="sxs-lookup"><span data-stu-id="7127c-133">Property</span></span>     | <span data-ttu-id="7127c-134">类型</span><span class="sxs-lookup"><span data-stu-id="7127c-134">Type</span></span>   |<span data-ttu-id="7127c-135">说明</span><span class="sxs-lookup"><span data-stu-id="7127c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7127c-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7127c-136">isEnabled</span></span>|<span data-ttu-id="7127c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7127c-137">Boolean</span></span>| <span data-ttu-id="7127c-138">`true` 如果用户的 **itemInsights** 和会议时间见解已启用; `false` 如果禁用了 **用户的 itemInsights** 和会议小时数见解。</span><span class="sxs-lookup"><span data-stu-id="7127c-138">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="7127c-139">默认值为“`true`”。</span><span class="sxs-lookup"><span data-stu-id="7127c-139">Default is `true`.</span></span> <span data-ttu-id="7127c-140">可选。</span><span class="sxs-lookup"><span data-stu-id="7127c-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="7127c-141">响应</span><span class="sxs-lookup"><span data-stu-id="7127c-141">Response</span></span>

<span data-ttu-id="7127c-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userInsightsSettings](../resources/userinsightssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7127c-142">If successful, this method returns a `200 OK` response code and [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7127c-143">示例</span><span class="sxs-lookup"><span data-stu-id="7127c-143">Example</span></span> 

### <a name="request"></a><span data-ttu-id="7127c-144">请求</span><span class="sxs-lookup"><span data-stu-id="7127c-144">Request</span></span>

<span data-ttu-id="7127c-145">下面是有关用户如何更新"**isEnabled"** 隐私设置以禁用其项目见解和会议时间见解的示例请求。</span><span class="sxs-lookup"><span data-stu-id="7127c-145">The following is an example request on how user updates "**isEnabled**" privacy setting in order to disable his item insights and meeting hours insights.</span></span>

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


### <a name="response"></a><span data-ttu-id="7127c-146">响应</span><span class="sxs-lookup"><span data-stu-id="7127c-146">Response</span></span>

<span data-ttu-id="7127c-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7127c-147">The following is an example of the response.</span></span> 

><span data-ttu-id="7127c-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7127c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
