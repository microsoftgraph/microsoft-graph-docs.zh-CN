---
title: 创建 educationalActivity
description: 创建新的 educationalActivity。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 366417fd6cf8e218bf7fc3a0fe2f14bc9c0ac4d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036938"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="c1102-103">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="c1102-103">Create educationalActivity</span></span>

<span data-ttu-id="c1102-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1102-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1102-105">在用户配置文件中创建新的[educationalActivity。](../resources/educationalactivity.md) [](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="c1102-105">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1102-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1102-106">Permissions</span></span>

<span data-ttu-id="c1102-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1102-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1102-109">Permission type</span></span>                        | <span data-ttu-id="c1102-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1102-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1102-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1102-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1102-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1102-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c1102-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1102-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1102-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1102-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c1102-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1102-115">Application</span></span>                            | <span data-ttu-id="c1102-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1102-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="c1102-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1102-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/educationalActivities
POST /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="c1102-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1102-118">Request headers</span></span>

| <span data-ttu-id="c1102-119">名称</span><span class="sxs-lookup"><span data-stu-id="c1102-119">Name</span></span>           |<span data-ttu-id="c1102-120">说明</span><span class="sxs-lookup"><span data-stu-id="c1102-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c1102-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1102-121">Authorization</span></span>  | <span data-ttu-id="c1102-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1102-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c1102-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1102-124">Content-Type</span></span>   | <span data-ttu-id="c1102-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c1102-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1102-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1102-127">Request body</span></span>

<span data-ttu-id="c1102-128">在请求正文中，提供 [educationalActivity](../resources/educationalactivity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1102-128">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

<span data-ttu-id="c1102-129">下表显示了在用户配置文件中创建新的 [educationalActivity](../resources/educationalactivity.md) 对象时可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="c1102-129">The following table shows the properties that are possible to set when creating a new [educationalActivity](../resources/educationalactivity.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="c1102-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1102-130">Property</span></span>|<span data-ttu-id="c1102-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1102-131">Type</span></span>|<span data-ttu-id="c1102-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1102-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1102-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c1102-133">allowedAudiences</span></span>|<span data-ttu-id="c1102-134">String</span><span class="sxs-lookup"><span data-stu-id="c1102-134">String</span></span>|<span data-ttu-id="c1102-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="c1102-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c1102-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c1102-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c1102-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c1102-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c1102-138">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="c1102-138">completionMonthYear</span></span>|<span data-ttu-id="c1102-139">日期</span><span class="sxs-lookup"><span data-stu-id="c1102-139">Date</span></span>|<span data-ttu-id="c1102-140">用户注册或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="c1102-140">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="c1102-141">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="c1102-141">endMonthYear</span></span>|<span data-ttu-id="c1102-142">日期</span><span class="sxs-lookup"><span data-stu-id="c1102-142">Date</span></span>|<span data-ttu-id="c1102-143">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="c1102-143">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="c1102-144">inference</span><span class="sxs-lookup"><span data-stu-id="c1102-144">inference</span></span>|[<span data-ttu-id="c1102-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c1102-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c1102-146">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="c1102-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c1102-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c1102-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c1102-148">机构</span><span class="sxs-lookup"><span data-stu-id="c1102-148">institution</span></span>|[<span data-ttu-id="c1102-149">institutionData</span><span class="sxs-lookup"><span data-stu-id="c1102-149">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="c1102-150">包含所查看的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c1102-150">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="c1102-151">程序</span><span class="sxs-lookup"><span data-stu-id="c1102-151">program</span></span>|[<span data-ttu-id="c1102-152">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="c1102-152">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="c1102-153">包含有关计划或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="c1102-153">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="c1102-154">source</span><span class="sxs-lookup"><span data-stu-id="c1102-154">source</span></span>|[<span data-ttu-id="c1102-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="c1102-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="c1102-156">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="c1102-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="c1102-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c1102-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c1102-158">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="c1102-158">startMonthYear</span></span>|<span data-ttu-id="c1102-159">日期</span><span class="sxs-lookup"><span data-stu-id="c1102-159">Date</span></span>|<span data-ttu-id="c1102-160">用户对所引用的活动进行跟踪的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="c1102-160">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="c1102-161">响应</span><span class="sxs-lookup"><span data-stu-id="c1102-161">Response</span></span>

<span data-ttu-id="c1102-162">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [educationalActivity](../resources/educationalactivity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1102-162">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1102-163">示例</span><span class="sxs-lookup"><span data-stu-id="c1102-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1102-164">请求</span><span class="sxs-lookup"><span data-stu-id="c1102-164">Request</span></span>

<span data-ttu-id="c1102-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1102-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1102-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1102-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
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
# <a name="c"></a>[<span data-ttu-id="c1102-167">C#</span><span class="sxs-lookup"><span data-stu-id="c1102-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationalactivity-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1102-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1102-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationalactivity-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1102-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1102-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationalactivity-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1102-170">Java</span><span class="sxs-lookup"><span data-stu-id="c1102-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationalactivity-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1102-171">响应</span><span class="sxs-lookup"><span data-stu-id="c1102-171">Response</span></span>

<span data-ttu-id="c1102-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1102-172">The following is an example of the response.</span></span>

> <span data-ttu-id="c1102-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1102-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
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


