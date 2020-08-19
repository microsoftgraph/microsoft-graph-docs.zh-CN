---
title: 创建 skillProficiency
description: 使用此 API 创建新的 skillProficiency。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1943b28688af983aa0bd78db1b18df246867962d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810056"
---
# <a name="create-skillproficiency"></a><span data-ttu-id="b594e-103">创建 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="b594e-103">Create skillProficiency</span></span>

<span data-ttu-id="b594e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b594e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b594e-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[skillProficiency](../resources/skillproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b594e-105">Use this API to create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b594e-106">权限</span><span class="sxs-lookup"><span data-stu-id="b594e-106">Permissions</span></span>

<span data-ttu-id="b594e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b594e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b594e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b594e-109">Permission type</span></span>                        | <span data-ttu-id="b594e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b594e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b594e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b594e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b594e-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b594e-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b594e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b594e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b594e-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b594e-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b594e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b594e-115">Application</span></span>                            | <span data-ttu-id="b594e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b594e-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b594e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b594e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
POST /users/{id | userPrincipalName}/profile/skills
```

## <a name="request-headers"></a><span data-ttu-id="b594e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b594e-118">Request headers</span></span>

| <span data-ttu-id="b594e-119">名称</span><span class="sxs-lookup"><span data-stu-id="b594e-119">Name</span></span>           | <span data-ttu-id="b594e-120">说明</span><span class="sxs-lookup"><span data-stu-id="b594e-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="b594e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b594e-121">Authorization</span></span>  | <span data-ttu-id="b594e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b594e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b594e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b594e-124">Content-Type</span></span>   | <span data-ttu-id="b594e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b594e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b594e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b594e-127">Request body</span></span>

<span data-ttu-id="b594e-128">在请求正文中，提供 [skillProficiency](../resources/skillproficiency.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b594e-128">In the request body, supply a JSON representation of [skillProficiency](../resources/skillproficiency.md) object.</span></span>

<span data-ttu-id="b594e-129">下表显示了在用户的[配置文件](../resources/profile.md)中创建新的[skillProficiency](../resources/skillproficiency.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="b594e-129">The following table shows the properties that are possible to set when you create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="b594e-130">属性</span><span class="sxs-lookup"><span data-stu-id="b594e-130">Property</span></span>|<span data-ttu-id="b594e-131">类型</span><span class="sxs-lookup"><span data-stu-id="b594e-131">Type</span></span>|<span data-ttu-id="b594e-132">说明</span><span class="sxs-lookup"><span data-stu-id="b594e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b594e-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b594e-133">allowedAudiences</span></span>|<span data-ttu-id="b594e-134">String</span><span class="sxs-lookup"><span data-stu-id="b594e-134">String</span></span>|<span data-ttu-id="b594e-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="b594e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b594e-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b594e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b594e-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b594e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b594e-138">categories</span><span class="sxs-lookup"><span data-stu-id="b594e-138">categories</span></span>|<span data-ttu-id="b594e-139">String collection</span><span class="sxs-lookup"><span data-stu-id="b594e-139">String collection</span></span>|<span data-ttu-id="b594e-140">包含用户与技能相关联的类别 (例如，个人、职业、爱好) 。</span><span class="sxs-lookup"><span data-stu-id="b594e-140">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="b594e-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="b594e-141">collaborationTags</span></span>|<span data-ttu-id="b594e-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b594e-142">String collection</span></span>|<span data-ttu-id="b594e-143">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="b594e-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="b594e-144">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="b594e-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="b594e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b594e-145">displayName</span></span>|<span data-ttu-id="b594e-146">String</span><span class="sxs-lookup"><span data-stu-id="b594e-146">String</span></span>|<span data-ttu-id="b594e-147">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b594e-147">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="b594e-148">推导</span><span class="sxs-lookup"><span data-stu-id="b594e-148">inference</span></span>|[<span data-ttu-id="b594e-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b594e-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b594e-150">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="b594e-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b594e-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b594e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b594e-152">水平</span><span class="sxs-lookup"><span data-stu-id="b594e-152">proficiency</span></span>|<span data-ttu-id="b594e-153">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="b594e-153">skillProficiencyLevel</span></span>|<span data-ttu-id="b594e-154">熟练掌握此技能的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b594e-154">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="b594e-155">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b594e-155">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b594e-156">source</span><span class="sxs-lookup"><span data-stu-id="b594e-156">source</span></span>|[<span data-ttu-id="b594e-157">personDataSource</span><span class="sxs-lookup"><span data-stu-id="b594e-157">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="b594e-158">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="b594e-158">Where the values originated if synced from another service.</span></span> <span data-ttu-id="b594e-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b594e-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b594e-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="b594e-160">webUrl</span></span>|<span data-ttu-id="b594e-161">String</span><span class="sxs-lookup"><span data-stu-id="b594e-161">String</span></span>|<span data-ttu-id="b594e-162">包含指向有关技能的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="b594e-162">Contains a link to an information source about the skill.</span></span> |

## <a name="response"></a><span data-ttu-id="b594e-163">响应</span><span class="sxs-lookup"><span data-stu-id="b594e-163">Response</span></span>

<span data-ttu-id="b594e-164">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [skillProficiency](../resources/skillproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b594e-164">If successful, this method returns `201, Created` response code and a new [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b594e-165">示例</span><span class="sxs-lookup"><span data-stu-id="b594e-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b594e-166">请求</span><span class="sxs-lookup"><span data-stu-id="b594e-166">Request</span></span>

<span data-ttu-id="b594e-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b594e-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b594e-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="b594e-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b594e-169">C#</span><span class="sxs-lookup"><span data-stu-id="b594e-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b594e-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b594e-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b594e-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b594e-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b594e-172">响应</span><span class="sxs-lookup"><span data-stu-id="b594e-172">Response</span></span>
<span data-ttu-id="b594e-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b594e-173">**Note:** The response object shown here might be shortened for readability.</span></span>
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
