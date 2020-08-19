---
title: 创建 projectParticipation
description: 使用此 API 创建新的 projectParticipation。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 29d8bf6342dc1b1b07c7a07a1fe96dd399b5a8e8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811600"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="08c87-103">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="08c87-103">Create projectParticipation</span></span>

<span data-ttu-id="08c87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08c87-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[projectParticipation](../resources/projectParticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08c87-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08c87-106">权限</span><span class="sxs-lookup"><span data-stu-id="08c87-106">Permissions</span></span>

<span data-ttu-id="08c87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08c87-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="08c87-109">Permission type</span></span>                        | <span data-ttu-id="08c87-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08c87-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08c87-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08c87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08c87-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="08c87-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="08c87-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08c87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08c87-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="08c87-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="08c87-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="08c87-115">Application</span></span>                            | <span data-ttu-id="08c87-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c87-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="08c87-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08c87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
POST /users/{id | userPrincipalName}/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="08c87-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="08c87-118">Request headers</span></span>

| <span data-ttu-id="08c87-119">名称</span><span class="sxs-lookup"><span data-stu-id="08c87-119">Name</span></span>           |<span data-ttu-id="08c87-120">说明</span><span class="sxs-lookup"><span data-stu-id="08c87-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="08c87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c87-121">Authorization</span></span>  | <span data-ttu-id="08c87-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08c87-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="08c87-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08c87-124">Content-Type</span></span>   | <span data-ttu-id="08c87-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="08c87-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08c87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08c87-127">Request body</span></span>

<span data-ttu-id="08c87-128">在请求正文中，提供 [projectParticipation](../resources/projectparticipation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08c87-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

<span data-ttu-id="08c87-129">下表显示了在用户的[配置文件](../resources/profile.md)中创建新的[projectParticipation](../resources/projectParticipation.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="08c87-129">The following table shows the properties that are possible to set when you create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="08c87-130">属性</span><span class="sxs-lookup"><span data-stu-id="08c87-130">Property</span></span>|<span data-ttu-id="08c87-131">类型</span><span class="sxs-lookup"><span data-stu-id="08c87-131">Type</span></span>|<span data-ttu-id="08c87-132">说明</span><span class="sxs-lookup"><span data-stu-id="08c87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c87-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="08c87-133">allowedAudiences</span></span>|<span data-ttu-id="08c87-134">String</span><span class="sxs-lookup"><span data-stu-id="08c87-134">String</span></span>|<span data-ttu-id="08c87-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="08c87-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="08c87-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="08c87-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="08c87-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="08c87-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="08c87-138">categories</span><span class="sxs-lookup"><span data-stu-id="08c87-138">categories</span></span>|<span data-ttu-id="08c87-139">String collection</span><span class="sxs-lookup"><span data-stu-id="08c87-139">String collection</span></span>|<span data-ttu-id="08c87-140">包含用户与项目相关联的类别 (例如，数字转换、石油远程测试机组) 。</span><span class="sxs-lookup"><span data-stu-id="08c87-140">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="08c87-141">客户端</span><span class="sxs-lookup"><span data-stu-id="08c87-141">client</span></span>|[<span data-ttu-id="08c87-142">companyDetail</span><span class="sxs-lookup"><span data-stu-id="08c87-142">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="08c87-143">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="08c87-143">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="08c87-144">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="08c87-144">collaborationTags</span></span>|<span data-ttu-id="08c87-145">字符串集合</span><span class="sxs-lookup"><span data-stu-id="08c87-145">String collection</span></span>|<span data-ttu-id="08c87-146">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="08c87-146">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="08c87-147">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="08c87-147">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="08c87-148">征求</span><span class="sxs-lookup"><span data-stu-id="08c87-148">colleagues</span></span>|<span data-ttu-id="08c87-149">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08c87-149">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="08c87-150">列出也在项目中工作的人员。</span><span class="sxs-lookup"><span data-stu-id="08c87-150">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="08c87-151">介绍</span><span class="sxs-lookup"><span data-stu-id="08c87-151">detail</span></span>|[<span data-ttu-id="08c87-152">positionDetail</span><span class="sxs-lookup"><span data-stu-id="08c87-152">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="08c87-153">包含有关用户在项目上的角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="08c87-153">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="08c87-154">displayName</span><span class="sxs-lookup"><span data-stu-id="08c87-154">displayName</span></span>|<span data-ttu-id="08c87-155">String</span><span class="sxs-lookup"><span data-stu-id="08c87-155">String</span></span>|<span data-ttu-id="08c87-156">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="08c87-156">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="08c87-157">推导</span><span class="sxs-lookup"><span data-stu-id="08c87-157">inference</span></span>|[<span data-ttu-id="08c87-158">inferenceData</span><span class="sxs-lookup"><span data-stu-id="08c87-158">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="08c87-159">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="08c87-159">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="08c87-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="08c87-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="08c87-161">source</span><span class="sxs-lookup"><span data-stu-id="08c87-161">source</span></span>|[<span data-ttu-id="08c87-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="08c87-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="08c87-163">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="08c87-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="08c87-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="08c87-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="08c87-165">人</span><span class="sxs-lookup"><span data-stu-id="08c87-165">sponsors</span></span>|<span data-ttu-id="08c87-166">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08c87-166">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="08c87-167">发起项目的人员或人员。</span><span class="sxs-lookup"><span data-stu-id="08c87-167">The Person or people who sponsored the project.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="08c87-168">关系</span><span class="sxs-lookup"><span data-stu-id="08c87-168">Relationships</span></span>

## <a name="response"></a><span data-ttu-id="08c87-169">响应</span><span class="sxs-lookup"><span data-stu-id="08c87-169">Response</span></span>

<span data-ttu-id="08c87-170">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [projectParticipation](../resources/projectparticipation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08c87-170">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08c87-171">示例</span><span class="sxs-lookup"><span data-stu-id="08c87-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08c87-172">请求</span><span class="sxs-lookup"><span data-stu-id="08c87-172">Request</span></span>

<span data-ttu-id="08c87-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08c87-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08c87-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="08c87-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "department": "Consulting",
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  }
}
```
# <a name="c"></a>[<span data-ttu-id="08c87-175">C#</span><span class="sxs-lookup"><span data-stu-id="08c87-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08c87-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08c87-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08c87-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08c87-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08c87-178">响应</span><span class="sxs-lookup"><span data-stu-id="08c87-178">Response</span></span>

<span data-ttu-id="08c87-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08c87-179">The following is an example of the response.</span></span>

> <span data-ttu-id="08c87-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08c87-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "pronunciation": null,
    "department": "Corporate Marketing",
    "officeLocation": null,
    "address": null,
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": null,
      "address": null,
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "endMonthYear": "datetime-value",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "startMonthYear": "datetime-value",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  },
  "colleagues": null,
  "sponsors": null
}
```
