---
title: 更新教育活动
description: 更新 educationalActivity 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7f59b6ef2b5bebb2369a3cbd44baaae6ca209b97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044478"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="bf77d-103">更新教育活动</span><span class="sxs-lookup"><span data-stu-id="bf77d-103">Update educationalactivity</span></span>

<span data-ttu-id="bf77d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf77d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf77d-105">更新用户配置文件 [中的 educationalActivity](../resources/educationalactivity.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="bf77d-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf77d-106">权限</span><span class="sxs-lookup"><span data-stu-id="bf77d-106">Permissions</span></span>

<span data-ttu-id="bf77d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf77d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf77d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf77d-109">Permission type</span></span>                        | <span data-ttu-id="bf77d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf77d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bf77d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf77d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf77d-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf77d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bf77d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf77d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf77d-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf77d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bf77d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf77d-115">Application</span></span>                            | <span data-ttu-id="bf77d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf77d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bf77d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf77d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id}
PATCH /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf77d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf77d-118">Request headers</span></span>

| <span data-ttu-id="bf77d-119">名称</span><span class="sxs-lookup"><span data-stu-id="bf77d-119">Name</span></span>           |<span data-ttu-id="bf77d-120">说明</span><span class="sxs-lookup"><span data-stu-id="bf77d-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bf77d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf77d-121">Authorization</span></span>  | <span data-ttu-id="bf77d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf77d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bf77d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf77d-124">Content-Type</span></span>   | <span data-ttu-id="bf77d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf77d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf77d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf77d-127">Request body</span></span>

<span data-ttu-id="bf77d-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bf77d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bf77d-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bf77d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bf77d-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bf77d-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="bf77d-131">属性</span><span class="sxs-lookup"><span data-stu-id="bf77d-131">Property</span></span>|<span data-ttu-id="bf77d-132">类型</span><span class="sxs-lookup"><span data-stu-id="bf77d-132">Type</span></span>|<span data-ttu-id="bf77d-133">说明</span><span class="sxs-lookup"><span data-stu-id="bf77d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf77d-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="bf77d-134">allowedAudiences</span></span>|<span data-ttu-id="bf77d-135">String</span><span class="sxs-lookup"><span data-stu-id="bf77d-135">String</span></span>|<span data-ttu-id="bf77d-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="bf77d-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="bf77d-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bf77d-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="bf77d-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bf77d-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bf77d-139">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="bf77d-139">completionMonthYear</span></span>|<span data-ttu-id="bf77d-140">日期</span><span class="sxs-lookup"><span data-stu-id="bf77d-140">Date</span></span>|<span data-ttu-id="bf77d-141">用户注册或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="bf77d-141">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="bf77d-142">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="bf77d-142">endMonthYear</span></span>|<span data-ttu-id="bf77d-143">日期</span><span class="sxs-lookup"><span data-stu-id="bf77d-143">Date</span></span>|<span data-ttu-id="bf77d-144">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="bf77d-144">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="bf77d-145">inference</span><span class="sxs-lookup"><span data-stu-id="bf77d-145">inference</span></span>|[<span data-ttu-id="bf77d-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="bf77d-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="bf77d-147">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf77d-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="bf77d-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bf77d-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bf77d-149">机构</span><span class="sxs-lookup"><span data-stu-id="bf77d-149">institution</span></span>|[<span data-ttu-id="bf77d-150">institutionData</span><span class="sxs-lookup"><span data-stu-id="bf77d-150">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="bf77d-151">包含所查看的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf77d-151">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="bf77d-152">程序</span><span class="sxs-lookup"><span data-stu-id="bf77d-152">program</span></span>|[<span data-ttu-id="bf77d-153">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bf77d-153">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="bf77d-154">包含有关计划或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="bf77d-154">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="bf77d-155">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="bf77d-155">startMonthYear</span></span>|<span data-ttu-id="bf77d-156">日期</span><span class="sxs-lookup"><span data-stu-id="bf77d-156">Date</span></span>|<span data-ttu-id="bf77d-157">用户对所引用的活动进行跟踪的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="bf77d-157">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="bf77d-158">响应</span><span class="sxs-lookup"><span data-stu-id="bf77d-158">Response</span></span>

<span data-ttu-id="bf77d-159">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` [的 educationalActivity](../resources/educationalactivity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf77d-159">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf77d-160">示例</span><span class="sxs-lookup"><span data-stu-id="bf77d-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf77d-161">请求</span><span class="sxs-lookup"><span data-stu-id="bf77d-161">Request</span></span>

<span data-ttu-id="bf77d-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf77d-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf77d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf77d-163">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
Content-type: application/json

{
  "institution": {
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    }
  }
}
```

# <a name="c"></a>[<span data-ttu-id="bf77d-164">C#</span><span class="sxs-lookup"><span data-stu-id="bf77d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf77d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf77d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf77d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf77d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf77d-167">Java</span><span class="sxs-lookup"><span data-stu-id="bf77d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bf77d-168">响应</span><span class="sxs-lookup"><span data-stu-id="bf77d-168">Response</span></span>

<span data-ttu-id="bf77d-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf77d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="bf77d-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bf77d-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```


