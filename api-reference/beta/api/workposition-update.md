---
title: 更新 workPosition
description: 更新用户的配置文件中的 workPosition 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8c814f81a9ffbbb6f9e962c770a9a8908b288cde
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812826"
---
# <a name="update-workposition"></a><span data-ttu-id="b14ef-103">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="b14ef-103">Update workPosition</span></span>

<span data-ttu-id="b14ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b14ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b14ef-105">更新用户的[配置文件](../resources/profile.md)中的[workPosition](../resources/workposition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b14ef-105">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b14ef-106">权限</span><span class="sxs-lookup"><span data-stu-id="b14ef-106">Permissions</span></span>

<span data-ttu-id="b14ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b14ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b14ef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b14ef-109">Permission type</span></span>                        | <span data-ttu-id="b14ef-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b14ef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b14ef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b14ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b14ef-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b14ef-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b14ef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b14ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b14ef-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b14ef-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b14ef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b14ef-115">Application</span></span>                            | <span data-ttu-id="b14ef-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b14ef-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b14ef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b14ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
PATCH /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b14ef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b14ef-118">Request headers</span></span>

| <span data-ttu-id="b14ef-119">名称</span><span class="sxs-lookup"><span data-stu-id="b14ef-119">Name</span></span>           |<span data-ttu-id="b14ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="b14ef-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b14ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b14ef-121">Authorization</span></span>  | <span data-ttu-id="b14ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b14ef-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b14ef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b14ef-124">Content-Type</span></span>   | <span data-ttu-id="b14ef-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b14ef-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b14ef-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b14ef-127">Request body</span></span>

<span data-ttu-id="b14ef-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b14ef-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b14ef-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b14ef-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b14ef-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b14ef-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="properties"></a><span data-ttu-id="b14ef-131">属性</span><span class="sxs-lookup"><span data-stu-id="b14ef-131">Properties</span></span>
|<span data-ttu-id="b14ef-132">属性</span><span class="sxs-lookup"><span data-stu-id="b14ef-132">Property</span></span>|<span data-ttu-id="b14ef-133">类型</span><span class="sxs-lookup"><span data-stu-id="b14ef-133">Type</span></span>|<span data-ttu-id="b14ef-134">说明</span><span class="sxs-lookup"><span data-stu-id="b14ef-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b14ef-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b14ef-135">allowedAudiences</span></span>|<span data-ttu-id="b14ef-136">String</span><span class="sxs-lookup"><span data-stu-id="b14ef-136">String</span></span>|<span data-ttu-id="b14ef-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="b14ef-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b14ef-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b14ef-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b14ef-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b14ef-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b14ef-140">categories</span><span class="sxs-lookup"><span data-stu-id="b14ef-140">categories</span></span>|<span data-ttu-id="b14ef-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b14ef-141">String collection</span></span>|<span data-ttu-id="b14ef-142">用户已与此位置关联的类别。</span><span class="sxs-lookup"><span data-stu-id="b14ef-142">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="b14ef-143">征求</span><span class="sxs-lookup"><span data-stu-id="b14ef-143">colleagues</span></span>|<span data-ttu-id="b14ef-144">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b14ef-144">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="b14ef-145">与此职位相关联的同事。</span><span class="sxs-lookup"><span data-stu-id="b14ef-145">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="b14ef-146">介绍</span><span class="sxs-lookup"><span data-stu-id="b14ef-146">detail</span></span>|[<span data-ttu-id="b14ef-147">positionDetail</span><span class="sxs-lookup"><span data-stu-id="b14ef-147">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="b14ef-148">包含有关职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b14ef-148">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="b14ef-149">推导</span><span class="sxs-lookup"><span data-stu-id="b14ef-149">inference</span></span>|[<span data-ttu-id="b14ef-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b14ef-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b14ef-151">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="b14ef-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b14ef-152">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b14ef-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b14ef-153">isCurrent</span><span class="sxs-lookup"><span data-stu-id="b14ef-153">isCurrent</span></span>|<span data-ttu-id="b14ef-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="b14ef-154">Boolean</span></span>|<span data-ttu-id="b14ef-155">指示位置是否是最新的。</span><span class="sxs-lookup"><span data-stu-id="b14ef-155">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="b14ef-156">manager</span><span class="sxs-lookup"><span data-stu-id="b14ef-156">manager</span></span>|[<span data-ttu-id="b14ef-157">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="b14ef-157">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="b14ef-158">包含用户在此位置的经理的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b14ef-158">Contains detail of the user's manager in this position.</span></span>|

## <a name="response"></a><span data-ttu-id="b14ef-159">响应</span><span class="sxs-lookup"><span data-stu-id="b14ef-159">Response</span></span>

<span data-ttu-id="b14ef-160">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workPosition](../resources/workposition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b14ef-160">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b14ef-161">示例</span><span class="sxs-lookup"><span data-stu-id="b14ef-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b14ef-162">请求</span><span class="sxs-lookup"><span data-stu-id="b14ef-162">Request</span></span>

<span data-ttu-id="b14ef-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b14ef-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b14ef-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b14ef-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b14ef-165">C#</span><span class="sxs-lookup"><span data-stu-id="b14ef-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b14ef-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b14ef-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b14ef-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b14ef-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b14ef-168">响应</span><span class="sxs-lookup"><span data-stu-id="b14ef-168">Response</span></span>

<span data-ttu-id="b14ef-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b14ef-169">The following is an example of the response.</span></span>

> <span data-ttu-id="b14ef-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b14ef-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
