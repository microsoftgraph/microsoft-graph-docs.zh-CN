---
title: 更新 projectParticipation 资源类型
description: 更新用户的配置文件中的 projectParticipation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c44ab0be22873ae37120d99ef86b70df586eb918
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010598"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="1a494-103">更新 projectparticipation</span><span class="sxs-lookup"><span data-stu-id="1a494-103">Update projectparticipation</span></span>

<span data-ttu-id="1a494-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a494-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a494-105">更新用户的[配置文件](../resources/profile.md)中的[projectParticipation](../resources/projectParticipation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a494-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a494-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a494-106">Permissions</span></span>

<span data-ttu-id="1a494-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a494-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a494-109">Permission type</span></span>                        | <span data-ttu-id="1a494-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a494-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a494-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a494-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a494-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1a494-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a494-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a494-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a494-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1a494-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a494-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a494-115">Application</span></span>                            | <span data-ttu-id="1a494-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a494-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1a494-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a494-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a494-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a494-118">Request headers</span></span>

| <span data-ttu-id="1a494-119">名称</span><span class="sxs-lookup"><span data-stu-id="1a494-119">Name</span></span>           |<span data-ttu-id="1a494-120">说明</span><span class="sxs-lookup"><span data-stu-id="1a494-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1a494-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a494-121">Authorization</span></span>  | <span data-ttu-id="1a494-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a494-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1a494-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a494-124">Content-Type</span></span>   | <span data-ttu-id="1a494-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1a494-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a494-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a494-127">Request body</span></span>

<span data-ttu-id="1a494-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="1a494-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1a494-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="1a494-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1a494-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1a494-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="1a494-131">属性</span><span class="sxs-lookup"><span data-stu-id="1a494-131">Property</span></span>|<span data-ttu-id="1a494-132">类型</span><span class="sxs-lookup"><span data-stu-id="1a494-132">Type</span></span>|<span data-ttu-id="1a494-133">说明</span><span class="sxs-lookup"><span data-stu-id="1a494-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a494-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1a494-134">allowedAudiences</span></span>|<span data-ttu-id="1a494-135">String</span><span class="sxs-lookup"><span data-stu-id="1a494-135">String</span></span>|<span data-ttu-id="1a494-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="1a494-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1a494-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="1a494-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1a494-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1a494-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1a494-139">类别</span><span class="sxs-lookup"><span data-stu-id="1a494-139">categories</span></span>|<span data-ttu-id="1a494-140">String collection</span><span class="sxs-lookup"><span data-stu-id="1a494-140">String collection</span></span>|<span data-ttu-id="1a494-141">包含用户与项目相关联的类别 (例如，数字转换、石油远程测试机组) 。</span><span class="sxs-lookup"><span data-stu-id="1a494-141">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="1a494-142">客户端</span><span class="sxs-lookup"><span data-stu-id="1a494-142">client</span></span>|[<span data-ttu-id="1a494-143">companyDetail</span><span class="sxs-lookup"><span data-stu-id="1a494-143">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="1a494-144">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1a494-144">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="1a494-145">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="1a494-145">collaborationTags</span></span>|<span data-ttu-id="1a494-146">String collection</span><span class="sxs-lookup"><span data-stu-id="1a494-146">String collection</span></span>|<span data-ttu-id="1a494-147">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="1a494-147">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="1a494-148">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="1a494-148">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="1a494-149">征求</span><span class="sxs-lookup"><span data-stu-id="1a494-149">colleagues</span></span>|<span data-ttu-id="1a494-150">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a494-150">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="1a494-151">列出也在项目中工作的人员。</span><span class="sxs-lookup"><span data-stu-id="1a494-151">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="1a494-152">介绍</span><span class="sxs-lookup"><span data-stu-id="1a494-152">detail</span></span>|[<span data-ttu-id="1a494-153">positionDetail</span><span class="sxs-lookup"><span data-stu-id="1a494-153">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="1a494-154">包含有关用户在项目上的角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1a494-154">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="1a494-155">displayName</span><span class="sxs-lookup"><span data-stu-id="1a494-155">displayName</span></span>|<span data-ttu-id="1a494-156">String</span><span class="sxs-lookup"><span data-stu-id="1a494-156">String</span></span>|<span data-ttu-id="1a494-157">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="1a494-157">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="1a494-158">推导</span><span class="sxs-lookup"><span data-stu-id="1a494-158">inference</span></span>|[<span data-ttu-id="1a494-159">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1a494-159">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1a494-160">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="1a494-160">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1a494-161">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="1a494-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1a494-162">人</span><span class="sxs-lookup"><span data-stu-id="1a494-162">sponsors</span></span>|<span data-ttu-id="1a494-163">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a494-163">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="1a494-164">发起项目的人员或人员。</span><span class="sxs-lookup"><span data-stu-id="1a494-164">The Person or people who sponsored the project.</span></span>    |

## <a name="response"></a><span data-ttu-id="1a494-165">响应</span><span class="sxs-lookup"><span data-stu-id="1a494-165">Response</span></span>

<span data-ttu-id="1a494-166">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [projectParticipation](../resources/projectparticipation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a494-166">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a494-167">示例</span><span class="sxs-lookup"><span data-stu-id="1a494-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a494-168">请求</span><span class="sxs-lookup"><span data-stu-id="1a494-168">Request</span></span>

<span data-ttu-id="1a494-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a494-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a494-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a494-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "allowedAudiences": "organization",
  "client": {
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1a494-171">C#</span><span class="sxs-lookup"><span data-stu-id="1a494-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a494-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a494-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a494-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a494-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a494-174">响应</span><span class="sxs-lookup"><span data-stu-id="1a494-174">Response</span></span>

<span data-ttu-id="1a494-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a494-175">The following is an example of the response.</span></span>

> <span data-ttu-id="1a494-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1a494-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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


