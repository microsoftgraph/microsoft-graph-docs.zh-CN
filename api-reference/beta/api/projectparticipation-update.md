---
title: 更新 projectParticipation 资源类型
description: 更新用户的配置文件中的 projectParticipation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b18aeb9e56eb79ea2c6d2ce4b0b0160c71c47595
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997675"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="439cd-103">更新 projectparticipation</span><span class="sxs-lookup"><span data-stu-id="439cd-103">Update projectparticipation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="439cd-104">更新用户的[配置文件](../resources/profile.md)中的[projectParticipation](../resources/projectParticipation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="439cd-104">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="439cd-105">权限</span><span class="sxs-lookup"><span data-stu-id="439cd-105">Permissions</span></span>

<span data-ttu-id="439cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="439cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="439cd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="439cd-108">Permission type</span></span>                        | <span data-ttu-id="439cd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="439cd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="439cd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="439cd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="439cd-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="439cd-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="439cd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="439cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="439cd-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="439cd-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="439cd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="439cd-114">Application</span></span>                            | <span data-ttu-id="439cd-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="439cd-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="439cd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="439cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="439cd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="439cd-117">Request headers</span></span>

| <span data-ttu-id="439cd-118">名称</span><span class="sxs-lookup"><span data-stu-id="439cd-118">Name</span></span>           |<span data-ttu-id="439cd-119">说明</span><span class="sxs-lookup"><span data-stu-id="439cd-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="439cd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="439cd-120">Authorization</span></span>  | <span data-ttu-id="439cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="439cd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="439cd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="439cd-123">Content-Type</span></span>   | <span data-ttu-id="439cd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="439cd-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="439cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="439cd-126">Request body</span></span>

<span data-ttu-id="439cd-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="439cd-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="439cd-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="439cd-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="439cd-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="439cd-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="439cd-130">属性</span><span class="sxs-lookup"><span data-stu-id="439cd-130">Property</span></span>     | <span data-ttu-id="439cd-131">类型</span><span class="sxs-lookup"><span data-stu-id="439cd-131">Type</span></span>                                                     | <span data-ttu-id="439cd-132">说明</span><span class="sxs-lookup"><span data-stu-id="439cd-132">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="439cd-133">categories</span><span class="sxs-lookup"><span data-stu-id="439cd-133">categories</span></span>    |<span data-ttu-id="439cd-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="439cd-134">String collection</span></span>                                         | <span data-ttu-id="439cd-135">包含用户与项目相关联的类别（例如：数字转换、石油远程测试机组）</span><span class="sxs-lookup"><span data-stu-id="439cd-135">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="439cd-136">客户端</span><span class="sxs-lookup"><span data-stu-id="439cd-136">client</span></span>        |[<span data-ttu-id="439cd-137">companyDetail</span><span class="sxs-lookup"><span data-stu-id="439cd-137">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="439cd-138">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="439cd-138">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="439cd-139">征求</span><span class="sxs-lookup"><span data-stu-id="439cd-139">colleagues</span></span>    |<span data-ttu-id="439cd-140">[relatedPerson](../resources/relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="439cd-140">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="439cd-141">对项目也有效的人员。</span><span class="sxs-lookup"><span data-stu-id="439cd-141">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="439cd-142">介绍</span><span class="sxs-lookup"><span data-stu-id="439cd-142">detail</span></span>        |[<span data-ttu-id="439cd-143">positionDetail</span><span class="sxs-lookup"><span data-stu-id="439cd-143">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="439cd-144">包含有关项目上的用户角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="439cd-144">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="439cd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="439cd-145">displayName</span></span>   |<span data-ttu-id="439cd-146">String</span><span class="sxs-lookup"><span data-stu-id="439cd-146">String</span></span>                                                    | <span data-ttu-id="439cd-147">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="439cd-147">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="439cd-148">人</span><span class="sxs-lookup"><span data-stu-id="439cd-148">sponsors</span></span>      |<span data-ttu-id="439cd-149">[relatedPerson](../resources/relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="439cd-149">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="439cd-150">赞助项目的人员（人员）。</span><span class="sxs-lookup"><span data-stu-id="439cd-150">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="439cd-151">响应</span><span class="sxs-lookup"><span data-stu-id="439cd-151">Response</span></span>

<span data-ttu-id="439cd-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[projectParticipation](../resources/projectparticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="439cd-152">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="439cd-153">示例</span><span class="sxs-lookup"><span data-stu-id="439cd-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="439cd-154">请求</span><span class="sxs-lookup"><span data-stu-id="439cd-154">Request</span></span>

<span data-ttu-id="439cd-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="439cd-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="439cd-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="439cd-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="439cd-157">C#</span><span class="sxs-lookup"><span data-stu-id="439cd-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="439cd-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="439cd-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="439cd-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="439cd-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="439cd-160">响应</span><span class="sxs-lookup"><span data-stu-id="439cd-160">Response</span></span>

<span data-ttu-id="439cd-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="439cd-161">The following is an example of the response.</span></span>

> <span data-ttu-id="439cd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="439cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update projectparticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
