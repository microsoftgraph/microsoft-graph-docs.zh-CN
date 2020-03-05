---
title: 更新 projectParticipation 资源类型
description: 更新用户的配置文件中的 projectParticipation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b0aa9353a9e16929bd71f41f5328c0fdaf12c531
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454925"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="b9e5f-103">更新 projectparticipation</span><span class="sxs-lookup"><span data-stu-id="b9e5f-103">Update projectparticipation</span></span>

<span data-ttu-id="b9e5f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b9e5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9e5f-105">更新用户的[配置文件](../resources/profile.md)中的[projectParticipation](../resources/projectParticipation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e5f-106">权限</span><span class="sxs-lookup"><span data-stu-id="b9e5f-106">Permissions</span></span>

<span data-ttu-id="b9e5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9e5f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e5f-109">Permission type</span></span>                        | <span data-ttu-id="b9e5f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e5f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9e5f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e5f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e5f-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b9e5f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e5f-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b9e5f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e5f-115">Application</span></span>                            | <span data-ttu-id="b9e5f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e5f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b9e5f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e5f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9e5f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e5f-118">Request headers</span></span>

| <span data-ttu-id="b9e5f-119">名称</span><span class="sxs-lookup"><span data-stu-id="b9e5f-119">Name</span></span>           |<span data-ttu-id="b9e5f-120">说明</span><span class="sxs-lookup"><span data-stu-id="b9e5f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b9e5f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e5f-121">Authorization</span></span>  | <span data-ttu-id="b9e5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b9e5f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9e5f-124">Content-Type</span></span>   | <span data-ttu-id="b9e5f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b9e5f-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b9e5f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e5f-127">Request body</span></span>

<span data-ttu-id="b9e5f-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b9e5f-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b9e5f-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9e5f-131">属性</span><span class="sxs-lookup"><span data-stu-id="b9e5f-131">Property</span></span>     | <span data-ttu-id="b9e5f-132">类型</span><span class="sxs-lookup"><span data-stu-id="b9e5f-132">Type</span></span>                                                     | <span data-ttu-id="b9e5f-133">说明</span><span class="sxs-lookup"><span data-stu-id="b9e5f-133">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b9e5f-134">categories</span><span class="sxs-lookup"><span data-stu-id="b9e5f-134">categories</span></span>    |<span data-ttu-id="b9e5f-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9e5f-135">String collection</span></span>                                         | <span data-ttu-id="b9e5f-136">包含用户与项目相关联的类别（例如：数字转换、石油远程测试机组）</span><span class="sxs-lookup"><span data-stu-id="b9e5f-136">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="b9e5f-137">客户端</span><span class="sxs-lookup"><span data-stu-id="b9e5f-137">client</span></span>        |[<span data-ttu-id="b9e5f-138">companyDetail</span><span class="sxs-lookup"><span data-stu-id="b9e5f-138">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="b9e5f-139">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-139">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="b9e5f-140">征求</span><span class="sxs-lookup"><span data-stu-id="b9e5f-140">colleagues</span></span>    |<span data-ttu-id="b9e5f-141">[relatedPerson](../resources/relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9e5f-141">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="b9e5f-142">对项目也有效的人员。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-142">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="b9e5f-143">介绍</span><span class="sxs-lookup"><span data-stu-id="b9e5f-143">detail</span></span>        |[<span data-ttu-id="b9e5f-144">positionDetail</span><span class="sxs-lookup"><span data-stu-id="b9e5f-144">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="b9e5f-145">包含有关项目上的用户角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-145">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="b9e5f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b9e5f-146">displayName</span></span>   |<span data-ttu-id="b9e5f-147">String</span><span class="sxs-lookup"><span data-stu-id="b9e5f-147">String</span></span>                                                    | <span data-ttu-id="b9e5f-148">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-148">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="b9e5f-149">人</span><span class="sxs-lookup"><span data-stu-id="b9e5f-149">sponsors</span></span>      |<span data-ttu-id="b9e5f-150">[relatedPerson](../resources/relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9e5f-150">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="b9e5f-151">赞助项目的人员（人员）。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-151">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="b9e5f-152">响应</span><span class="sxs-lookup"><span data-stu-id="b9e5f-152">Response</span></span>

<span data-ttu-id="b9e5f-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[projectParticipation](../resources/projectparticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-153">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9e5f-154">示例</span><span class="sxs-lookup"><span data-stu-id="b9e5f-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9e5f-155">请求</span><span class="sxs-lookup"><span data-stu-id="b9e5f-155">Request</span></span>

<span data-ttu-id="b9e5f-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9e5f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e5f-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9e5f-158">C#</span><span class="sxs-lookup"><span data-stu-id="b9e5f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9e5f-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9e5f-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9e5f-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9e5f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9e5f-161">响应</span><span class="sxs-lookup"><span data-stu-id="b9e5f-161">Response</span></span>

<span data-ttu-id="b9e5f-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-162">The following is an example of the response.</span></span>

> <span data-ttu-id="b9e5f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b9e5f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
