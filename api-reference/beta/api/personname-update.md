---
title: 更新 personName
description: 更新 personName 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0959c7eec1b1e52ff3a9295ad7e5af07b416a3bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051100"
---
# <a name="update-personname"></a><span data-ttu-id="402f9-103">更新 personname</span><span class="sxs-lookup"><span data-stu-id="402f9-103">Update personname</span></span>

<span data-ttu-id="402f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="402f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="402f9-105">更新用户配置文件 [中的 personName](../resources/personname.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="402f9-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="402f9-106">权限</span><span class="sxs-lookup"><span data-stu-id="402f9-106">Permissions</span></span>

<span data-ttu-id="402f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="402f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="402f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="402f9-109">Permission type</span></span>                        | <span data-ttu-id="402f9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="402f9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="402f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="402f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="402f9-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402f9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="402f9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="402f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="402f9-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402f9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="402f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="402f9-115">Application</span></span>                            | <span data-ttu-id="402f9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402f9-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="402f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="402f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="402f9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="402f9-118">Request headers</span></span>

| <span data-ttu-id="402f9-119">名称</span><span class="sxs-lookup"><span data-stu-id="402f9-119">Name</span></span>           |<span data-ttu-id="402f9-120">说明</span><span class="sxs-lookup"><span data-stu-id="402f9-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="402f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="402f9-121">Authorization</span></span>  | <span data-ttu-id="402f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="402f9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="402f9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="402f9-124">Content-Type</span></span>   | <span data-ttu-id="402f9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="402f9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="402f9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="402f9-127">Request body</span></span>

<span data-ttu-id="402f9-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="402f9-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="402f9-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="402f9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="402f9-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="402f9-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="402f9-131">下表显示了在用户配置文件中的现有 [personName](../resources/personname.md) 对象中可以更新 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="402f9-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="402f9-132">属性</span><span class="sxs-lookup"><span data-stu-id="402f9-132">Property</span></span>|<span data-ttu-id="402f9-133">类型</span><span class="sxs-lookup"><span data-stu-id="402f9-133">Type</span></span>|<span data-ttu-id="402f9-134">说明</span><span class="sxs-lookup"><span data-stu-id="402f9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="402f9-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="402f9-135">allowedAudiences</span></span>|<span data-ttu-id="402f9-136">String</span><span class="sxs-lookup"><span data-stu-id="402f9-136">String</span></span>|<span data-ttu-id="402f9-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="402f9-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="402f9-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="402f9-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="402f9-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="402f9-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="402f9-140">displayName</span><span class="sxs-lookup"><span data-stu-id="402f9-140">displayName</span></span>|<span data-ttu-id="402f9-141">String</span><span class="sxs-lookup"><span data-stu-id="402f9-141">String</span></span>|<span data-ttu-id="402f9-142">根据用户或设备区域设置提供 firstName 和 lastName 的有序呈现。</span><span class="sxs-lookup"><span data-stu-id="402f9-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="402f9-143">first</span><span class="sxs-lookup"><span data-stu-id="402f9-143">first</span></span>|<span data-ttu-id="402f9-144">String</span><span class="sxs-lookup"><span data-stu-id="402f9-144">String</span></span>|<span data-ttu-id="402f9-145">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="402f9-145">First name of the user.</span></span>|
|<span data-ttu-id="402f9-146">inference</span><span class="sxs-lookup"><span data-stu-id="402f9-146">inference</span></span>|[<span data-ttu-id="402f9-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="402f9-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="402f9-148">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="402f9-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="402f9-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="402f9-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="402f9-150">initials</span><span class="sxs-lookup"><span data-stu-id="402f9-150">initials</span></span>|<span data-ttu-id="402f9-151">String</span><span class="sxs-lookup"><span data-stu-id="402f9-151">String</span></span>|<span data-ttu-id="402f9-152">用户缩写。</span><span class="sxs-lookup"><span data-stu-id="402f9-152">Initials of the user.</span></span>|
|<span data-ttu-id="402f9-153">languageTag</span><span class="sxs-lookup"><span data-stu-id="402f9-153">languageTag</span></span>|<span data-ttu-id="402f9-154">String</span><span class="sxs-lookup"><span data-stu-id="402f9-154">String</span></span>|<span data-ttu-id="402f9-155">包含以下 IETF BCP47 (en-US、no-NB、en-AU) 语言的名称。</span><span class="sxs-lookup"><span data-stu-id="402f9-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="402f9-156">last</span><span class="sxs-lookup"><span data-stu-id="402f9-156">last</span></span>|<span data-ttu-id="402f9-157">String</span><span class="sxs-lookup"><span data-stu-id="402f9-157">String</span></span>|<span data-ttu-id="402f9-158">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="402f9-158">Last name of the user.</span></span>|
|<span data-ttu-id="402f9-159">一些</span><span class="sxs-lookup"><span data-stu-id="402f9-159">maiden</span></span>|<span data-ttu-id="402f9-160">String</span><span class="sxs-lookup"><span data-stu-id="402f9-160">String</span></span>|<span data-ttu-id="402f9-161">用户的姓名。</span><span class="sxs-lookup"><span data-stu-id="402f9-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="402f9-162">middle</span><span class="sxs-lookup"><span data-stu-id="402f9-162">middle</span></span>|<span data-ttu-id="402f9-163">String</span><span class="sxs-lookup"><span data-stu-id="402f9-163">String</span></span>|<span data-ttu-id="402f9-164">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="402f9-164">Middle name of the user.</span></span>|
|<span data-ttu-id="402f9-165">nickname</span><span class="sxs-lookup"><span data-stu-id="402f9-165">nickname</span></span>|<span data-ttu-id="402f9-166">String</span><span class="sxs-lookup"><span data-stu-id="402f9-166">String</span></span>|<span data-ttu-id="402f9-167">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="402f9-167">Nickname of the user.</span></span>|
|<span data-ttu-id="402f9-168">pronunciation</span><span class="sxs-lookup"><span data-stu-id="402f9-168">pronunciation</span></span>|[<span data-ttu-id="402f9-169">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="402f9-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="402f9-170">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="402f9-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="402f9-171">后缀</span><span class="sxs-lookup"><span data-stu-id="402f9-171">suffix</span></span>|<span data-ttu-id="402f9-172">String</span><span class="sxs-lookup"><span data-stu-id="402f9-172">String</span></span>|<span data-ttu-id="402f9-173">用户名名称后使用 (，例如：PhD.) </span><span class="sxs-lookup"><span data-stu-id="402f9-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="402f9-174">title</span><span class="sxs-lookup"><span data-stu-id="402f9-174">title</span></span>|<span data-ttu-id="402f9-175">String</span><span class="sxs-lookup"><span data-stu-id="402f9-175">String</span></span>|<span data-ttu-id="402f9-176">用于为用户名称添加前缀的 (例如：Dr、Sir、Sir、Mrs.) </span><span class="sxs-lookup"><span data-stu-id="402f9-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="402f9-177">响应</span><span class="sxs-lookup"><span data-stu-id="402f9-177">Response</span></span>

<span data-ttu-id="402f9-178">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [personName](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="402f9-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="402f9-179">示例</span><span class="sxs-lookup"><span data-stu-id="402f9-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="402f9-180">请求</span><span class="sxs-lookup"><span data-stu-id="402f9-180">Request</span></span>

<span data-ttu-id="402f9-181">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="402f9-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="402f9-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="402f9-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "nickname": "Kesha"
}

```
# <a name="c"></a>[<span data-ttu-id="402f9-183">C#</span><span class="sxs-lookup"><span data-stu-id="402f9-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="402f9-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="402f9-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="402f9-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="402f9-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="402f9-186">Java</span><span class="sxs-lookup"><span data-stu-id="402f9-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="402f9-187">响应</span><span class="sxs-lookup"><span data-stu-id="402f9-187">Response</span></span>

<span data-ttu-id="402f9-188">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="402f9-188">The following is an example of the response.</span></span>

> <span data-ttu-id="402f9-189">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="402f9-189">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
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
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "displayName": "In-no ken-te ",
    "first": "In-no ken-te Pop-ov",
    "maiden": null,
    "middle": null,
    "last": "Pop-ov"
  }
}
```


