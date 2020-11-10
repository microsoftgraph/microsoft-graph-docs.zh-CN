---
title: 创建 personAnniversary
description: 使用此 API 创建新的 personAnniversary。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 89cae3dc7fe0b5e1b314adbebd9510eab5f65d23
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964591"
---
# <a name="create-personanniversary"></a><span data-ttu-id="4b769-103">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="4b769-103">Create personAnniversary</span></span>

<span data-ttu-id="4b769-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b769-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b769-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b769-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b769-106">权限</span><span class="sxs-lookup"><span data-stu-id="4b769-106">Permissions</span></span>

<span data-ttu-id="4b769-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b769-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b769-109">Permission type</span></span>                        | <span data-ttu-id="4b769-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b769-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b769-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b769-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b769-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4b769-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b769-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b769-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b769-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4b769-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b769-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b769-115">Application</span></span>                            | <span data-ttu-id="4b769-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b769-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4b769-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b769-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="4b769-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b769-118">Request headers</span></span>

| <span data-ttu-id="4b769-119">名称</span><span class="sxs-lookup"><span data-stu-id="4b769-119">Name</span></span>      |<span data-ttu-id="4b769-120">说明</span><span class="sxs-lookup"><span data-stu-id="4b769-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b769-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b769-121">Authorization</span></span>  | <span data-ttu-id="4b769-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b769-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4b769-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b769-124">Content-Type</span></span>   | <span data-ttu-id="4b769-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4b769-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b769-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b769-127">Request body</span></span>

<span data-ttu-id="4b769-128">在请求正文中，提供 [personAnniversary](../resources/personanniversary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b769-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="4b769-129">下表显示了可以在用户 [配置文件](../resources/profile.md)中的新 \* \* personAnniversary \* \* \* \* 对象中设置的属性。</span><span class="sxs-lookup"><span data-stu-id="4b769-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="4b769-130">属性</span><span class="sxs-lookup"><span data-stu-id="4b769-130">Property</span></span>|<span data-ttu-id="4b769-131">类型</span><span class="sxs-lookup"><span data-stu-id="4b769-131">Type</span></span>|<span data-ttu-id="4b769-132">说明</span><span class="sxs-lookup"><span data-stu-id="4b769-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b769-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4b769-133">allowedAudiences</span></span>|<span data-ttu-id="4b769-134">String</span><span class="sxs-lookup"><span data-stu-id="4b769-134">String</span></span>|<span data-ttu-id="4b769-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="4b769-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4b769-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4b769-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4b769-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4b769-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4b769-138">date</span><span class="sxs-lookup"><span data-stu-id="4b769-138">date</span></span>|<span data-ttu-id="4b769-139">Date</span><span class="sxs-lookup"><span data-stu-id="4b769-139">Date</span></span>|<span data-ttu-id="4b769-140">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="4b769-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="4b769-141">推导</span><span class="sxs-lookup"><span data-stu-id="4b769-141">inference</span></span>|[<span data-ttu-id="4b769-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4b769-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4b769-143">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="4b769-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4b769-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4b769-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4b769-145">source</span><span class="sxs-lookup"><span data-stu-id="4b769-145">source</span></span>|[<span data-ttu-id="4b769-146">personDataSource</span><span class="sxs-lookup"><span data-stu-id="4b769-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="4b769-147">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="4b769-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="4b769-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4b769-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4b769-149">type</span><span class="sxs-lookup"><span data-stu-id="4b769-149">type</span></span>|<span data-ttu-id="4b769-150">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="4b769-150">anniversaryType</span></span>|<span data-ttu-id="4b769-151">日期所代表的周年纪念的类型。</span><span class="sxs-lookup"><span data-stu-id="4b769-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="4b769-152">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4b769-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="4b769-153">响应</span><span class="sxs-lookup"><span data-stu-id="4b769-153">Response</span></span>

<span data-ttu-id="4b769-154">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [personAnniversary](../resources/personanniversary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b769-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b769-155">示例</span><span class="sxs-lookup"><span data-stu-id="4b769-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b769-156">请求</span><span class="sxs-lookup"><span data-stu-id="4b769-156">Request</span></span>

<span data-ttu-id="4b769-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b769-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b769-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b769-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "birthday",
  "date": "1980-01-08"
}
```
# <a name="c"></a>[<span data-ttu-id="4b769-159">C#</span><span class="sxs-lookup"><span data-stu-id="4b769-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b769-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b769-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b769-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b769-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b769-162">Java</span><span class="sxs-lookup"><span data-stu-id="4b769-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personanniversary-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4b769-163">响应</span><span class="sxs-lookup"><span data-stu-id="4b769-163">Response</span></span>

<span data-ttu-id="4b769-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b769-164">The following is an example of the response.</span></span>

> <span data-ttu-id="4b769-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4b769-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
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
  "type": "birthday",
  "date": "Date"
}
```


