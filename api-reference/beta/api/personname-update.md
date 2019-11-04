---
title: 更新 Contact.personname
description: 更新 contact.personname 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 97a4497b88e7cb065ea5ad73229dc4acc8c45556
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937859"
---
# <a name="update-personname"></a><span data-ttu-id="001d1-103">更新 contact.personname</span><span class="sxs-lookup"><span data-stu-id="001d1-103">Update personname</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001d1-104">更新用户的[配置文件](../resources/profile.md)中的[contact.personname](../resources/personname.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="001d1-104">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="001d1-105">权限</span><span class="sxs-lookup"><span data-stu-id="001d1-105">Permissions</span></span>

<span data-ttu-id="001d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="001d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="001d1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="001d1-108">Permission type</span></span>                        | <span data-ttu-id="001d1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="001d1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="001d1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="001d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="001d1-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="001d1-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="001d1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="001d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="001d1-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="001d1-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="001d1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="001d1-114">Application</span></span>                            | <span data-ttu-id="001d1-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="001d1-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="001d1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="001d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="001d1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="001d1-117">Request headers</span></span>

| <span data-ttu-id="001d1-118">名称</span><span class="sxs-lookup"><span data-stu-id="001d1-118">Name</span></span>           |<span data-ttu-id="001d1-119">说明</span><span class="sxs-lookup"><span data-stu-id="001d1-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="001d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="001d1-120">Authorization</span></span>  | <span data-ttu-id="001d1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="001d1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="001d1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="001d1-123">Content-Type</span></span>   | <span data-ttu-id="001d1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="001d1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="001d1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="001d1-126">Request body</span></span>

<span data-ttu-id="001d1-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="001d1-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="001d1-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="001d1-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="001d1-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="001d1-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="001d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="001d1-130">Property</span></span>     | <span data-ttu-id="001d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="001d1-131">Type</span></span>                                            | <span data-ttu-id="001d1-132">描述</span><span class="sxs-lookup"><span data-stu-id="001d1-132">Description</span></span>                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="001d1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="001d1-133">displayName</span></span>   |<span data-ttu-id="001d1-134">String</span><span class="sxs-lookup"><span data-stu-id="001d1-134">String</span></span>                                           | <span data-ttu-id="001d1-135">提供名和姓的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="001d1-135">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="001d1-136">前</span><span class="sxs-lookup"><span data-stu-id="001d1-136">first</span></span>         |<span data-ttu-id="001d1-137">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-137">String</span></span>                                           | <span data-ttu-id="001d1-138">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="001d1-138">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="001d1-139">initials</span><span class="sxs-lookup"><span data-stu-id="001d1-139">initials</span></span>      |<span data-ttu-id="001d1-140">String</span><span class="sxs-lookup"><span data-stu-id="001d1-140">String</span></span>                                           | <span data-ttu-id="001d1-141">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="001d1-141">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="001d1-142">languageTag</span><span class="sxs-lookup"><span data-stu-id="001d1-142">languageTag</span></span>   |<span data-ttu-id="001d1-143">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-143">String</span></span>                                           | <span data-ttu-id="001d1-144">包含遵循 IETF BCP47 格式的语言（en-us，无 NB，en-us）的名称。</span><span class="sxs-lookup"><span data-stu-id="001d1-144">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="001d1-145">末</span><span class="sxs-lookup"><span data-stu-id="001d1-145">last</span></span>          |<span data-ttu-id="001d1-146">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-146">String</span></span>                                           | <span data-ttu-id="001d1-147">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="001d1-147">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="001d1-148">maiden</span><span class="sxs-lookup"><span data-stu-id="001d1-148">maiden</span></span>        |<span data-ttu-id="001d1-149">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-149">String</span></span>                                           | <span data-ttu-id="001d1-150">用户的预 marriage 姓。</span><span class="sxs-lookup"><span data-stu-id="001d1-150">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="001d1-151">中间</span><span class="sxs-lookup"><span data-stu-id="001d1-151">middle</span></span>        |<span data-ttu-id="001d1-152">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-152">String</span></span>                                           | <span data-ttu-id="001d1-153">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="001d1-153">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="001d1-154">昵称</span><span class="sxs-lookup"><span data-stu-id="001d1-154">nickname</span></span>      |<span data-ttu-id="001d1-155">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-155">String</span></span>                                           | <span data-ttu-id="001d1-156">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="001d1-156">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="001d1-157">拼音</span><span class="sxs-lookup"><span data-stu-id="001d1-157">pronunciation</span></span> |[<span data-ttu-id="001d1-158">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="001d1-158">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="001d1-159">包含有关用户姓名的读音的详细信息。</span><span class="sxs-lookup"><span data-stu-id="001d1-159">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="001d1-160">后缀</span><span class="sxs-lookup"><span data-stu-id="001d1-160">suffix</span></span>        |<span data-ttu-id="001d1-161">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-161">String</span></span>                                           | <span data-ttu-id="001d1-162">在 users 名称之后使用的指示符。</span><span class="sxs-lookup"><span data-stu-id="001d1-162">Designators used after the users name.</span></span> <span data-ttu-id="001d1-163">（例如： PhD.）</span><span class="sxs-lookup"><span data-stu-id="001d1-163">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="001d1-164">title</span><span class="sxs-lookup"><span data-stu-id="001d1-164">title</span></span>         |<span data-ttu-id="001d1-165">字符串</span><span class="sxs-lookup"><span data-stu-id="001d1-165">String</span></span>                                           | <span data-ttu-id="001d1-166">Honorifics 用于为用户名称加前缀。</span><span class="sxs-lookup"><span data-stu-id="001d1-166">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="001d1-167">（例如： Dr.、罗德、Madam、Mrs）</span><span class="sxs-lookup"><span data-stu-id="001d1-167">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="001d1-168">响应</span><span class="sxs-lookup"><span data-stu-id="001d1-168">Response</span></span>

<span data-ttu-id="001d1-169">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="001d1-169">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="001d1-170">示例</span><span class="sxs-lookup"><span data-stu-id="001d1-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="001d1-171">请求</span><span class="sxs-lookup"><span data-stu-id="001d1-171">Request</span></span>

<span data-ttu-id="001d1-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="001d1-172">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="001d1-173">响应</span><span class="sxs-lookup"><span data-stu-id="001d1-173">Response</span></span>

<span data-ttu-id="001d1-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="001d1-174">The following is an example of the response.</span></span>

> <span data-ttu-id="001d1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="001d1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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