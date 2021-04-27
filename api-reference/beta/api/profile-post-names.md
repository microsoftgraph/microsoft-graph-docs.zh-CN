---
title: 创建 personName
description: 使用此 API 在用户配置文件中创建新的 personName。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f29c138fbf2a0dfe374111bfa6f9d2511f5e62b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036882"
---
# <a name="create-personname"></a><span data-ttu-id="1886a-103">创建 personName</span><span class="sxs-lookup"><span data-stu-id="1886a-103">Create personName</span></span>

<span data-ttu-id="1886a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1886a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1886a-105">使用此 API 在用户配置文件中创建新的 [personName](../resources/personname.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="1886a-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1886a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1886a-106">Permissions</span></span>

<span data-ttu-id="1886a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1886a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1886a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1886a-109">Permission type</span></span>                        | <span data-ttu-id="1886a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1886a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1886a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1886a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1886a-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1886a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1886a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1886a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1886a-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1886a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1886a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1886a-115">Application</span></span>                            | <span data-ttu-id="1886a-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1886a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1886a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1886a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="1886a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1886a-118">Request headers</span></span>

| <span data-ttu-id="1886a-119">名称</span><span class="sxs-lookup"><span data-stu-id="1886a-119">Name</span></span>           |<span data-ttu-id="1886a-120">说明</span><span class="sxs-lookup"><span data-stu-id="1886a-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1886a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1886a-121">Authorization</span></span>  | <span data-ttu-id="1886a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1886a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1886a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1886a-124">Content-Type</span></span>   | <span data-ttu-id="1886a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1886a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1886a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1886a-127">Request body</span></span>
<span data-ttu-id="1886a-128">在请求正文中，提供 [personName](../resources/personname.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1886a-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="1886a-129">下表显示创建 [personName](../resources/personname.md) 对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="1886a-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="1886a-130">属性</span><span class="sxs-lookup"><span data-stu-id="1886a-130">Property</span></span>|<span data-ttu-id="1886a-131">类型</span><span class="sxs-lookup"><span data-stu-id="1886a-131">Type</span></span>|<span data-ttu-id="1886a-132">说明</span><span class="sxs-lookup"><span data-stu-id="1886a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1886a-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1886a-133">allowedAudiences</span></span>|<span data-ttu-id="1886a-134">String</span><span class="sxs-lookup"><span data-stu-id="1886a-134">String</span></span>|<span data-ttu-id="1886a-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="1886a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1886a-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="1886a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1886a-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1886a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1886a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1886a-138">displayName</span></span>|<span data-ttu-id="1886a-139">String</span><span class="sxs-lookup"><span data-stu-id="1886a-139">String</span></span>|<span data-ttu-id="1886a-140">根据用户或设备区域设置提供 firstName 和 lastName 的有序呈现。</span><span class="sxs-lookup"><span data-stu-id="1886a-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="1886a-141">first</span><span class="sxs-lookup"><span data-stu-id="1886a-141">first</span></span>|<span data-ttu-id="1886a-142">String</span><span class="sxs-lookup"><span data-stu-id="1886a-142">String</span></span>|<span data-ttu-id="1886a-143">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="1886a-143">First name of the user.</span></span>|
|<span data-ttu-id="1886a-144">id</span><span class="sxs-lookup"><span data-stu-id="1886a-144">id</span></span>|<span data-ttu-id="1886a-145">String</span><span class="sxs-lookup"><span data-stu-id="1886a-145">String</span></span>|<span data-ttu-id="1886a-146">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="1886a-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="1886a-147">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="1886a-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="1886a-148">inference</span><span class="sxs-lookup"><span data-stu-id="1886a-148">inference</span></span>|[<span data-ttu-id="1886a-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1886a-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1886a-150">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="1886a-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1886a-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="1886a-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1886a-152">initials</span><span class="sxs-lookup"><span data-stu-id="1886a-152">initials</span></span>|<span data-ttu-id="1886a-153">String</span><span class="sxs-lookup"><span data-stu-id="1886a-153">String</span></span>|<span data-ttu-id="1886a-154">用户缩写。</span><span class="sxs-lookup"><span data-stu-id="1886a-154">Initials of the user.</span></span>|
|<span data-ttu-id="1886a-155">languageTag</span><span class="sxs-lookup"><span data-stu-id="1886a-155">languageTag</span></span>|<span data-ttu-id="1886a-156">String</span><span class="sxs-lookup"><span data-stu-id="1886a-156">String</span></span>|<span data-ttu-id="1886a-157">包含以下 IETF BCP47 (en-US、no-NB、en-AU) 语言的名称。</span><span class="sxs-lookup"><span data-stu-id="1886a-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="1886a-158">last</span><span class="sxs-lookup"><span data-stu-id="1886a-158">last</span></span>|<span data-ttu-id="1886a-159">String</span><span class="sxs-lookup"><span data-stu-id="1886a-159">String</span></span>|<span data-ttu-id="1886a-160">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="1886a-160">Last name of the user.</span></span>|
|<span data-ttu-id="1886a-161">一些</span><span class="sxs-lookup"><span data-stu-id="1886a-161">maiden</span></span>|<span data-ttu-id="1886a-162">String</span><span class="sxs-lookup"><span data-stu-id="1886a-162">String</span></span>|<span data-ttu-id="1886a-163">用户的姓名。</span><span class="sxs-lookup"><span data-stu-id="1886a-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="1886a-164">middle</span><span class="sxs-lookup"><span data-stu-id="1886a-164">middle</span></span>|<span data-ttu-id="1886a-165">String</span><span class="sxs-lookup"><span data-stu-id="1886a-165">String</span></span>|<span data-ttu-id="1886a-166">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="1886a-166">Middle name of the user.</span></span>|
|<span data-ttu-id="1886a-167">nickname</span><span class="sxs-lookup"><span data-stu-id="1886a-167">nickname</span></span>|<span data-ttu-id="1886a-168">String</span><span class="sxs-lookup"><span data-stu-id="1886a-168">String</span></span>|<span data-ttu-id="1886a-169">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="1886a-169">Nickname of the user.</span></span>|
|<span data-ttu-id="1886a-170">pronunciation</span><span class="sxs-lookup"><span data-stu-id="1886a-170">pronunciation</span></span>|[<span data-ttu-id="1886a-171">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="1886a-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="1886a-172">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="1886a-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="1886a-173">后缀</span><span class="sxs-lookup"><span data-stu-id="1886a-173">suffix</span></span>|<span data-ttu-id="1886a-174">String</span><span class="sxs-lookup"><span data-stu-id="1886a-174">String</span></span>|<span data-ttu-id="1886a-175">用户名名称后使用 (，例如：PhD.) </span><span class="sxs-lookup"><span data-stu-id="1886a-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="1886a-176">title</span><span class="sxs-lookup"><span data-stu-id="1886a-176">title</span></span>|<span data-ttu-id="1886a-177">String</span><span class="sxs-lookup"><span data-stu-id="1886a-177">String</span></span>|<span data-ttu-id="1886a-178">用于为用户名称添加前缀的 (例如：Dr、Sir、Sir、Mrs.) </span><span class="sxs-lookup"><span data-stu-id="1886a-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="1886a-179">响应</span><span class="sxs-lookup"><span data-stu-id="1886a-179">Response</span></span>

<span data-ttu-id="1886a-180">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和新 [personName](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1886a-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1886a-181">示例</span><span class="sxs-lookup"><span data-stu-id="1886a-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1886a-182">请求</span><span class="sxs-lookup"><span data-stu-id="1886a-182">Request</span></span>

<span data-ttu-id="1886a-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1886a-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1886a-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="1886a-184">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null
}
```
# <a name="c"></a>[<span data-ttu-id="1886a-185">C#</span><span class="sxs-lookup"><span data-stu-id="1886a-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1886a-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1886a-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1886a-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1886a-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1886a-188">Java</span><span class="sxs-lookup"><span data-stu-id="1886a-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personname-from-profilev2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1886a-189">响应</span><span class="sxs-lookup"><span data-stu-id="1886a-189">Response</span></span>

<span data-ttu-id="1886a-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1886a-190">The following is an example of the response.</span></span>

> <span data-ttu-id="1886a-191">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1886a-191">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
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
  "nickname": null,
  "suffix": null,
  "title": null,
  "pronunciation": null
}
```


