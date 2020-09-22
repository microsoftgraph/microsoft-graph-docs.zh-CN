---
title: 更新 personInterest
description: 更新 personInterest 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 812a692a721e9d9a76cb7a0fa2547e48fb849e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067933"
---
# <a name="update-personinterest"></a><span data-ttu-id="32596-103">更新 personinterest</span><span class="sxs-lookup"><span data-stu-id="32596-103">Update personinterest</span></span>

<span data-ttu-id="32596-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32596-105">更新用户的[配置文件](../resources/profile.md)中的[personInterest](../resources/personinterest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32596-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32596-106">权限</span><span class="sxs-lookup"><span data-stu-id="32596-106">Permissions</span></span>

<span data-ttu-id="32596-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32596-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32596-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32596-109">Permission type</span></span>                        | <span data-ttu-id="32596-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32596-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="32596-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32596-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32596-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="32596-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="32596-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32596-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32596-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="32596-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="32596-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="32596-115">Application</span></span>                            | <span data-ttu-id="32596-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32596-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="32596-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32596-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
PATCH /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32596-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="32596-118">Request headers</span></span>

| <span data-ttu-id="32596-119">名称</span><span class="sxs-lookup"><span data-stu-id="32596-119">Name</span></span>           |<span data-ttu-id="32596-120">说明</span><span class="sxs-lookup"><span data-stu-id="32596-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="32596-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32596-121">Authorization</span></span>  | <span data-ttu-id="32596-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32596-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="32596-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32596-124">Content-Type</span></span>   | <span data-ttu-id="32596-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32596-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32596-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="32596-127">Request body</span></span>

<span data-ttu-id="32596-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="32596-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="32596-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="32596-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="32596-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="32596-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="32596-131">下表显示了可以在用户[配置文件](../resources/profile.md)中的现有[personInterest](../resources/personinterest.md)对象内进行更新的属性。</span><span class="sxs-lookup"><span data-stu-id="32596-131">The following table shows the properties that are possible to update within an existing [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="32596-132">属性</span><span class="sxs-lookup"><span data-stu-id="32596-132">Property</span></span>|<span data-ttu-id="32596-133">类型</span><span class="sxs-lookup"><span data-stu-id="32596-133">Type</span></span>|<span data-ttu-id="32596-134">说明</span><span class="sxs-lookup"><span data-stu-id="32596-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32596-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="32596-135">allowedAudiences</span></span>|<span data-ttu-id="32596-136">String</span><span class="sxs-lookup"><span data-stu-id="32596-136">String</span></span>|<span data-ttu-id="32596-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="32596-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="32596-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="32596-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="32596-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="32596-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32596-140">categories</span><span class="sxs-lookup"><span data-stu-id="32596-140">categories</span></span>|<span data-ttu-id="32596-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="32596-141">String collection</span></span>|<span data-ttu-id="32596-142">包含用户与兴趣相关联的类别 (例如，个人 recipies) 。</span><span class="sxs-lookup"><span data-stu-id="32596-142">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="32596-143">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="32596-143">collaborationTags</span></span>|<span data-ttu-id="32596-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="32596-144">String collection</span></span>|<span data-ttu-id="32596-145">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="32596-145">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="32596-146">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="32596-146">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="32596-147">说明</span><span class="sxs-lookup"><span data-stu-id="32596-147">description</span></span>|<span data-ttu-id="32596-148">String</span><span class="sxs-lookup"><span data-stu-id="32596-148">String</span></span>|<span data-ttu-id="32596-149">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="32596-149">Contains a description of the interest.</span></span>|
|<span data-ttu-id="32596-150">displayName</span><span class="sxs-lookup"><span data-stu-id="32596-150">displayName</span></span>|<span data-ttu-id="32596-151">String</span><span class="sxs-lookup"><span data-stu-id="32596-151">String</span></span>|<span data-ttu-id="32596-152">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="32596-152">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="32596-153">推导</span><span class="sxs-lookup"><span data-stu-id="32596-153">inference</span></span>|[<span data-ttu-id="32596-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="32596-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="32596-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="32596-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="32596-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="32596-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="32596-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="32596-157">webUrl</span></span>|<span data-ttu-id="32596-158">String</span><span class="sxs-lookup"><span data-stu-id="32596-158">String</span></span>|<span data-ttu-id="32596-159">包含指向有关该兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="32596-159">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="32596-160">响应</span><span class="sxs-lookup"><span data-stu-id="32596-160">Response</span></span>

<span data-ttu-id="32596-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32596-161">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32596-162">示例</span><span class="sxs-lookup"><span data-stu-id="32596-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32596-163">请求</span><span class="sxs-lookup"><span data-stu-id="32596-163">Request</span></span>

<span data-ttu-id="32596-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32596-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32596-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="32596-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "Sports"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="32596-166">C#</span><span class="sxs-lookup"><span data-stu-id="32596-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32596-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32596-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32596-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32596-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32596-169">响应</span><span class="sxs-lookup"><span data-stu-id="32596-169">Response</span></span>

<span data-ttu-id="32596-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32596-170">The following is an example of the response.</span></span>

> <span data-ttu-id="32596-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32596-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


