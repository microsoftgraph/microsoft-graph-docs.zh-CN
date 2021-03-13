---
title: 更新 personAnnotation
description: 更新 personAnnotation 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a86467b01d6072f4a14dad6fc5d1a6838249899b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774164"
---
# <a name="update-personannotation"></a><span data-ttu-id="12311-103">更新 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="12311-103">Update personAnnotation</span></span>
<span data-ttu-id="12311-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12311-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12311-105">更新用户配置文件 [中的 personAnnotation](../resources/personannotation.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="12311-105">Update the properties of a [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12311-106">权限</span><span class="sxs-lookup"><span data-stu-id="12311-106">Permissions</span></span>

<span data-ttu-id="12311-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12311-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12311-109">Permission type</span></span>                        | <span data-ttu-id="12311-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12311-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="12311-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12311-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12311-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12311-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12311-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12311-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12311-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12311-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12311-115">Application</span><span class="sxs-lookup"><span data-stu-id="12311-115">Application</span></span>                            | <span data-ttu-id="12311-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12311-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="12311-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12311-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/notes/{id}
PATCH /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="12311-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="12311-118">Request headers</span></span>
|<span data-ttu-id="12311-119">名称</span><span class="sxs-lookup"><span data-stu-id="12311-119">Name</span></span>|<span data-ttu-id="12311-120">说明</span><span class="sxs-lookup"><span data-stu-id="12311-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12311-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12311-121">Authorization</span></span>|<span data-ttu-id="12311-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12311-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12311-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12311-124">Content-Type</span></span>|<span data-ttu-id="12311-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="12311-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12311-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12311-127">Request body</span></span>

<span data-ttu-id="12311-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="12311-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="12311-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="12311-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="12311-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="12311-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="12311-131">下表显示了在用户配置文件中的现有 [personAnnotation](../resources/personannotation.md) 对象中可以更新 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="12311-131">The following table shows the properties that are possible to update within an existing [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="12311-132">属性</span><span class="sxs-lookup"><span data-stu-id="12311-132">Property</span></span>|<span data-ttu-id="12311-133">类型</span><span class="sxs-lookup"><span data-stu-id="12311-133">Type</span></span>|<span data-ttu-id="12311-134">说明</span><span class="sxs-lookup"><span data-stu-id="12311-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12311-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="12311-135">allowedAudiences</span></span>|<span data-ttu-id="12311-136">字符串</span><span class="sxs-lookup"><span data-stu-id="12311-136">String</span></span>|<span data-ttu-id="12311-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="12311-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="12311-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12311-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="12311-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="12311-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="12311-140">detail</span><span class="sxs-lookup"><span data-stu-id="12311-140">detail</span></span>|[<span data-ttu-id="12311-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="12311-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="12311-142">包含注释本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="12311-142">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="12311-143">displayName</span><span class="sxs-lookup"><span data-stu-id="12311-143">displayName</span></span>|<span data-ttu-id="12311-144">字符串</span><span class="sxs-lookup"><span data-stu-id="12311-144">String</span></span>|<span data-ttu-id="12311-145">包含便笺的友好名称。</span><span class="sxs-lookup"><span data-stu-id="12311-145">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="12311-146">inference</span><span class="sxs-lookup"><span data-stu-id="12311-146">inference</span></span>|[<span data-ttu-id="12311-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="12311-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="12311-148">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="12311-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="12311-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12311-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="12311-150">响应</span><span class="sxs-lookup"><span data-stu-id="12311-150">Response</span></span>

<span data-ttu-id="12311-151">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [personAnnotation](../resources/personannotation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12311-151">If successful, this method returns a `200 OK` response code and an updated [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12311-152">示例</span><span class="sxs-lookup"><span data-stu-id="12311-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12311-153">请求</span><span class="sxs-lookup"><span data-stu-id="12311-153">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="12311-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="12311-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personannotation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/notes/{id}
Content-Type: application/json
Content-length: 413

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="12311-155">C#</span><span class="sxs-lookup"><span data-stu-id="12311-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personannotation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12311-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12311-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personannotation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12311-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12311-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personannotation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12311-158">Java</span><span class="sxs-lookup"><span data-stu-id="12311-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personannotation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="12311-159">响应</span><span class="sxs-lookup"><span data-stu-id="12311-159">Response</span></span>
<span data-ttu-id="12311-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12311-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
    "@odata.type": "microsoft.graph.personAnnotation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow."
  },
  "displayName": "About Me"
}
```



