---
title: 更新 languageProficiency
description: 更新用户的配置文件中的 languageProficiency 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6d85263db9d54565613678d4941594e5df312d57
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998242"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="1316f-103">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="1316f-103">Update languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1316f-104">更新用户的[配置文件](../resources/profile.md)中的[languageProficiency](../resources/languageproficiency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1316f-104">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1316f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1316f-105">Permissions</span></span>

<span data-ttu-id="1316f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1316f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1316f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1316f-108">Permission type</span></span>                        | <span data-ttu-id="1316f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1316f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1316f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1316f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1316f-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1316f-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1316f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1316f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1316f-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1316f-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1316f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1316f-114">Application</span></span>                            | <span data-ttu-id="1316f-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1316f-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1316f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1316f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1316f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1316f-117">Request headers</span></span>

| <span data-ttu-id="1316f-118">名称</span><span class="sxs-lookup"><span data-stu-id="1316f-118">Name</span></span>           |<span data-ttu-id="1316f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1316f-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1316f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1316f-120">Authorization</span></span>  | <span data-ttu-id="1316f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1316f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1316f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1316f-123">Content-Type</span></span>   | <span data-ttu-id="1316f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1316f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1316f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1316f-126">Request body</span></span>

<span data-ttu-id="1316f-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="1316f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1316f-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="1316f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1316f-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1316f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1316f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1316f-130">Property</span></span>     | <span data-ttu-id="1316f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1316f-131">Type</span></span>        | <span data-ttu-id="1316f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1316f-132">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1316f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1316f-133">displayName</span></span>   |<span data-ttu-id="1316f-134">String</span><span class="sxs-lookup"><span data-stu-id="1316f-134">String</span></span>       | <span data-ttu-id="1316f-135">包含所述语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="1316f-135">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="1316f-136">水平</span><span class="sxs-lookup"><span data-stu-id="1316f-136">proficiency</span></span>   |<span data-ttu-id="1316f-137">string</span><span class="sxs-lookup"><span data-stu-id="1316f-137">string</span></span>       | <span data-ttu-id="1316f-138">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1316f-138">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1316f-139">tag</span><span class="sxs-lookup"><span data-stu-id="1316f-139">tag</span></span>           |<span data-ttu-id="1316f-140">String</span><span class="sxs-lookup"><span data-stu-id="1316f-140">String</span></span>       | <span data-ttu-id="1316f-141">包含4个字符 BCP47 语言的名称（en-us，无 NB，en-us）</span><span class="sxs-lookup"><span data-stu-id="1316f-141">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="1316f-142">响应</span><span class="sxs-lookup"><span data-stu-id="1316f-142">Response</span></span>

<span data-ttu-id="1316f-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[languageProficiency](../resources/languageproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1316f-143">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1316f-144">示例</span><span class="sxs-lookup"><span data-stu-id="1316f-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1316f-145">请求</span><span class="sxs-lookup"><span data-stu-id="1316f-145">Request</span></span>

<span data-ttu-id="1316f-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1316f-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1316f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1316f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1316f-148">C#</span><span class="sxs-lookup"><span data-stu-id="1316f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1316f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1316f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1316f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1316f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1316f-151">响应</span><span class="sxs-lookup"><span data-stu-id="1316f-151">Response</span></span>

<span data-ttu-id="1316f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1316f-152">The following is an example of the response.</span></span>

> <span data-ttu-id="1316f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1316f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update languageproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
