---
title: 更新 itemPatent
description: 更新 itemPatent 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 92044e1a5e4edb7bbb422571543f6b11ed3e70dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777795"
---
# <a name="update-itempatent"></a><span data-ttu-id="591c0-103">更新 itemPatent</span><span class="sxs-lookup"><span data-stu-id="591c0-103">Update itemPatent</span></span>

<span data-ttu-id="591c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="591c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="591c0-105">更新 [itemPatent 对象](../resources/itempatent.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="591c0-105">Update the properties of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="591c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="591c0-106">Permissions</span></span>

<span data-ttu-id="591c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="591c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="591c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="591c0-109">Permission type</span></span>                        | <span data-ttu-id="591c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="591c0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="591c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="591c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="591c0-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591c0-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="591c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="591c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="591c0-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591c0-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="591c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="591c0-115">Application</span></span>                            | <span data-ttu-id="591c0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591c0-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="591c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="591c0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/patents/{id}
PATCH /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="591c0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="591c0-118">Request headers</span></span>
|<span data-ttu-id="591c0-119">名称</span><span class="sxs-lookup"><span data-stu-id="591c0-119">Name</span></span>|<span data-ttu-id="591c0-120">说明</span><span class="sxs-lookup"><span data-stu-id="591c0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="591c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="591c0-121">Authorization</span></span>|<span data-ttu-id="591c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="591c0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="591c0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="591c0-124">Content-Type</span></span>|<span data-ttu-id="591c0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="591c0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="591c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="591c0-127">Request body</span></span>

<span data-ttu-id="591c0-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="591c0-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="591c0-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="591c0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="591c0-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="591c0-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="591c0-131">属性</span><span class="sxs-lookup"><span data-stu-id="591c0-131">Property</span></span>|<span data-ttu-id="591c0-132">类型</span><span class="sxs-lookup"><span data-stu-id="591c0-132">Type</span></span>|<span data-ttu-id="591c0-133">说明</span><span class="sxs-lookup"><span data-stu-id="591c0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="591c0-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="591c0-134">allowedAudiences</span></span>|<span data-ttu-id="591c0-135">字符串</span><span class="sxs-lookup"><span data-stu-id="591c0-135">String</span></span>|<span data-ttu-id="591c0-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="591c0-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="591c0-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="591c0-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="591c0-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="591c0-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="591c0-139">说明</span><span class="sxs-lookup"><span data-stu-id="591c0-139">description</span></span>|<span data-ttu-id="591c0-140">字符串</span><span class="sxs-lookup"><span data-stu-id="591c0-140">String</span></span>|<span data-ttu-id="591c0-141">专利或归档的去向。</span><span class="sxs-lookup"><span data-stu-id="591c0-141">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="591c0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="591c0-142">displayName</span></span>|<span data-ttu-id="591c0-143">字符串</span><span class="sxs-lookup"><span data-stu-id="591c0-143">String</span></span>|<span data-ttu-id="591c0-144">专利或归档的标题。</span><span class="sxs-lookup"><span data-stu-id="591c0-144">Title of the patent or filing.</span></span> |
|<span data-ttu-id="591c0-145">inference</span><span class="sxs-lookup"><span data-stu-id="591c0-145">inference</span></span>|[<span data-ttu-id="591c0-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="591c0-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="591c0-147">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="591c0-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="591c0-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="591c0-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="591c0-149">isPending</span><span class="sxs-lookup"><span data-stu-id="591c0-149">isPending</span></span>        |<span data-ttu-id="591c0-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="591c0-150">Boolean</span></span>     |<span data-ttu-id="591c0-151">指示正在申请专利。</span><span class="sxs-lookup"><span data-stu-id="591c0-151">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="591c0-152">issuedDate</span><span class="sxs-lookup"><span data-stu-id="591c0-152">issuedDate</span></span>       |<span data-ttu-id="591c0-153">日期</span><span class="sxs-lookup"><span data-stu-id="591c0-153">Date</span></span>        |<span data-ttu-id="591c0-154">授予专利的日期。</span><span class="sxs-lookup"><span data-stu-id="591c0-154">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="591c0-155">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="591c0-155">issuingAuthority</span></span> |<span data-ttu-id="591c0-156">字符串</span><span class="sxs-lookup"><span data-stu-id="591c0-156">String</span></span>      |<span data-ttu-id="591c0-157">授予专利的颁发机构。</span><span class="sxs-lookup"><span data-stu-id="591c0-157">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="591c0-158">number</span><span class="sxs-lookup"><span data-stu-id="591c0-158">number</span></span>           |<span data-ttu-id="591c0-159">字符串</span><span class="sxs-lookup"><span data-stu-id="591c0-159">String</span></span>      |<span data-ttu-id="591c0-160">专利号。</span><span class="sxs-lookup"><span data-stu-id="591c0-160">The patent number.</span></span>                      |
|<span data-ttu-id="591c0-161">source</span><span class="sxs-lookup"><span data-stu-id="591c0-161">source</span></span>|[<span data-ttu-id="591c0-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="591c0-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="591c0-163">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="591c0-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="591c0-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="591c0-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="591c0-165">WebUrl</span><span class="sxs-lookup"><span data-stu-id="591c0-165">webUrl</span></span>           |<span data-ttu-id="591c0-166">String</span><span class="sxs-lookup"><span data-stu-id="591c0-166">String</span></span>      |<span data-ttu-id="591c0-167">引用专利或归档的 URL。</span><span class="sxs-lookup"><span data-stu-id="591c0-167">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="591c0-168">响应</span><span class="sxs-lookup"><span data-stu-id="591c0-168">Response</span></span>

<span data-ttu-id="591c0-169">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="591c0-169">If successful, this method returns a `200 OK` response code and an updated [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="591c0-170">示例</span><span class="sxs-lookup"><span data-stu-id="591c0-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="591c0-171">请求</span><span class="sxs-lookup"><span data-stu-id="591c0-171">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="591c0-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="591c0-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itempatent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/patents/{id}
Content-Type: application/json
Content-length: 497

{
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="591c0-173">C#</span><span class="sxs-lookup"><span data-stu-id="591c0-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="591c0-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="591c0-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="591c0-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="591c0-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="591c0-176">Java</span><span class="sxs-lookup"><span data-stu-id="591c0-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-itempatent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="591c0-177">响应</span><span class="sxs-lookup"><span data-stu-id="591c0-177">Response</span></span>
<span data-ttu-id="591c0-178">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="591c0-178">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```


