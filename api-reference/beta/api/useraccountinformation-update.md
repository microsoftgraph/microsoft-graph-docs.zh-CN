---
title: 更新 userAccountInformation
description: 更新 userAccountInformation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: af2081afcf12d2cac33abf188ad6592e5e4720e1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049581"
---
# <a name="update-useraccountinformation"></a><span data-ttu-id="f6c2d-103">更新 useraccountinformation</span><span class="sxs-lookup"><span data-stu-id="f6c2d-103">Update useraccountinformation</span></span>

<span data-ttu-id="f6c2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c2d-105">更新用户配置文件 [中的 userAccountInformation](../resources/useraccountinformation.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-105">Update the properties of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c2d-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6c2d-106">Permissions</span></span>

<span data-ttu-id="f6c2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6c2d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c2d-109">Permission type</span></span>                        | <span data-ttu-id="f6c2d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6c2d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f6c2d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c2d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6c2d-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c2d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f6c2d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c2d-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c2d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f6c2d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c2d-115">Application</span></span>                            | <span data-ttu-id="f6c2d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c2d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f6c2d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c2d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
PATCH /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6c2d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c2d-118">Request headers</span></span>

| <span data-ttu-id="f6c2d-119">名称</span><span class="sxs-lookup"><span data-stu-id="f6c2d-119">Name</span></span>           |<span data-ttu-id="f6c2d-120">说明</span><span class="sxs-lookup"><span data-stu-id="f6c2d-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="f6c2d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c2d-121">Authorization</span></span>  | <span data-ttu-id="f6c2d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6c2d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6c2d-124">Content-Type</span></span>   | <span data-ttu-id="f6c2d-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="f6c2d-125">application/json.</span></span> <span data-ttu-id="f6c2d-126">必需</span><span class="sxs-lookup"><span data-stu-id="f6c2d-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6c2d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c2d-127">Request body</span></span>

<span data-ttu-id="f6c2d-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f6c2d-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f6c2d-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="f6c2d-131">属性</span><span class="sxs-lookup"><span data-stu-id="f6c2d-131">Property</span></span>|<span data-ttu-id="f6c2d-132">类型</span><span class="sxs-lookup"><span data-stu-id="f6c2d-132">Type</span></span>|<span data-ttu-id="f6c2d-133">说明</span><span class="sxs-lookup"><span data-stu-id="f6c2d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c2d-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="f6c2d-134">allowedAudiences</span></span>|<span data-ttu-id="f6c2d-135">String</span><span class="sxs-lookup"><span data-stu-id="f6c2d-135">String</span></span>|<span data-ttu-id="f6c2d-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f6c2d-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f6c2d-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f6c2d-139">countryCode</span><span class="sxs-lookup"><span data-stu-id="f6c2d-139">countryCode</span></span>|<span data-ttu-id="f6c2d-140">String</span><span class="sxs-lookup"><span data-stu-id="f6c2d-140">String</span></span>|<span data-ttu-id="f6c2d-141">包含与用户帐户关联的两个字符的国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-141">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="f6c2d-142">inference</span><span class="sxs-lookup"><span data-stu-id="f6c2d-142">inference</span></span>|[<span data-ttu-id="f6c2d-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="f6c2d-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f6c2d-144">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f6c2d-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f6c2d-146">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="f6c2d-146">preferredLanguageTag</span></span>|[<span data-ttu-id="f6c2d-147">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f6c2d-147">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="f6c2d-148">包含用户关联为帐户首选的语言。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-148">Contains the language the user has associated as preferred for the account.</span></span>   |

## <a name="response"></a><span data-ttu-id="f6c2d-149">响应</span><span class="sxs-lookup"><span data-stu-id="f6c2d-149">Response</span></span>

<span data-ttu-id="f6c2d-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userAccountInformation](../resources/useraccountinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-150">If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6c2d-151">示例</span><span class="sxs-lookup"><span data-stu-id="f6c2d-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6c2d-152">请求</span><span class="sxs-lookup"><span data-stu-id="f6c2d-152">Request</span></span>

<span data-ttu-id="f6c2d-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6c2d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c2d-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "countryCode": "NO"
}
```
# <a name="c"></a>[<span data-ttu-id="f6c2d-155">C#</span><span class="sxs-lookup"><span data-stu-id="f6c2d-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6c2d-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c2d-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6c2d-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c2d-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6c2d-158">Java</span><span class="sxs-lookup"><span data-stu-id="f6c2d-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6c2d-159">响应</span><span class="sxs-lookup"><span data-stu-id="f6c2d-159">Response</span></span>

<span data-ttu-id="f6c2d-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-160">The following is an example of the response.</span></span>

> <span data-ttu-id="f6c2d-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f6c2d-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


