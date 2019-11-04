---
title: 更新 languageProficiency
description: 更新用户的配置文件中的 languageProficiency 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a1b19bced8e76d94cfdeb51725a7e67314890449
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938420"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="94f77-103">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="94f77-103">Update languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94f77-104">更新用户的[配置文件](../resources/profile.md)中的[languageProficiency](../resources/languageproficiency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94f77-104">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94f77-105">权限</span><span class="sxs-lookup"><span data-stu-id="94f77-105">Permissions</span></span>

<span data-ttu-id="94f77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94f77-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94f77-108">Permission type</span></span>                        | <span data-ttu-id="94f77-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94f77-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94f77-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94f77-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94f77-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="94f77-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94f77-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94f77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94f77-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="94f77-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94f77-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94f77-114">Application</span></span>                            | <span data-ttu-id="94f77-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f77-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="94f77-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94f77-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94f77-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="94f77-117">Request headers</span></span>

| <span data-ttu-id="94f77-118">名称</span><span class="sxs-lookup"><span data-stu-id="94f77-118">Name</span></span>           |<span data-ttu-id="94f77-119">说明</span><span class="sxs-lookup"><span data-stu-id="94f77-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="94f77-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f77-120">Authorization</span></span>  | <span data-ttu-id="94f77-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94f77-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="94f77-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94f77-123">Content-Type</span></span>   | <span data-ttu-id="94f77-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="94f77-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94f77-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94f77-126">Request body</span></span>

<span data-ttu-id="94f77-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="94f77-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="94f77-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="94f77-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="94f77-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="94f77-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94f77-130">属性</span><span class="sxs-lookup"><span data-stu-id="94f77-130">Property</span></span>     | <span data-ttu-id="94f77-131">类型</span><span class="sxs-lookup"><span data-stu-id="94f77-131">Type</span></span>        | <span data-ttu-id="94f77-132">描述</span><span class="sxs-lookup"><span data-stu-id="94f77-132">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="94f77-133">displayName</span><span class="sxs-lookup"><span data-stu-id="94f77-133">displayName</span></span>   |<span data-ttu-id="94f77-134">String</span><span class="sxs-lookup"><span data-stu-id="94f77-134">String</span></span>       | <span data-ttu-id="94f77-135">包含所述语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="94f77-135">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="94f77-136">水平</span><span class="sxs-lookup"><span data-stu-id="94f77-136">proficiency</span></span>   |<span data-ttu-id="94f77-137">string</span><span class="sxs-lookup"><span data-stu-id="94f77-137">string</span></span>       | <span data-ttu-id="94f77-138">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="94f77-138">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="94f77-139">tag</span><span class="sxs-lookup"><span data-stu-id="94f77-139">tag</span></span>           |<span data-ttu-id="94f77-140">字符串</span><span class="sxs-lookup"><span data-stu-id="94f77-140">String</span></span>       | <span data-ttu-id="94f77-141">包含4个字符 BCP47 语言的名称（en-us，无 NB，en-us）</span><span class="sxs-lookup"><span data-stu-id="94f77-141">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="94f77-142">响应</span><span class="sxs-lookup"><span data-stu-id="94f77-142">Response</span></span>

<span data-ttu-id="94f77-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[languageProficiency](../resources/languageproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94f77-143">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94f77-144">示例</span><span class="sxs-lookup"><span data-stu-id="94f77-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94f77-145">请求</span><span class="sxs-lookup"><span data-stu-id="94f77-145">Request</span></span>

<span data-ttu-id="94f77-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94f77-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94f77-147">响应</span><span class="sxs-lookup"><span data-stu-id="94f77-147">Response</span></span>

<span data-ttu-id="94f77-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94f77-148">The following is an example of the response.</span></span>

> <span data-ttu-id="94f77-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94f77-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
