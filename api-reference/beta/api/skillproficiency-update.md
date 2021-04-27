---
title: 更新 skillProficiency
description: 更新用户配置文件中的 skillProficiency 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da18f3fc53cac80fc4f357083c6dea3c95d5c84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048986"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="d9326-103">更新技能</span><span class="sxs-lookup"><span data-stu-id="d9326-103">Update skillproficiency</span></span>

<span data-ttu-id="d9326-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9326-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9326-105">更新用户配置文件 [中的一个技能Proficiency](../resources/skillproficiency.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="d9326-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9326-106">权限</span><span class="sxs-lookup"><span data-stu-id="d9326-106">Permissions</span></span>

<span data-ttu-id="d9326-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9326-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9326-109">Permission type</span></span>                        | <span data-ttu-id="d9326-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9326-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9326-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9326-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9326-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9326-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d9326-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9326-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9326-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9326-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d9326-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9326-115">Application</span></span>                            | <span data-ttu-id="d9326-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9326-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d9326-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9326-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
PATCH /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9326-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9326-118">Request headers</span></span>

| <span data-ttu-id="d9326-119">名称</span><span class="sxs-lookup"><span data-stu-id="d9326-119">Name</span></span>           |<span data-ttu-id="d9326-120">说明</span><span class="sxs-lookup"><span data-stu-id="d9326-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d9326-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9326-121">Authorization</span></span>  | <span data-ttu-id="d9326-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9326-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d9326-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9326-124">Content-Type</span></span>   | <span data-ttu-id="d9326-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d9326-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d9326-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9326-127">Request body</span></span>

<span data-ttu-id="d9326-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d9326-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d9326-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d9326-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d9326-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d9326-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d9326-131">属性</span><span class="sxs-lookup"><span data-stu-id="d9326-131">Property</span></span>|<span data-ttu-id="d9326-132">类型</span><span class="sxs-lookup"><span data-stu-id="d9326-132">Type</span></span>|<span data-ttu-id="d9326-133">说明</span><span class="sxs-lookup"><span data-stu-id="d9326-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9326-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d9326-134">allowedAudiences</span></span>|<span data-ttu-id="d9326-135">String</span><span class="sxs-lookup"><span data-stu-id="d9326-135">String</span></span>|<span data-ttu-id="d9326-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="d9326-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d9326-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d9326-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d9326-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d9326-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d9326-139">categories</span><span class="sxs-lookup"><span data-stu-id="d9326-139">categories</span></span>|<span data-ttu-id="d9326-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9326-140">String collection</span></span>|<span data-ttu-id="d9326-141">包含用户与技能类别关联的类别 (例如个人、专业、爱好) 。</span><span class="sxs-lookup"><span data-stu-id="d9326-141">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="d9326-142">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="d9326-142">collaborationTags</span></span>|<span data-ttu-id="d9326-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d9326-143">String collection</span></span>|<span data-ttu-id="d9326-144">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="d9326-144">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="d9326-145">集合中允许的值为 `askMeAbout` `ableToMentor` ：、、、。 `wantsToLearn` `wantsToImprove`</span><span class="sxs-lookup"><span data-stu-id="d9326-145">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="d9326-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d9326-146">displayName</span></span>|<span data-ttu-id="d9326-147">String</span><span class="sxs-lookup"><span data-stu-id="d9326-147">String</span></span>|<span data-ttu-id="d9326-148">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d9326-148">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="d9326-149">inference</span><span class="sxs-lookup"><span data-stu-id="d9326-149">inference</span></span>|[<span data-ttu-id="d9326-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d9326-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d9326-151">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="d9326-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d9326-152">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d9326-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d9326-153">熟练程度</span><span class="sxs-lookup"><span data-stu-id="d9326-153">proficiency</span></span>|<span data-ttu-id="d9326-154">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="d9326-154">skillProficiencyLevel</span></span>|<span data-ttu-id="d9326-155">此技能的用户熟练程度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d9326-155">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="d9326-156">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d9326-156">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="d9326-157">响应</span><span class="sxs-lookup"><span data-stu-id="d9326-157">Response</span></span>

<span data-ttu-id="d9326-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [skillProficiency](../resources/skillproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9326-158">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9326-159">示例</span><span class="sxs-lookup"><span data-stu-id="d9326-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9326-160">请求</span><span class="sxs-lookup"><span data-stu-id="d9326-160">Request</span></span>

<span data-ttu-id="d9326-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9326-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9326-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9326-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_skillproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/skills/{id}
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "proficiency": "advancedProfessional"
}
```
# <a name="c"></a>[<span data-ttu-id="d9326-163">C#</span><span class="sxs-lookup"><span data-stu-id="d9326-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9326-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9326-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9326-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9326-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9326-166">Java</span><span class="sxs-lookup"><span data-stu-id="d9326-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9326-167">响应</span><span class="sxs-lookup"><span data-stu-id="d9326-167">Response</span></span>

<span data-ttu-id="d9326-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9326-168">The following is an example of the response.</span></span>

> <span data-ttu-id="d9326-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d9326-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


