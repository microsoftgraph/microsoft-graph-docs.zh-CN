---
title: 更新 Contact.personname
description: 更新 Contact.personname 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 26989c4eb5b7af987ab9a50555d3abdf07e3a16a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228690"
---
# <a name="update-personname"></a><span data-ttu-id="a0769-103">更新 contact.personname</span><span class="sxs-lookup"><span data-stu-id="a0769-103">Update personname</span></span>

<span data-ttu-id="a0769-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0769-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0769-105">更新用户的[配置文件](../resources/profile.md)中的[contact.personname](../resources/personname.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a0769-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0769-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0769-106">Permissions</span></span>

<span data-ttu-id="a0769-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0769-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0769-109">Permission type</span></span>                        | <span data-ttu-id="a0769-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0769-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0769-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0769-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0769-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a0769-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a0769-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0769-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0769-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a0769-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a0769-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0769-115">Application</span></span>                            | <span data-ttu-id="a0769-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0769-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a0769-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0769-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a0769-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0769-118">Request headers</span></span>

| <span data-ttu-id="a0769-119">名称</span><span class="sxs-lookup"><span data-stu-id="a0769-119">Name</span></span>           |<span data-ttu-id="a0769-120">说明</span><span class="sxs-lookup"><span data-stu-id="a0769-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a0769-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0769-121">Authorization</span></span>  | <span data-ttu-id="a0769-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0769-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a0769-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0769-124">Content-Type</span></span>   | <span data-ttu-id="a0769-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a0769-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0769-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0769-127">Request body</span></span>

<span data-ttu-id="a0769-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a0769-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a0769-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a0769-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a0769-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a0769-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0769-131">属性</span><span class="sxs-lookup"><span data-stu-id="a0769-131">Property</span></span>     | <span data-ttu-id="a0769-132">类型</span><span class="sxs-lookup"><span data-stu-id="a0769-132">Type</span></span>                                            | <span data-ttu-id="a0769-133">说明</span><span class="sxs-lookup"><span data-stu-id="a0769-133">Description</span></span>                                                                             |
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="a0769-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a0769-134">displayName</span></span>   |<span data-ttu-id="a0769-135">String</span><span class="sxs-lookup"><span data-stu-id="a0769-135">String</span></span>                                           | <span data-ttu-id="a0769-136">提供名和姓的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="a0769-136">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="a0769-137">前</span><span class="sxs-lookup"><span data-stu-id="a0769-137">first</span></span>         |<span data-ttu-id="a0769-138">String</span><span class="sxs-lookup"><span data-stu-id="a0769-138">String</span></span>                                           | <span data-ttu-id="a0769-139">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="a0769-139">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="a0769-140">initials</span><span class="sxs-lookup"><span data-stu-id="a0769-140">initials</span></span>      |<span data-ttu-id="a0769-141">String</span><span class="sxs-lookup"><span data-stu-id="a0769-141">String</span></span>                                           | <span data-ttu-id="a0769-142">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="a0769-142">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="a0769-143">languageTag</span><span class="sxs-lookup"><span data-stu-id="a0769-143">languageTag</span></span>   |<span data-ttu-id="a0769-144">String</span><span class="sxs-lookup"><span data-stu-id="a0769-144">String</span></span>                                           | <span data-ttu-id="a0769-145">包含遵循 IETF BCP47 格式的语言（en-us，无 NB，en-us）的名称。</span><span class="sxs-lookup"><span data-stu-id="a0769-145">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="a0769-146">末</span><span class="sxs-lookup"><span data-stu-id="a0769-146">last</span></span>          |<span data-ttu-id="a0769-147">String</span><span class="sxs-lookup"><span data-stu-id="a0769-147">String</span></span>                                           | <span data-ttu-id="a0769-148">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="a0769-148">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="a0769-149">maiden</span><span class="sxs-lookup"><span data-stu-id="a0769-149">maiden</span></span>        |<span data-ttu-id="a0769-150">String</span><span class="sxs-lookup"><span data-stu-id="a0769-150">String</span></span>                                           | <span data-ttu-id="a0769-151">用户的预 marriage 姓。</span><span class="sxs-lookup"><span data-stu-id="a0769-151">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="a0769-152">中间</span><span class="sxs-lookup"><span data-stu-id="a0769-152">middle</span></span>        |<span data-ttu-id="a0769-153">String</span><span class="sxs-lookup"><span data-stu-id="a0769-153">String</span></span>                                           | <span data-ttu-id="a0769-154">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="a0769-154">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="a0769-155">昵称</span><span class="sxs-lookup"><span data-stu-id="a0769-155">nickname</span></span>      |<span data-ttu-id="a0769-156">String</span><span class="sxs-lookup"><span data-stu-id="a0769-156">String</span></span>                                           | <span data-ttu-id="a0769-157">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="a0769-157">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="a0769-158">拼音</span><span class="sxs-lookup"><span data-stu-id="a0769-158">pronunciation</span></span> |[<span data-ttu-id="a0769-159">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="a0769-159">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="a0769-160">包含有关用户姓名的读音的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0769-160">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="a0769-161">后缀</span><span class="sxs-lookup"><span data-stu-id="a0769-161">suffix</span></span>        |<span data-ttu-id="a0769-162">String</span><span class="sxs-lookup"><span data-stu-id="a0769-162">String</span></span>                                           | <span data-ttu-id="a0769-163">在 users 名称之后使用的指示符。</span><span class="sxs-lookup"><span data-stu-id="a0769-163">Designators used after the users name.</span></span> <span data-ttu-id="a0769-164">（例如： PhD.）</span><span class="sxs-lookup"><span data-stu-id="a0769-164">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="a0769-165">title</span><span class="sxs-lookup"><span data-stu-id="a0769-165">title</span></span>         |<span data-ttu-id="a0769-166">字符串</span><span class="sxs-lookup"><span data-stu-id="a0769-166">String</span></span>                                           | <span data-ttu-id="a0769-167">Honorifics 用于为用户名称加前缀。</span><span class="sxs-lookup"><span data-stu-id="a0769-167">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="a0769-168">（例如： Dr.、罗德、Madam、Mrs）</span><span class="sxs-lookup"><span data-stu-id="a0769-168">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="a0769-169">响应</span><span class="sxs-lookup"><span data-stu-id="a0769-169">Response</span></span>

<span data-ttu-id="a0769-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0769-170">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0769-171">示例</span><span class="sxs-lookup"><span data-stu-id="a0769-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0769-172">请求</span><span class="sxs-lookup"><span data-stu-id="a0769-172">Request</span></span>

<span data-ttu-id="a0769-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0769-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0769-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0769-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a0769-175">C#</span><span class="sxs-lookup"><span data-stu-id="a0769-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0769-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0769-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0769-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0769-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a0769-178">响应</span><span class="sxs-lookup"><span data-stu-id="a0769-178">Response</span></span>

<span data-ttu-id="a0769-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0769-179">The following is an example of the response.</span></span>

> <span data-ttu-id="a0769-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0769-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personname",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
