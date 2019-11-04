---
title: 更新 userAccountInformation
description: 更新 userAccountInformation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78d890a00916c72b8c48e5b41a1c84e1e2e2ffb8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938139"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="f4863-103">更新 useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="f4863-103">Update useraccountinformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4863-104">更新用户的[配置文件](../resources/profile.md)中的[userAccountInformation](../resources/useraccountinformation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4863-104">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4863-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4863-105">Permissions</span></span>

<span data-ttu-id="f4863-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4863-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4863-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4863-108">Permission type</span></span>                        | <span data-ttu-id="f4863-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4863-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4863-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4863-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4863-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="f4863-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f4863-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4863-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4863-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="f4863-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f4863-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4863-114">Application</span></span>                            | <span data-ttu-id="f4863-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4863-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f4863-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4863-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4863-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4863-117">Request headers</span></span>

| <span data-ttu-id="f4863-118">名称</span><span class="sxs-lookup"><span data-stu-id="f4863-118">Name</span></span>           |<span data-ttu-id="f4863-119">说明</span><span class="sxs-lookup"><span data-stu-id="f4863-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="f4863-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4863-120">Authorization</span></span>  | <span data-ttu-id="f4863-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4863-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f4863-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4863-123">Content-Type</span></span>   | <span data-ttu-id="f4863-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="f4863-124">application/json.</span></span> <span data-ttu-id="f4863-125">必需</span><span class="sxs-lookup"><span data-stu-id="f4863-125">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4863-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4863-126">Request body</span></span>

<span data-ttu-id="f4863-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f4863-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4863-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f4863-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f4863-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f4863-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f4863-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4863-130">Property</span></span>            | <span data-ttu-id="f4863-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4863-131">Type</span></span>                                    | <span data-ttu-id="f4863-132">描述</span><span class="sxs-lookup"><span data-stu-id="f4863-132">Description</span></span>                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="f4863-133">ageGroup</span><span class="sxs-lookup"><span data-stu-id="f4863-133">ageGroup</span></span>             |<span data-ttu-id="f4863-134">String</span><span class="sxs-lookup"><span data-stu-id="f4863-134">String</span></span>                                   |<span data-ttu-id="f4863-135">显示用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="f4863-135">Shows the age group of user.</span></span> <span data-ttu-id="f4863-136">允许的`null`值`minor`、 `notAdult`和`adult`。</span><span class="sxs-lookup"><span data-stu-id="f4863-136">Allowed values `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="f4863-137">只读。</span><span class="sxs-lookup"><span data-stu-id="f4863-137">Read Only.</span></span> |
|<span data-ttu-id="f4863-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="f4863-138">countryCode</span></span>          |<span data-ttu-id="f4863-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f4863-139">String</span></span>                                   |<span data-ttu-id="f4863-140">包含与用户帐户关联的双字符 countryCode。</span><span class="sxs-lookup"><span data-stu-id="f4863-140">Contains the two-character countryCode associated with the users account.</span></span>                       |
|<span data-ttu-id="f4863-141">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="f4863-141">preferredLanguageTag</span></span> |[<span data-ttu-id="f4863-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f4863-142">localeInfo</span></span>](../resources/localeinfo.md) |<span data-ttu-id="f4863-143">包含用户与帐户相关的首选语言。</span><span class="sxs-lookup"><span data-stu-id="f4863-143">Contains the language the user has associated as preferred for the account.</span></span>                     |
|<span data-ttu-id="f4863-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4863-144">userPrincipalName</span></span>    |<span data-ttu-id="f4863-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f4863-145">String</span></span>                                   |<span data-ttu-id="f4863-146">与帐户关联的用户的用户主体名称（UPN）。</span><span class="sxs-lookup"><span data-stu-id="f4863-146">The user principal name (UPN) of the user associated with the account.</span></span>                          |

## <a name="response"></a><span data-ttu-id="f4863-147">响应</span><span class="sxs-lookup"><span data-stu-id="f4863-147">Response</span></span>

<span data-ttu-id="f4863-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userAccountInformation](../resources/useraccountinformation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4863-148">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4863-149">示例</span><span class="sxs-lookup"><span data-stu-id="f4863-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4863-150">请求</span><span class="sxs-lookup"><span data-stu-id="f4863-150">Request</span></span>

<span data-ttu-id="f4863-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4863-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

### <a name="response"></a><span data-ttu-id="f4863-152">响应</span><span class="sxs-lookup"><span data-stu-id="f4863-152">Response</span></span>

<span data-ttu-id="f4863-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4863-153">The following is an example of the response.</span></span>

> <span data-ttu-id="f4863-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f4863-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update useraccountinformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
