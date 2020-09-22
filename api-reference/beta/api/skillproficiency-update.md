---
title: 更新 skillProficiency
description: 更新用户的配置文件中的 skillProficiency 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d62205d62af5977a8855c990604dbb31621a9134
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044361"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="4bd27-103">更新 skillproficiency</span><span class="sxs-lookup"><span data-stu-id="4bd27-103">Update skillproficiency</span></span>

<span data-ttu-id="4bd27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bd27-105">更新用户的[配置文件](../resources/profile.md)中的[skillProficiency](../resources/skillproficiency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4bd27-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bd27-106">权限</span><span class="sxs-lookup"><span data-stu-id="4bd27-106">Permissions</span></span>

<span data-ttu-id="4bd27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bd27-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bd27-109">Permission type</span></span>                        | <span data-ttu-id="4bd27-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bd27-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bd27-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd27-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bd27-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4bd27-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4bd27-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd27-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4bd27-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4bd27-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bd27-115">Application</span></span>                            | <span data-ttu-id="4bd27-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd27-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4bd27-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bd27-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
PATCH /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4bd27-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bd27-118">Request headers</span></span>

| <span data-ttu-id="4bd27-119">名称</span><span class="sxs-lookup"><span data-stu-id="4bd27-119">Name</span></span>           |<span data-ttu-id="4bd27-120">说明</span><span class="sxs-lookup"><span data-stu-id="4bd27-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4bd27-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd27-121">Authorization</span></span>  | <span data-ttu-id="4bd27-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bd27-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4bd27-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bd27-124">Content-Type</span></span>   | <span data-ttu-id="4bd27-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4bd27-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4bd27-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bd27-127">Request body</span></span>

<span data-ttu-id="4bd27-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4bd27-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4bd27-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4bd27-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4bd27-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4bd27-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="4bd27-131">属性</span><span class="sxs-lookup"><span data-stu-id="4bd27-131">Property</span></span>|<span data-ttu-id="4bd27-132">类型</span><span class="sxs-lookup"><span data-stu-id="4bd27-132">Type</span></span>|<span data-ttu-id="4bd27-133">说明</span><span class="sxs-lookup"><span data-stu-id="4bd27-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bd27-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4bd27-134">allowedAudiences</span></span>|<span data-ttu-id="4bd27-135">String</span><span class="sxs-lookup"><span data-stu-id="4bd27-135">String</span></span>|<span data-ttu-id="4bd27-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="4bd27-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4bd27-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4bd27-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4bd27-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4bd27-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4bd27-139">类别</span><span class="sxs-lookup"><span data-stu-id="4bd27-139">categories</span></span>|<span data-ttu-id="4bd27-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="4bd27-140">String collection</span></span>|<span data-ttu-id="4bd27-141">包含用户与技能相关联的类别 (例如，个人、职业、爱好) 。</span><span class="sxs-lookup"><span data-stu-id="4bd27-141">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="4bd27-142">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="4bd27-142">collaborationTags</span></span>|<span data-ttu-id="4bd27-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="4bd27-143">String collection</span></span>|<span data-ttu-id="4bd27-144">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="4bd27-144">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="4bd27-145">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="4bd27-145">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="4bd27-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4bd27-146">displayName</span></span>|<span data-ttu-id="4bd27-147">String</span><span class="sxs-lookup"><span data-stu-id="4bd27-147">String</span></span>|<span data-ttu-id="4bd27-148">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="4bd27-148">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="4bd27-149">推导</span><span class="sxs-lookup"><span data-stu-id="4bd27-149">inference</span></span>|[<span data-ttu-id="4bd27-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4bd27-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4bd27-151">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="4bd27-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4bd27-152">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4bd27-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4bd27-153">水平</span><span class="sxs-lookup"><span data-stu-id="4bd27-153">proficiency</span></span>|<span data-ttu-id="4bd27-154">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="4bd27-154">skillProficiencyLevel</span></span>|<span data-ttu-id="4bd27-155">熟练掌握此技能的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4bd27-155">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="4bd27-156">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4bd27-156">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="4bd27-157">响应</span><span class="sxs-lookup"><span data-stu-id="4bd27-157">Response</span></span>

<span data-ttu-id="4bd27-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [skillProficiency](../resources/skillproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bd27-158">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bd27-159">示例</span><span class="sxs-lookup"><span data-stu-id="4bd27-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4bd27-160">请求</span><span class="sxs-lookup"><span data-stu-id="4bd27-160">Request</span></span>

<span data-ttu-id="4bd27-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4bd27-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bd27-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd27-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4bd27-163">C#</span><span class="sxs-lookup"><span data-stu-id="4bd27-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bd27-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bd27-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bd27-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bd27-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4bd27-166">响应</span><span class="sxs-lookup"><span data-stu-id="4bd27-166">Response</span></span>

<span data-ttu-id="4bd27-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bd27-167">The following is an example of the response.</span></span>

> <span data-ttu-id="4bd27-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4bd27-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


