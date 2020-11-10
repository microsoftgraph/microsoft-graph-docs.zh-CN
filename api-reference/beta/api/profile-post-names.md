---
title: 创建 Contact.personname
description: 使用此 API 在用户的配置文件中创建新的 Contact.personname。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b8cc9365132d102698edceb18c36838bfd8a3b2f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974755"
---
# <a name="create-personname"></a><span data-ttu-id="e9e8e-103">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="e9e8e-103">Create personName</span></span>

<span data-ttu-id="e9e8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e8e-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9e8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9e8e-106">Permissions</span></span>

<span data-ttu-id="e9e8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9e8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9e8e-109">Permission type</span></span>                        | <span data-ttu-id="e9e8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9e8e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e9e8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9e8e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9e8e-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e9e8e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e9e8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9e8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9e8e-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e9e8e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e9e8e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9e8e-115">Application</span></span>                            | <span data-ttu-id="e9e8e-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="e9e8e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9e8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9e8e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="e9e8e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9e8e-118">Request headers</span></span>

| <span data-ttu-id="e9e8e-119">名称</span><span class="sxs-lookup"><span data-stu-id="e9e8e-119">Name</span></span>           |<span data-ttu-id="e9e8e-120">说明</span><span class="sxs-lookup"><span data-stu-id="e9e8e-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e9e8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9e8e-121">Authorization</span></span>  | <span data-ttu-id="e9e8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e9e8e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9e8e-124">Content-Type</span></span>   | <span data-ttu-id="e9e8e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e9e8e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9e8e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9e8e-127">Request body</span></span>
<span data-ttu-id="e9e8e-128">在请求正文中，提供 [contact.personname](../resources/personname.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="e9e8e-129">下表显示了创建 [contact.personname](../resources/personname.md) 对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="e9e8e-130">属性</span><span class="sxs-lookup"><span data-stu-id="e9e8e-130">Property</span></span>|<span data-ttu-id="e9e8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9e8e-131">Type</span></span>|<span data-ttu-id="e9e8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9e8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9e8e-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e9e8e-133">allowedAudiences</span></span>|<span data-ttu-id="e9e8e-134">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-134">String</span></span>|<span data-ttu-id="e9e8e-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e9e8e-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e9e8e-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e9e8e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e9e8e-138">displayName</span></span>|<span data-ttu-id="e9e8e-139">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-139">String</span></span>|<span data-ttu-id="e9e8e-140">根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="e9e8e-141">前</span><span class="sxs-lookup"><span data-stu-id="e9e8e-141">first</span></span>|<span data-ttu-id="e9e8e-142">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-142">String</span></span>|<span data-ttu-id="e9e8e-143">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-143">First name of the user.</span></span>|
|<span data-ttu-id="e9e8e-144">id</span><span class="sxs-lookup"><span data-stu-id="e9e8e-144">id</span></span>|<span data-ttu-id="e9e8e-145">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-145">String</span></span>|<span data-ttu-id="e9e8e-146">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="e9e8e-147">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="e9e8e-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e9e8e-148">推导</span><span class="sxs-lookup"><span data-stu-id="e9e8e-148">inference</span></span>|[<span data-ttu-id="e9e8e-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e9e8e-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e9e8e-150">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e9e8e-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e9e8e-152">initials</span><span class="sxs-lookup"><span data-stu-id="e9e8e-152">initials</span></span>|<span data-ttu-id="e9e8e-153">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-153">String</span></span>|<span data-ttu-id="e9e8e-154">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-154">Initials of the user.</span></span>|
|<span data-ttu-id="e9e8e-155">languageTag</span><span class="sxs-lookup"><span data-stu-id="e9e8e-155">languageTag</span></span>|<span data-ttu-id="e9e8e-156">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-156">String</span></span>|<span data-ttu-id="e9e8e-157">包含以下语言的名称： (en-us、无 NB、en-us) 以下 IETF BCP47 格式。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="e9e8e-158">末</span><span class="sxs-lookup"><span data-stu-id="e9e8e-158">last</span></span>|<span data-ttu-id="e9e8e-159">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-159">String</span></span>|<span data-ttu-id="e9e8e-160">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-160">Last name of the user.</span></span>|
|<span data-ttu-id="e9e8e-161">maiden</span><span class="sxs-lookup"><span data-stu-id="e9e8e-161">maiden</span></span>|<span data-ttu-id="e9e8e-162">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-162">String</span></span>|<span data-ttu-id="e9e8e-163">Maiden 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="e9e8e-164">中间</span><span class="sxs-lookup"><span data-stu-id="e9e8e-164">middle</span></span>|<span data-ttu-id="e9e8e-165">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-165">String</span></span>|<span data-ttu-id="e9e8e-166">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-166">Middle name of the user.</span></span>|
|<span data-ttu-id="e9e8e-167">昵称</span><span class="sxs-lookup"><span data-stu-id="e9e8e-167">nickname</span></span>|<span data-ttu-id="e9e8e-168">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-168">String</span></span>|<span data-ttu-id="e9e8e-169">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-169">Nickname of the user.</span></span>|
|<span data-ttu-id="e9e8e-170">拼音</span><span class="sxs-lookup"><span data-stu-id="e9e8e-170">pronunciation</span></span>|[<span data-ttu-id="e9e8e-171">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="e9e8e-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="e9e8e-172">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="e9e8e-173">后缀</span><span class="sxs-lookup"><span data-stu-id="e9e8e-173">suffix</span></span>|<span data-ttu-id="e9e8e-174">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-174">String</span></span>|<span data-ttu-id="e9e8e-175">用户名称之后使用的指示符 (例如：博士. ) </span><span class="sxs-lookup"><span data-stu-id="e9e8e-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="e9e8e-176">title</span><span class="sxs-lookup"><span data-stu-id="e9e8e-176">title</span></span>|<span data-ttu-id="e9e8e-177">String</span><span class="sxs-lookup"><span data-stu-id="e9e8e-177">String</span></span>|<span data-ttu-id="e9e8e-178">Honorifics 用于为用户名称加上前缀 (例如： Dr.、罗德、Madam、Mrs ) </span><span class="sxs-lookup"><span data-stu-id="e9e8e-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="e9e8e-179">响应</span><span class="sxs-lookup"><span data-stu-id="e9e8e-179">Response</span></span>

<span data-ttu-id="e9e8e-180">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [contact.personname](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9e8e-181">示例</span><span class="sxs-lookup"><span data-stu-id="e9e8e-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9e8e-182">请求</span><span class="sxs-lookup"><span data-stu-id="e9e8e-182">Request</span></span>

<span data-ttu-id="e9e8e-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9e8e-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9e8e-184">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="e9e8e-185">C#</span><span class="sxs-lookup"><span data-stu-id="e9e8e-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9e8e-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9e8e-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9e8e-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9e8e-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9e8e-188">Java</span><span class="sxs-lookup"><span data-stu-id="e9e8e-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personname-from-profilev2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e9e8e-189">响应</span><span class="sxs-lookup"><span data-stu-id="e9e8e-189">Response</span></span>

<span data-ttu-id="e9e8e-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-190">The following is an example of the response.</span></span>

> <span data-ttu-id="e9e8e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e9e8e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


