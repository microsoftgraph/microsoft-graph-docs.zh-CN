---
title: 创建 languageProficiency
description: 使用此 API 创建新的 languageProficiency。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ca294f73e9fbac6ea08305f8a85a3688de82b455
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811619"
---
# <a name="create-languageproficiency"></a><span data-ttu-id="9b20a-103">创建 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="9b20a-103">Create languageProficiency</span></span>

<span data-ttu-id="9b20a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b20a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b20a-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[languageProficiency](../resources/languageproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b20a-105">Use this API to create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b20a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b20a-106">Permissions</span></span>

<span data-ttu-id="9b20a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b20a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b20a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b20a-109">Permission type</span></span>                        | <span data-ttu-id="9b20a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b20a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b20a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b20a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b20a-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9b20a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9b20a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b20a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b20a-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9b20a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9b20a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b20a-115">Application</span></span>                            | <span data-ttu-id="9b20a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b20a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9b20a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b20a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/languages
POST /users/{id | userPrincipalName}/profile/languages
```

## <a name="request-headers"></a><span data-ttu-id="9b20a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b20a-118">Request headers</span></span>

| <span data-ttu-id="9b20a-119">名称</span><span class="sxs-lookup"><span data-stu-id="9b20a-119">Name</span></span>           | <span data-ttu-id="9b20a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b20a-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="9b20a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b20a-121">Authorization</span></span>  | <span data-ttu-id="9b20a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b20a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9b20a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b20a-124">Content-Type</span></span>   | <span data-ttu-id="9b20a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9b20a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b20a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b20a-127">Request body</span></span>

<span data-ttu-id="9b20a-128">在请求正文中，提供 [languageProficiency](../resources/languageproficiency.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b20a-128">In the request body, supply a JSON representation of [languageProficiency](../resources/languageproficiency.md) object.</span></span>

<span data-ttu-id="9b20a-129">下表显示了在用户的[配置文件](../resources/profile.md)中创建新的[languageProficiency](../resources/languageproficiency.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="9b20a-129">The following table shows the properties that are possible to set when you create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="9b20a-130">属性</span><span class="sxs-lookup"><span data-stu-id="9b20a-130">Property</span></span>|<span data-ttu-id="9b20a-131">类型</span><span class="sxs-lookup"><span data-stu-id="9b20a-131">Type</span></span>|<span data-ttu-id="9b20a-132">说明</span><span class="sxs-lookup"><span data-stu-id="9b20a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b20a-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="9b20a-133">allowedAudiences</span></span>|<span data-ttu-id="9b20a-134">String</span><span class="sxs-lookup"><span data-stu-id="9b20a-134">String</span></span>|<span data-ttu-id="9b20a-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="9b20a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="9b20a-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9b20a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="9b20a-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b20a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9b20a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9b20a-138">displayName</span></span>|<span data-ttu-id="9b20a-139">String</span><span class="sxs-lookup"><span data-stu-id="9b20a-139">String</span></span>|<span data-ttu-id="9b20a-140">包含语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="9b20a-140">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="9b20a-141">推导</span><span class="sxs-lookup"><span data-stu-id="9b20a-141">inference</span></span>|[<span data-ttu-id="9b20a-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="9b20a-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="9b20a-143">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="9b20a-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="9b20a-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9b20a-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9b20a-145">读物</span><span class="sxs-lookup"><span data-stu-id="9b20a-145">reading</span></span>|<span data-ttu-id="9b20a-146">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="9b20a-146">languageProficiencyLevel</span></span>|<span data-ttu-id="9b20a-147">表示对对象代表的语言进行阅读理解的用户。</span><span class="sxs-lookup"><span data-stu-id="9b20a-147">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="9b20a-148">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b20a-148">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9b20a-149">source</span><span class="sxs-lookup"><span data-stu-id="9b20a-149">source</span></span>|[<span data-ttu-id="9b20a-150">personDataSource</span><span class="sxs-lookup"><span data-stu-id="9b20a-150">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="9b20a-151">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="9b20a-151">Where the values originated if synced from another service.</span></span> <span data-ttu-id="9b20a-152">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9b20a-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9b20a-153">发音</span><span class="sxs-lookup"><span data-stu-id="9b20a-153">spoken</span></span>|<span data-ttu-id="9b20a-154">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="9b20a-154">languageProficiencyLevel</span></span>|<span data-ttu-id="9b20a-155">表示面向对象所代表的语言的熟练程度的用户。</span><span class="sxs-lookup"><span data-stu-id="9b20a-155">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="9b20a-156">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b20a-156">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9b20a-157">tag</span><span class="sxs-lookup"><span data-stu-id="9b20a-157">tag</span></span>|<span data-ttu-id="9b20a-158">String</span><span class="sxs-lookup"><span data-stu-id="9b20a-158">String</span></span>|<span data-ttu-id="9b20a-159">包含四个字符的 BCP47 名称，该语言 (en-us、无 NB、en-us) 。</span><span class="sxs-lookup"><span data-stu-id="9b20a-159">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="9b20a-160">面向</span><span class="sxs-lookup"><span data-stu-id="9b20a-160">written</span></span>|<span data-ttu-id="9b20a-161">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="9b20a-161">languageProficiencyLevel</span></span>|<span data-ttu-id="9b20a-162">代表对象所代表的语言的已编写熟练程度的用户。</span><span class="sxs-lookup"><span data-stu-id="9b20a-162">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="9b20a-163">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b20a-163">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="9b20a-164">响应</span><span class="sxs-lookup"><span data-stu-id="9b20a-164">Response</span></span>

<span data-ttu-id="9b20a-165">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [languageProficiency](../resources/languageproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b20a-165">If successful, this method returns `201, Created` response code and a new [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b20a-166">示例</span><span class="sxs-lookup"><span data-stu-id="9b20a-166">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b20a-167">请求</span><span class="sxs-lookup"><span data-stu-id="9b20a-167">Request</span></span>

<span data-ttu-id="9b20a-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b20a-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b20a-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b20a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_languageproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/languages
Content-type: application/json

{
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```
# <a name="c"></a>[<span data-ttu-id="9b20a-170">C#</span><span class="sxs-lookup"><span data-stu-id="9b20a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-languageproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b20a-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b20a-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-languageproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b20a-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b20a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-languageproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b20a-173">响应</span><span class="sxs-lookup"><span data-stu-id="9b20a-173">Response</span></span>

<span data-ttu-id="9b20a-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b20a-174">The following is an example of the response.</span></span>

> <span data-ttu-id="9b20a-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b20a-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
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
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```
