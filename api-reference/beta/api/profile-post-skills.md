---
title: 创建 skillProficiency
description: 使用此 API 创建新的 skillProficiency。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 873e568e86972e3d5b0581635e1ef8f4b6a1c612
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972717"
---
# <a name="create-skillproficiency"></a><span data-ttu-id="4177b-103">创建 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="4177b-103">Create skillProficiency</span></span>

<span data-ttu-id="4177b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4177b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4177b-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[skillProficiency](../resources/skillproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4177b-105">Use this API to create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4177b-106">权限</span><span class="sxs-lookup"><span data-stu-id="4177b-106">Permissions</span></span>

<span data-ttu-id="4177b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4177b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4177b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4177b-109">Permission type</span></span>                        | <span data-ttu-id="4177b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4177b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4177b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4177b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4177b-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4177b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4177b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4177b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4177b-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4177b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4177b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4177b-115">Application</span></span>                            | <span data-ttu-id="4177b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4177b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4177b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4177b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
POST /users/{id | userPrincipalName}/profile/skills
```

## <a name="request-headers"></a><span data-ttu-id="4177b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4177b-118">Request headers</span></span>

| <span data-ttu-id="4177b-119">名称</span><span class="sxs-lookup"><span data-stu-id="4177b-119">Name</span></span>           | <span data-ttu-id="4177b-120">说明</span><span class="sxs-lookup"><span data-stu-id="4177b-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="4177b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4177b-121">Authorization</span></span>  | <span data-ttu-id="4177b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4177b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4177b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4177b-124">Content-Type</span></span>   | <span data-ttu-id="4177b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4177b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4177b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4177b-127">Request body</span></span>

<span data-ttu-id="4177b-128">在请求正文中，提供 [skillProficiency](../resources/skillproficiency.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4177b-128">In the request body, supply a JSON representation of [skillProficiency](../resources/skillproficiency.md) object.</span></span>

<span data-ttu-id="4177b-129">下表显示了在用户的[配置文件](../resources/profile.md)中创建新的[skillProficiency](../resources/skillproficiency.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="4177b-129">The following table shows the properties that are possible to set when you create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="4177b-130">属性</span><span class="sxs-lookup"><span data-stu-id="4177b-130">Property</span></span>|<span data-ttu-id="4177b-131">类型</span><span class="sxs-lookup"><span data-stu-id="4177b-131">Type</span></span>|<span data-ttu-id="4177b-132">说明</span><span class="sxs-lookup"><span data-stu-id="4177b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4177b-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4177b-133">allowedAudiences</span></span>|<span data-ttu-id="4177b-134">String</span><span class="sxs-lookup"><span data-stu-id="4177b-134">String</span></span>|<span data-ttu-id="4177b-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="4177b-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4177b-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4177b-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4177b-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4177b-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4177b-138">categories</span><span class="sxs-lookup"><span data-stu-id="4177b-138">categories</span></span>|<span data-ttu-id="4177b-139">String collection</span><span class="sxs-lookup"><span data-stu-id="4177b-139">String collection</span></span>|<span data-ttu-id="4177b-140">包含用户与技能相关联的类别 (例如，个人、职业、爱好) 。</span><span class="sxs-lookup"><span data-stu-id="4177b-140">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="4177b-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="4177b-141">collaborationTags</span></span>|<span data-ttu-id="4177b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4177b-142">String collection</span></span>|<span data-ttu-id="4177b-143">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="4177b-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="4177b-144">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="4177b-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="4177b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4177b-145">displayName</span></span>|<span data-ttu-id="4177b-146">String</span><span class="sxs-lookup"><span data-stu-id="4177b-146">String</span></span>|<span data-ttu-id="4177b-147">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="4177b-147">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="4177b-148">推导</span><span class="sxs-lookup"><span data-stu-id="4177b-148">inference</span></span>|[<span data-ttu-id="4177b-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4177b-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4177b-150">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="4177b-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4177b-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4177b-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4177b-152">水平</span><span class="sxs-lookup"><span data-stu-id="4177b-152">proficiency</span></span>|<span data-ttu-id="4177b-153">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="4177b-153">skillProficiencyLevel</span></span>|<span data-ttu-id="4177b-154">熟练掌握此技能的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4177b-154">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="4177b-155">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4177b-155">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4177b-156">source</span><span class="sxs-lookup"><span data-stu-id="4177b-156">source</span></span>|[<span data-ttu-id="4177b-157">personDataSource</span><span class="sxs-lookup"><span data-stu-id="4177b-157">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="4177b-158">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="4177b-158">Where the values originated if synced from another service.</span></span> <span data-ttu-id="4177b-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4177b-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4177b-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="4177b-160">webUrl</span></span>|<span data-ttu-id="4177b-161">String</span><span class="sxs-lookup"><span data-stu-id="4177b-161">String</span></span>|<span data-ttu-id="4177b-162">包含指向有关技能的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="4177b-162">Contains a link to an information source about the skill.</span></span> |

## <a name="response"></a><span data-ttu-id="4177b-163">响应</span><span class="sxs-lookup"><span data-stu-id="4177b-163">Response</span></span>

<span data-ttu-id="4177b-164">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [skillProficiency](../resources/skillproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4177b-164">If successful, this method returns `201, Created` response code and a new [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4177b-165">示例</span><span class="sxs-lookup"><span data-stu-id="4177b-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4177b-166">请求</span><span class="sxs-lookup"><span data-stu-id="4177b-166">Request</span></span>

<span data-ttu-id="4177b-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4177b-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4177b-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="4177b-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_skillproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/skills
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "allowedAudiences": "organization",
  "displayName": "API Design",
  "proficiency": "generalProfessional",
  "collaborationTags": [
    "ableToMentor"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="4177b-169">C#</span><span class="sxs-lookup"><span data-stu-id="4177b-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4177b-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4177b-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4177b-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4177b-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4177b-172">Java</span><span class="sxs-lookup"><span data-stu-id="4177b-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-skillproficiency-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4177b-173">响应</span><span class="sxs-lookup"><span data-stu-id="4177b-173">Response</span></span>
<span data-ttu-id="4177b-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4177b-174">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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


