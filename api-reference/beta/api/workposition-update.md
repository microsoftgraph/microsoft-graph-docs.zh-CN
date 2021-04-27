---
title: 更新 workPosition
description: 更新用户配置文件中 workPosition 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1028690028c209df1b2dcb6e75dd731c2cca4d36
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051681"
---
# <a name="update-workposition"></a><span data-ttu-id="a1908-103">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="a1908-103">Update workPosition</span></span>

<span data-ttu-id="a1908-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1908-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1908-105">更新用户配置文件 [中的 workPosition](../resources/workposition.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="a1908-105">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1908-106">权限</span><span class="sxs-lookup"><span data-stu-id="a1908-106">Permissions</span></span>

<span data-ttu-id="a1908-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1908-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1908-109">Permission type</span></span>                        | <span data-ttu-id="a1908-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1908-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1908-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1908-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1908-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1908-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a1908-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1908-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1908-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1908-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a1908-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1908-115">Application</span></span>                            | <span data-ttu-id="a1908-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1908-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a1908-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1908-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
PATCH /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a1908-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1908-118">Request headers</span></span>

| <span data-ttu-id="a1908-119">名称</span><span class="sxs-lookup"><span data-stu-id="a1908-119">Name</span></span>           |<span data-ttu-id="a1908-120">说明</span><span class="sxs-lookup"><span data-stu-id="a1908-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a1908-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1908-121">Authorization</span></span>  | <span data-ttu-id="a1908-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1908-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a1908-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1908-124">Content-Type</span></span>   | <span data-ttu-id="a1908-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a1908-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a1908-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1908-127">Request body</span></span>

<span data-ttu-id="a1908-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a1908-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a1908-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a1908-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a1908-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a1908-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="properties"></a><span data-ttu-id="a1908-131">属性</span><span class="sxs-lookup"><span data-stu-id="a1908-131">Properties</span></span>
|<span data-ttu-id="a1908-132">属性</span><span class="sxs-lookup"><span data-stu-id="a1908-132">Property</span></span>|<span data-ttu-id="a1908-133">类型</span><span class="sxs-lookup"><span data-stu-id="a1908-133">Type</span></span>|<span data-ttu-id="a1908-134">说明</span><span class="sxs-lookup"><span data-stu-id="a1908-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1908-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a1908-135">allowedAudiences</span></span>|<span data-ttu-id="a1908-136">String</span><span class="sxs-lookup"><span data-stu-id="a1908-136">String</span></span>|<span data-ttu-id="a1908-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="a1908-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a1908-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a1908-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a1908-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a1908-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a1908-140">categories</span><span class="sxs-lookup"><span data-stu-id="a1908-140">categories</span></span>|<span data-ttu-id="a1908-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="a1908-141">String collection</span></span>|<span data-ttu-id="a1908-142">用户与此位置关联的类别。</span><span class="sxs-lookup"><span data-stu-id="a1908-142">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="a1908-143">同事</span><span class="sxs-lookup"><span data-stu-id="a1908-143">colleagues</span></span>|<span data-ttu-id="a1908-144">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a1908-144">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="a1908-145">与此职位相关联的同事。</span><span class="sxs-lookup"><span data-stu-id="a1908-145">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="a1908-146">detail</span><span class="sxs-lookup"><span data-stu-id="a1908-146">detail</span></span>|[<span data-ttu-id="a1908-147">positionDetail</span><span class="sxs-lookup"><span data-stu-id="a1908-147">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="a1908-148">包含有关该位置的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1908-148">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="a1908-149">inference</span><span class="sxs-lookup"><span data-stu-id="a1908-149">inference</span></span>|[<span data-ttu-id="a1908-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a1908-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a1908-151">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1908-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a1908-152">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a1908-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a1908-153">isCurrent</span><span class="sxs-lookup"><span data-stu-id="a1908-153">isCurrent</span></span>|<span data-ttu-id="a1908-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="a1908-154">Boolean</span></span>|<span data-ttu-id="a1908-155">表示位置是否是当前位置。</span><span class="sxs-lookup"><span data-stu-id="a1908-155">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="a1908-156">manager</span><span class="sxs-lookup"><span data-stu-id="a1908-156">manager</span></span>|[<span data-ttu-id="a1908-157">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="a1908-157">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="a1908-158">包含此位置的用户经理的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1908-158">Contains detail of the user's manager in this position.</span></span>|

## <a name="response"></a><span data-ttu-id="a1908-159">响应</span><span class="sxs-lookup"><span data-stu-id="a1908-159">Response</span></span>

<span data-ttu-id="a1908-160">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [workPosition](../resources/workposition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1908-160">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1908-161">示例</span><span class="sxs-lookup"><span data-stu-id="a1908-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1908-162">请求</span><span class="sxs-lookup"><span data-stu-id="a1908-162">Request</span></span>

<span data-ttu-id="a1908-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1908-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1908-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1908-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
Content-type: application/json

{
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="a1908-165">C#</span><span class="sxs-lookup"><span data-stu-id="a1908-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1908-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1908-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1908-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1908-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1908-168">Java</span><span class="sxs-lookup"><span data-stu-id="a1908-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1908-169">响应</span><span class="sxs-lookup"><span data-stu-id="a1908-169">Response</span></span>

<span data-ttu-id="a1908-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1908-170">The following is an example of the response.</span></span>

> <span data-ttu-id="a1908-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a1908-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "source": null,
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workposition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


