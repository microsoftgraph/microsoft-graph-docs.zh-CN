---
title: 创建 workPosition
description: 使用此 API 创建新的 workPosition。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 178752d0a3b504c3edd160b321043e3194aab314
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820340"
---
# <a name="create-workposition"></a><span data-ttu-id="4d981-103">创建 workPosition</span><span class="sxs-lookup"><span data-stu-id="4d981-103">Create workPosition</span></span>

<span data-ttu-id="4d981-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d981-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d981-105">使用此 API 在用户配置文件[中创建新工作](../resources/workposition.md)[位置](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="4d981-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d981-106">权限</span><span class="sxs-lookup"><span data-stu-id="4d981-106">Permissions</span></span>

<span data-ttu-id="4d981-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d981-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d981-109">Permission type</span></span>                        | <span data-ttu-id="4d981-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d981-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d981-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d981-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d981-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d981-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4d981-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d981-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d981-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d981-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4d981-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d981-115">Application</span></span>                            | <span data-ttu-id="4d981-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d981-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4d981-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d981-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
POST /users/{id | userPrincipalName}/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="4d981-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d981-118">Request headers</span></span>

| <span data-ttu-id="4d981-119">名称</span><span class="sxs-lookup"><span data-stu-id="4d981-119">Name</span></span>      |<span data-ttu-id="4d981-120">说明</span><span class="sxs-lookup"><span data-stu-id="4d981-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d981-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d981-121">Authorization</span></span>  | <span data-ttu-id="4d981-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d981-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4d981-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d981-124">Content-Type</span></span>   | <span data-ttu-id="4d981-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4d981-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d981-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d981-127">Request body</span></span>

<span data-ttu-id="4d981-128">在请求正文中，提供 [workPosition](../resources/workposition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d981-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

<span data-ttu-id="4d981-129">下表显示在用户的配置文件中创建新 [workPosition](../resources/workPosition.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="4d981-129">The following table shows the properties that are possible to set when you create a new [workPosition](../resources/workPosition.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="4d981-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d981-130">Property</span></span>|<span data-ttu-id="4d981-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d981-131">Type</span></span>|<span data-ttu-id="4d981-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d981-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d981-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4d981-133">allowedAudiences</span></span>|<span data-ttu-id="4d981-134">String</span><span class="sxs-lookup"><span data-stu-id="4d981-134">String</span></span>|<span data-ttu-id="4d981-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="4d981-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4d981-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4d981-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4d981-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4d981-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4d981-138">categories</span><span class="sxs-lookup"><span data-stu-id="4d981-138">categories</span></span>|<span data-ttu-id="4d981-139">String collection</span><span class="sxs-lookup"><span data-stu-id="4d981-139">String collection</span></span>|<span data-ttu-id="4d981-140">用户具有与此位置关联的类别。</span><span class="sxs-lookup"><span data-stu-id="4d981-140">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="4d981-141">同事</span><span class="sxs-lookup"><span data-stu-id="4d981-141">colleagues</span></span>|<span data-ttu-id="4d981-142">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d981-142">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="4d981-143">与此位置关联的同事。</span><span class="sxs-lookup"><span data-stu-id="4d981-143">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="4d981-144">detail</span><span class="sxs-lookup"><span data-stu-id="4d981-144">detail</span></span>|[<span data-ttu-id="4d981-145">positionDetail</span><span class="sxs-lookup"><span data-stu-id="4d981-145">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="4d981-146">包含位置的相关详细信息。</span><span class="sxs-lookup"><span data-stu-id="4d981-146">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="4d981-147">推据</span><span class="sxs-lookup"><span data-stu-id="4d981-147">inference</span></span>|[<span data-ttu-id="4d981-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4d981-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4d981-149">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="4d981-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4d981-150">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4d981-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4d981-151">isCurrent</span><span class="sxs-lookup"><span data-stu-id="4d981-151">isCurrent</span></span>|<span data-ttu-id="4d981-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d981-152">Boolean</span></span>|<span data-ttu-id="4d981-153">表示位置是否是当前位置。</span><span class="sxs-lookup"><span data-stu-id="4d981-153">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="4d981-154">manager</span><span class="sxs-lookup"><span data-stu-id="4d981-154">manager</span></span>|[<span data-ttu-id="4d981-155">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="4d981-155">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="4d981-156">包含此位置中的用户经理的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4d981-156">Contains detail of the user's manager in this position.</span></span>|
|<span data-ttu-id="4d981-157">source</span><span class="sxs-lookup"><span data-stu-id="4d981-157">source</span></span>|[<span data-ttu-id="4d981-158">personDataSource</span><span class="sxs-lookup"><span data-stu-id="4d981-158">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="4d981-159">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="4d981-159">Where the values originated if synced from another service.</span></span> <span data-ttu-id="4d981-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4d981-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4d981-161">响应</span><span class="sxs-lookup"><span data-stu-id="4d981-161">Response</span></span>

<span data-ttu-id="4d981-162">如果成功，此方法在 `201, Created` 响应正文中返回 [响应代码](../resources/workposition.md) 和新的 workPosition 对象。</span><span class="sxs-lookup"><span data-stu-id="4d981-162">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d981-163">示例</span><span class="sxs-lookup"><span data-stu-id="4d981-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d981-164">请求</span><span class="sxs-lookup"><span data-stu-id="4d981-164">Request</span></span>

<span data-ttu-id="4d981-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d981-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d981-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d981-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/positions
Content-type: application/json

{
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
  },
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="4d981-167">C#</span><span class="sxs-lookup"><span data-stu-id="4d981-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workposition-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d981-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d981-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workposition-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d981-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d981-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workposition-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d981-170">响应</span><span class="sxs-lookup"><span data-stu-id="4d981-170">Response</span></span>

<span data-ttu-id="4d981-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d981-171">The following is an example of the response.</span></span>

> <span data-ttu-id="4d981-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4d981-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 201 Created
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
