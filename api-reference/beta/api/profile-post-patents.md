---
title: 创建专利
description: 创建新的专利对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b90cd7f5f3775b7aafc9f19ef9c8039488fabc35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034384"
---
# <a name="create-itempatent"></a><span data-ttu-id="95496-103">创建 itemPatent</span><span class="sxs-lookup"><span data-stu-id="95496-103">Create itemPatent</span></span>

<span data-ttu-id="95496-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95496-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95496-105">在用户的[配置文件](../resources/profile.md)中创建新的[itemPatent](../resources/itempatent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95496-105">Create a new [itemPatent](../resources/itempatent.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="95496-106">权限</span><span class="sxs-lookup"><span data-stu-id="95496-106">Permissions</span></span>

<span data-ttu-id="95496-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95496-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95496-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="95496-109">Permission type</span></span>                        | <span data-ttu-id="95496-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95496-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="95496-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95496-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95496-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="95496-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="95496-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95496-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95496-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="95496-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="95496-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="95496-115">Application</span></span>                            | <span data-ttu-id="95496-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95496-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="95496-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95496-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/patents
POST /users/{id | userPrincipalName}/profile/patents
```

## <a name="request-headers"></a><span data-ttu-id="95496-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="95496-118">Request headers</span></span>
|<span data-ttu-id="95496-119">名称</span><span class="sxs-lookup"><span data-stu-id="95496-119">Name</span></span>|<span data-ttu-id="95496-120">说明</span><span class="sxs-lookup"><span data-stu-id="95496-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="95496-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95496-121">Authorization</span></span>|<span data-ttu-id="95496-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95496-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="95496-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95496-124">Content-Type</span></span>|<span data-ttu-id="95496-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="95496-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95496-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95496-127">Request body</span></span>
<span data-ttu-id="95496-128">在请求正文中，提供 [itemPatent](../resources/itempatent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95496-128">In the request body, supply a JSON representation of the [itemPatent](../resources/itempatent.md) object.</span></span>

<span data-ttu-id="95496-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[itemPatent](../resources/itempatent.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="95496-129">The following table shows the properties that are possible to set when creating a new [itemPatent](../resources/itempatent.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="95496-130">属性</span><span class="sxs-lookup"><span data-stu-id="95496-130">Property</span></span>|<span data-ttu-id="95496-131">类型</span><span class="sxs-lookup"><span data-stu-id="95496-131">Type</span></span>|<span data-ttu-id="95496-132">说明</span><span class="sxs-lookup"><span data-stu-id="95496-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95496-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="95496-133">allowedAudiences</span></span>|<span data-ttu-id="95496-134">String</span><span class="sxs-lookup"><span data-stu-id="95496-134">String</span></span>|<span data-ttu-id="95496-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="95496-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="95496-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="95496-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="95496-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="95496-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="95496-138">description</span><span class="sxs-lookup"><span data-stu-id="95496-138">description</span></span>|<span data-ttu-id="95496-139">String</span><span class="sxs-lookup"><span data-stu-id="95496-139">String</span></span>|<span data-ttu-id="95496-140">专利或档案的 Descpription。</span><span class="sxs-lookup"><span data-stu-id="95496-140">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="95496-141">displayName</span><span class="sxs-lookup"><span data-stu-id="95496-141">displayName</span></span>|<span data-ttu-id="95496-142">String</span><span class="sxs-lookup"><span data-stu-id="95496-142">String</span></span>|<span data-ttu-id="95496-143">专利或档案的标题。</span><span class="sxs-lookup"><span data-stu-id="95496-143">Title of the patent or filing.</span></span> |
|<span data-ttu-id="95496-144">推导</span><span class="sxs-lookup"><span data-stu-id="95496-144">inference</span></span>|[<span data-ttu-id="95496-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="95496-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="95496-146">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="95496-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="95496-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="95496-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="95496-148">isPending</span><span class="sxs-lookup"><span data-stu-id="95496-148">isPending</span></span>        |<span data-ttu-id="95496-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="95496-149">Boolean</span></span>     |<span data-ttu-id="95496-150">指示专利处于待处理状态。</span><span class="sxs-lookup"><span data-stu-id="95496-150">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="95496-151">issuedDate</span><span class="sxs-lookup"><span data-stu-id="95496-151">issuedDate</span></span>       |<span data-ttu-id="95496-152">日期</span><span class="sxs-lookup"><span data-stu-id="95496-152">Date</span></span>        |<span data-ttu-id="95496-153">授予专利的日期。</span><span class="sxs-lookup"><span data-stu-id="95496-153">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="95496-154">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="95496-154">issuingAuthority</span></span> |<span data-ttu-id="95496-155">String</span><span class="sxs-lookup"><span data-stu-id="95496-155">String</span></span>      |<span data-ttu-id="95496-156">授予专利的证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="95496-156">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="95496-157">数字</span><span class="sxs-lookup"><span data-stu-id="95496-157">number</span></span>           |<span data-ttu-id="95496-158">String</span><span class="sxs-lookup"><span data-stu-id="95496-158">String</span></span>      |<span data-ttu-id="95496-159">专利号码。</span><span class="sxs-lookup"><span data-stu-id="95496-159">The patent number.</span></span>                      |
|<span data-ttu-id="95496-160">source</span><span class="sxs-lookup"><span data-stu-id="95496-160">source</span></span>|[<span data-ttu-id="95496-161">personDataSource</span><span class="sxs-lookup"><span data-stu-id="95496-161">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="95496-162">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="95496-162">Where the values originated if synced from another service.</span></span> <span data-ttu-id="95496-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="95496-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="95496-164">WebUrl</span><span class="sxs-lookup"><span data-stu-id="95496-164">webUrl</span></span>           |<span data-ttu-id="95496-165">String</span><span class="sxs-lookup"><span data-stu-id="95496-165">String</span></span>      |<span data-ttu-id="95496-166">引用专利或档案的 URL。</span><span class="sxs-lookup"><span data-stu-id="95496-166">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="95496-167">响应</span><span class="sxs-lookup"><span data-stu-id="95496-167">Response</span></span>

<span data-ttu-id="95496-168">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95496-168">If successful, this method returns a `201 Created` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95496-169">示例</span><span class="sxs-lookup"><span data-stu-id="95496-169">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="95496-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="95496-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itempatent_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/patents
Content-Type: application/json
Content-length: 497

{
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="95496-171">C#</span><span class="sxs-lookup"><span data-stu-id="95496-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempatent-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95496-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95496-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempatent-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95496-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95496-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempatent-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="95496-174">响应</span><span class="sxs-lookup"><span data-stu-id="95496-174">Response</span></span>
<span data-ttu-id="95496-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95496-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 201 Created
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


