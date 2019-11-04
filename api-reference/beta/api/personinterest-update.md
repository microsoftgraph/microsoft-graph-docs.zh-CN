---
title: 更新 personInterest
description: 更新 personinterest 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2c328000a775c6dc97fc74c454a21b6699acb390
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937880"
---
# <a name="update-personinterest"></a><span data-ttu-id="94408-103">更新 personinterest</span><span class="sxs-lookup"><span data-stu-id="94408-103">Update personinterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94408-104">更新用户的[配置文件](../resources/profile.md)中的[personInterest](../resources/personinterest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94408-104">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94408-105">权限</span><span class="sxs-lookup"><span data-stu-id="94408-105">Permissions</span></span>

<span data-ttu-id="94408-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94408-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94408-108">Permission type</span></span>                        | <span data-ttu-id="94408-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94408-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94408-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94408-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94408-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="94408-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94408-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94408-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94408-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="94408-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94408-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94408-114">Application</span></span>                            | <span data-ttu-id="94408-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94408-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="94408-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94408-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94408-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="94408-117">Request headers</span></span>

| <span data-ttu-id="94408-118">名称</span><span class="sxs-lookup"><span data-stu-id="94408-118">Name</span></span>           |<span data-ttu-id="94408-119">说明</span><span class="sxs-lookup"><span data-stu-id="94408-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="94408-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94408-120">Authorization</span></span>  | <span data-ttu-id="94408-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94408-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="94408-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94408-123">Content-Type</span></span>   | <span data-ttu-id="94408-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="94408-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94408-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94408-126">Request body</span></span>

<span data-ttu-id="94408-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="94408-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="94408-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="94408-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="94408-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="94408-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94408-130">属性</span><span class="sxs-lookup"><span data-stu-id="94408-130">Property</span></span>     | <span data-ttu-id="94408-131">类型</span><span class="sxs-lookup"><span data-stu-id="94408-131">Type</span></span>             | <span data-ttu-id="94408-132">描述</span><span class="sxs-lookup"><span data-stu-id="94408-132">Description</span></span>                                                                         |
|:-------------|:-----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="94408-133">类别</span><span class="sxs-lookup"><span data-stu-id="94408-133">categories</span></span>    |<span data-ttu-id="94408-134">String collection</span><span class="sxs-lookup"><span data-stu-id="94408-134">String collection</span></span> | <span data-ttu-id="94408-135">包含用户与兴趣相关联的类别（例如： personal、recipies）</span><span class="sxs-lookup"><span data-stu-id="94408-135">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span>|
|<span data-ttu-id="94408-136">description</span><span class="sxs-lookup"><span data-stu-id="94408-136">description</span></span>   |<span data-ttu-id="94408-137">字符串</span><span class="sxs-lookup"><span data-stu-id="94408-137">String</span></span>            | <span data-ttu-id="94408-138">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="94408-138">Contains a description of the interest.</span></span>                                             |
|<span data-ttu-id="94408-139">displayName</span><span class="sxs-lookup"><span data-stu-id="94408-139">displayName</span></span>   |<span data-ttu-id="94408-140">String</span><span class="sxs-lookup"><span data-stu-id="94408-140">String</span></span>            | <span data-ttu-id="94408-141">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="94408-141">Contains a friendly name for the interest.</span></span>                                          |
|<span data-ttu-id="94408-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="94408-142">webUrl</span></span>        |<span data-ttu-id="94408-143">String</span><span class="sxs-lookup"><span data-stu-id="94408-143">String</span></span>            | <span data-ttu-id="94408-144">包含指向有关该兴趣的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="94408-144">Contains a link to an information source about the interest.</span></span>                        |

## <a name="response"></a><span data-ttu-id="94408-145">响应</span><span class="sxs-lookup"><span data-stu-id="94408-145">Response</span></span>

<span data-ttu-id="94408-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[personInterest](../resources/personinterest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94408-146">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94408-147">示例</span><span class="sxs-lookup"><span data-stu-id="94408-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94408-148">请求</span><span class="sxs-lookup"><span data-stu-id="94408-148">Request</span></span>

<span data-ttu-id="94408-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94408-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="94408-150">响应</span><span class="sxs-lookup"><span data-stu-id="94408-150">Response</span></span>

<span data-ttu-id="94408-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94408-151">The following is an example of the response.</span></span>

> <span data-ttu-id="94408-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94408-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personinterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->