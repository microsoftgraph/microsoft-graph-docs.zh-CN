---
title: 创建 projectParticipation
description: 使用此 API 创建新的 projectParticipation。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7fdfc23831b30495f35f1eb4c4d82e863bba07fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036791"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="8a632-103">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="8a632-103">Create projectParticipation</span></span>

<span data-ttu-id="8a632-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a632-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a632-105">使用此 API 在用户配置文件中创建新的 [projectParticipation](../resources/projectParticipation.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="8a632-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a632-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a632-106">Permissions</span></span>

<span data-ttu-id="8a632-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a632-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a632-109">Permission type</span></span>                        | <span data-ttu-id="8a632-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a632-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8a632-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a632-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a632-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a632-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8a632-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a632-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a632-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a632-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8a632-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a632-115">Application</span></span>                            | <span data-ttu-id="8a632-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a632-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8a632-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a632-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
POST /users/{id | userPrincipalName}/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="8a632-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a632-118">Request headers</span></span>

| <span data-ttu-id="8a632-119">名称</span><span class="sxs-lookup"><span data-stu-id="8a632-119">Name</span></span>           |<span data-ttu-id="8a632-120">说明</span><span class="sxs-lookup"><span data-stu-id="8a632-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="8a632-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a632-121">Authorization</span></span>  | <span data-ttu-id="8a632-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a632-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8a632-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a632-124">Content-Type</span></span>   | <span data-ttu-id="8a632-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8a632-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a632-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a632-127">Request body</span></span>

<span data-ttu-id="8a632-128">在请求正文中，提供 [projectParticipation](../resources/projectparticipation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a632-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

<span data-ttu-id="8a632-129">下表显示了在用户配置文件中创建新的 [projectParticipation](../resources/projectParticipation.md) 对象时可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="8a632-129">The following table shows the properties that are possible to set when you create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="8a632-130">属性</span><span class="sxs-lookup"><span data-stu-id="8a632-130">Property</span></span>|<span data-ttu-id="8a632-131">类型</span><span class="sxs-lookup"><span data-stu-id="8a632-131">Type</span></span>|<span data-ttu-id="8a632-132">说明</span><span class="sxs-lookup"><span data-stu-id="8a632-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a632-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8a632-133">allowedAudiences</span></span>|<span data-ttu-id="8a632-134">String</span><span class="sxs-lookup"><span data-stu-id="8a632-134">String</span></span>|<span data-ttu-id="8a632-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="8a632-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8a632-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8a632-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8a632-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8a632-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8a632-138">categories</span><span class="sxs-lookup"><span data-stu-id="8a632-138">categories</span></span>|<span data-ttu-id="8a632-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a632-139">String collection</span></span>|<span data-ttu-id="8a632-140">包含用户与项目计划关联的类别 (例如，数字转换、国家/) 。</span><span class="sxs-lookup"><span data-stu-id="8a632-140">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="8a632-141">client</span><span class="sxs-lookup"><span data-stu-id="8a632-141">client</span></span>|[<span data-ttu-id="8a632-142">companyDetail</span><span class="sxs-lookup"><span data-stu-id="8a632-142">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="8a632-143">包含有关项目用于的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8a632-143">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="8a632-144">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="8a632-144">collaborationTags</span></span>|<span data-ttu-id="8a632-145">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8a632-145">String collection</span></span>|<span data-ttu-id="8a632-146">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="8a632-146">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="8a632-147">集合中允许的值为 `askMeAbout` `ableToMentor` ：、、、。 `wantsToLearn` `wantsToImprove`</span><span class="sxs-lookup"><span data-stu-id="8a632-147">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="8a632-148">同事</span><span class="sxs-lookup"><span data-stu-id="8a632-148">colleagues</span></span>|<span data-ttu-id="8a632-149">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a632-149">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="8a632-150">列出同样从事项目工作的人。</span><span class="sxs-lookup"><span data-stu-id="8a632-150">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="8a632-151">detail</span><span class="sxs-lookup"><span data-stu-id="8a632-151">detail</span></span>|[<span data-ttu-id="8a632-152">positionDetail</span><span class="sxs-lookup"><span data-stu-id="8a632-152">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="8a632-153">包含有关用户在项目上的角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8a632-153">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="8a632-154">displayName</span><span class="sxs-lookup"><span data-stu-id="8a632-154">displayName</span></span>|<span data-ttu-id="8a632-155">String</span><span class="sxs-lookup"><span data-stu-id="8a632-155">String</span></span>|<span data-ttu-id="8a632-156">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="8a632-156">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="8a632-157">inference</span><span class="sxs-lookup"><span data-stu-id="8a632-157">inference</span></span>|[<span data-ttu-id="8a632-158">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8a632-158">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8a632-159">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="8a632-159">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8a632-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8a632-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a632-161">source</span><span class="sxs-lookup"><span data-stu-id="8a632-161">source</span></span>|[<span data-ttu-id="8a632-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8a632-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8a632-163">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="8a632-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8a632-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8a632-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a632-165">发起人</span><span class="sxs-lookup"><span data-stu-id="8a632-165">sponsors</span></span>|<span data-ttu-id="8a632-166">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a632-166">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="8a632-167">为项目提供赞助的一个或多个人员。</span><span class="sxs-lookup"><span data-stu-id="8a632-167">The Person or people who sponsored the project.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="8a632-168">关系</span><span class="sxs-lookup"><span data-stu-id="8a632-168">Relationships</span></span>

## <a name="response"></a><span data-ttu-id="8a632-169">响应</span><span class="sxs-lookup"><span data-stu-id="8a632-169">Response</span></span>

<span data-ttu-id="8a632-170">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和一个新的 [projectParticipation](../resources/projectparticipation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a632-170">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a632-171">示例</span><span class="sxs-lookup"><span data-stu-id="8a632-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a632-172">请求</span><span class="sxs-lookup"><span data-stu-id="8a632-172">Request</span></span>

<span data-ttu-id="8a632-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a632-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a632-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a632-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8a632-175">C#</span><span class="sxs-lookup"><span data-stu-id="8a632-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a632-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a632-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a632-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a632-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a632-178">Java</span><span class="sxs-lookup"><span data-stu-id="8a632-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-projectparticipation-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a632-179">响应</span><span class="sxs-lookup"><span data-stu-id="8a632-179">Response</span></span>

<span data-ttu-id="8a632-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a632-180">The following is an example of the response.</span></span>

> <span data-ttu-id="8a632-181">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8a632-181">**Note:** The response object shown here might be shortened for readability.</span></span>

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


