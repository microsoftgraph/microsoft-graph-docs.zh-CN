---
title: 更新 languageProficiency
description: 更新用户的配置文件中的 languageProficiency 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9d831c0b284d3164c975e3d60cfc8bbaf81afc8b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971565"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="c0593-103">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="c0593-103">Update languageProficiency</span></span>

<span data-ttu-id="c0593-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0593-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0593-105">更新用户的[配置文件](../resources/profile.md)中的[languageProficiency](../resources/languageproficiency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0593-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0593-106">权限</span><span class="sxs-lookup"><span data-stu-id="c0593-106">Permissions</span></span>

<span data-ttu-id="c0593-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0593-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0593-109">Permission type</span></span>                        | <span data-ttu-id="c0593-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0593-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0593-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0593-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0593-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c0593-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c0593-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0593-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0593-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c0593-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c0593-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0593-115">Application</span></span>                            | <span data-ttu-id="c0593-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0593-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="c0593-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0593-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
PATCH /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0593-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0593-118">Request headers</span></span>

| <span data-ttu-id="c0593-119">名称</span><span class="sxs-lookup"><span data-stu-id="c0593-119">Name</span></span>           |<span data-ttu-id="c0593-120">说明</span><span class="sxs-lookup"><span data-stu-id="c0593-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c0593-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0593-121">Authorization</span></span>  | <span data-ttu-id="c0593-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0593-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c0593-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0593-124">Content-Type</span></span>   | <span data-ttu-id="c0593-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c0593-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0593-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0593-127">Request body</span></span>

<span data-ttu-id="c0593-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c0593-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c0593-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c0593-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c0593-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c0593-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="c0593-131">属性</span><span class="sxs-lookup"><span data-stu-id="c0593-131">Property</span></span>|<span data-ttu-id="c0593-132">类型</span><span class="sxs-lookup"><span data-stu-id="c0593-132">Type</span></span>|<span data-ttu-id="c0593-133">说明</span><span class="sxs-lookup"><span data-stu-id="c0593-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0593-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c0593-134">allowedAudiences</span></span>|<span data-ttu-id="c0593-135">String</span><span class="sxs-lookup"><span data-stu-id="c0593-135">String</span></span>|<span data-ttu-id="c0593-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="c0593-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c0593-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c0593-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c0593-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0593-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c0593-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c0593-139">displayName</span></span>|<span data-ttu-id="c0593-140">String</span><span class="sxs-lookup"><span data-stu-id="c0593-140">String</span></span>|<span data-ttu-id="c0593-141">包含语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="c0593-141">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="c0593-142">推导</span><span class="sxs-lookup"><span data-stu-id="c0593-142">inference</span></span>|[<span data-ttu-id="c0593-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c0593-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c0593-144">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="c0593-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c0593-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c0593-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c0593-146">读物</span><span class="sxs-lookup"><span data-stu-id="c0593-146">reading</span></span>|<span data-ttu-id="c0593-147">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="c0593-147">languageProficiencyLevel</span></span>|<span data-ttu-id="c0593-148">表示对对象代表的语言进行阅读理解的用户。</span><span class="sxs-lookup"><span data-stu-id="c0593-148">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="c0593-149">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0593-149">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c0593-150">source</span><span class="sxs-lookup"><span data-stu-id="c0593-150">source</span></span>|[<span data-ttu-id="c0593-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="c0593-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="c0593-152">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="c0593-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="c0593-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c0593-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c0593-154">发音</span><span class="sxs-lookup"><span data-stu-id="c0593-154">spoken</span></span>|<span data-ttu-id="c0593-155">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="c0593-155">languageProficiencyLevel</span></span>|<span data-ttu-id="c0593-156">表示面向对象所代表的语言的熟练程度的用户。</span><span class="sxs-lookup"><span data-stu-id="c0593-156">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="c0593-157">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0593-157">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c0593-158">tag</span><span class="sxs-lookup"><span data-stu-id="c0593-158">tag</span></span>|<span data-ttu-id="c0593-159">String</span><span class="sxs-lookup"><span data-stu-id="c0593-159">String</span></span>|<span data-ttu-id="c0593-160">包含四个字符的 BCP47 名称，该语言 (en-us、无 NB、en-us) 。</span><span class="sxs-lookup"><span data-stu-id="c0593-160">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="c0593-161">面向</span><span class="sxs-lookup"><span data-stu-id="c0593-161">written</span></span>|<span data-ttu-id="c0593-162">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="c0593-162">languageProficiencyLevel</span></span>|<span data-ttu-id="c0593-163">代表对象所代表的语言的已编写熟练程度的用户。</span><span class="sxs-lookup"><span data-stu-id="c0593-163">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="c0593-164">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c0593-164">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="c0593-165">响应</span><span class="sxs-lookup"><span data-stu-id="c0593-165">Response</span></span>

<span data-ttu-id="c0593-166">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [languageProficiency](../resources/languageproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0593-166">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0593-167">示例</span><span class="sxs-lookup"><span data-stu-id="c0593-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0593-168">请求</span><span class="sxs-lookup"><span data-stu-id="c0593-168">Request</span></span>

<span data-ttu-id="c0593-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c0593-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0593-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0593-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="c0593-171">C#</span><span class="sxs-lookup"><span data-stu-id="c0593-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0593-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0593-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0593-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0593-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0593-174">Java</span><span class="sxs-lookup"><span data-stu-id="c0593-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-languageproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c0593-175">响应</span><span class="sxs-lookup"><span data-stu-id="c0593-175">Response</span></span>

<span data-ttu-id="c0593-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0593-176">The following is an example of the response.</span></span>

> <span data-ttu-id="c0593-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0593-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
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
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```


