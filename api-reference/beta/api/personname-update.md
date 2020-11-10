---
title: 更新 Contact.personname
description: 更新 Contact.personname 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 540ce931e77b5f9347015fe5792c7c2e0f5486f8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972724"
---
# <a name="update-personname"></a><span data-ttu-id="2836a-103">更新 contact.personname</span><span class="sxs-lookup"><span data-stu-id="2836a-103">Update personname</span></span>

<span data-ttu-id="2836a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2836a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2836a-105">更新用户的[配置文件](../resources/profile.md)中的[contact.personname](../resources/personname.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2836a-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2836a-106">权限</span><span class="sxs-lookup"><span data-stu-id="2836a-106">Permissions</span></span>

<span data-ttu-id="2836a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2836a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2836a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2836a-109">Permission type</span></span>                        | <span data-ttu-id="2836a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2836a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2836a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2836a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2836a-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2836a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2836a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2836a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2836a-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2836a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2836a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2836a-115">Application</span></span>                            | <span data-ttu-id="2836a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2836a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="2836a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2836a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2836a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2836a-118">Request headers</span></span>

| <span data-ttu-id="2836a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2836a-119">Name</span></span>           |<span data-ttu-id="2836a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2836a-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2836a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2836a-121">Authorization</span></span>  | <span data-ttu-id="2836a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2836a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2836a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2836a-124">Content-Type</span></span>   | <span data-ttu-id="2836a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2836a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2836a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2836a-127">Request body</span></span>

<span data-ttu-id="2836a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2836a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2836a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2836a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2836a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2836a-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="2836a-131">下表显示了可以在用户[配置文件](../resources/profile.md)中的现有[contact.personname](../resources/personname.md)对象内进行更新的属性。</span><span class="sxs-lookup"><span data-stu-id="2836a-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="2836a-132">属性</span><span class="sxs-lookup"><span data-stu-id="2836a-132">Property</span></span>|<span data-ttu-id="2836a-133">类型</span><span class="sxs-lookup"><span data-stu-id="2836a-133">Type</span></span>|<span data-ttu-id="2836a-134">说明</span><span class="sxs-lookup"><span data-stu-id="2836a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2836a-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="2836a-135">allowedAudiences</span></span>|<span data-ttu-id="2836a-136">String</span><span class="sxs-lookup"><span data-stu-id="2836a-136">String</span></span>|<span data-ttu-id="2836a-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="2836a-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="2836a-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="2836a-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="2836a-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2836a-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2836a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2836a-140">displayName</span></span>|<span data-ttu-id="2836a-141">String</span><span class="sxs-lookup"><span data-stu-id="2836a-141">String</span></span>|<span data-ttu-id="2836a-142">根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="2836a-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="2836a-143">前</span><span class="sxs-lookup"><span data-stu-id="2836a-143">first</span></span>|<span data-ttu-id="2836a-144">String</span><span class="sxs-lookup"><span data-stu-id="2836a-144">String</span></span>|<span data-ttu-id="2836a-145">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="2836a-145">First name of the user.</span></span>|
|<span data-ttu-id="2836a-146">推导</span><span class="sxs-lookup"><span data-stu-id="2836a-146">inference</span></span>|[<span data-ttu-id="2836a-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="2836a-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="2836a-148">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="2836a-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="2836a-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="2836a-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="2836a-150">initials</span><span class="sxs-lookup"><span data-stu-id="2836a-150">initials</span></span>|<span data-ttu-id="2836a-151">String</span><span class="sxs-lookup"><span data-stu-id="2836a-151">String</span></span>|<span data-ttu-id="2836a-152">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="2836a-152">Initials of the user.</span></span>|
|<span data-ttu-id="2836a-153">languageTag</span><span class="sxs-lookup"><span data-stu-id="2836a-153">languageTag</span></span>|<span data-ttu-id="2836a-154">String</span><span class="sxs-lookup"><span data-stu-id="2836a-154">String</span></span>|<span data-ttu-id="2836a-155">包含以下语言的名称： (en-us、无 NB、en-us) 以下 IETF BCP47 格式。</span><span class="sxs-lookup"><span data-stu-id="2836a-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="2836a-156">末</span><span class="sxs-lookup"><span data-stu-id="2836a-156">last</span></span>|<span data-ttu-id="2836a-157">String</span><span class="sxs-lookup"><span data-stu-id="2836a-157">String</span></span>|<span data-ttu-id="2836a-158">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="2836a-158">Last name of the user.</span></span>|
|<span data-ttu-id="2836a-159">maiden</span><span class="sxs-lookup"><span data-stu-id="2836a-159">maiden</span></span>|<span data-ttu-id="2836a-160">String</span><span class="sxs-lookup"><span data-stu-id="2836a-160">String</span></span>|<span data-ttu-id="2836a-161">Maiden 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="2836a-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="2836a-162">中间</span><span class="sxs-lookup"><span data-stu-id="2836a-162">middle</span></span>|<span data-ttu-id="2836a-163">String</span><span class="sxs-lookup"><span data-stu-id="2836a-163">String</span></span>|<span data-ttu-id="2836a-164">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="2836a-164">Middle name of the user.</span></span>|
|<span data-ttu-id="2836a-165">昵称</span><span class="sxs-lookup"><span data-stu-id="2836a-165">nickname</span></span>|<span data-ttu-id="2836a-166">String</span><span class="sxs-lookup"><span data-stu-id="2836a-166">String</span></span>|<span data-ttu-id="2836a-167">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="2836a-167">Nickname of the user.</span></span>|
|<span data-ttu-id="2836a-168">拼音</span><span class="sxs-lookup"><span data-stu-id="2836a-168">pronunciation</span></span>|[<span data-ttu-id="2836a-169">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="2836a-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="2836a-170">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="2836a-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="2836a-171">后缀</span><span class="sxs-lookup"><span data-stu-id="2836a-171">suffix</span></span>|<span data-ttu-id="2836a-172">String</span><span class="sxs-lookup"><span data-stu-id="2836a-172">String</span></span>|<span data-ttu-id="2836a-173">用户名称之后使用的指示符 (例如：博士. ) </span><span class="sxs-lookup"><span data-stu-id="2836a-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="2836a-174">title</span><span class="sxs-lookup"><span data-stu-id="2836a-174">title</span></span>|<span data-ttu-id="2836a-175">String</span><span class="sxs-lookup"><span data-stu-id="2836a-175">String</span></span>|<span data-ttu-id="2836a-176">Honorifics 用于为用户名称加上前缀 (例如： Dr.、罗德、Madam、Mrs ) </span><span class="sxs-lookup"><span data-stu-id="2836a-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="2836a-177">响应</span><span class="sxs-lookup"><span data-stu-id="2836a-177">Response</span></span>

<span data-ttu-id="2836a-178">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [contact.personname](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2836a-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2836a-179">示例</span><span class="sxs-lookup"><span data-stu-id="2836a-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2836a-180">请求</span><span class="sxs-lookup"><span data-stu-id="2836a-180">Request</span></span>

<span data-ttu-id="2836a-181">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2836a-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2836a-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="2836a-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2836a-183">C#</span><span class="sxs-lookup"><span data-stu-id="2836a-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2836a-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2836a-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2836a-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2836a-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2836a-186">Java</span><span class="sxs-lookup"><span data-stu-id="2836a-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2836a-187">响应</span><span class="sxs-lookup"><span data-stu-id="2836a-187">Response</span></span>

<span data-ttu-id="2836a-188">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2836a-188">The following is an example of the response.</span></span>

> <span data-ttu-id="2836a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2836a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


