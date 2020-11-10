---
title: 创建 educationalActivity
description: 创建新的 educationalActivity。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 39805d864a81289fc74391db17f765b40299e3df
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972943"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="54fc1-103">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="54fc1-103">Create educationalActivity</span></span>

<span data-ttu-id="54fc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54fc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fc1-105">在用户的[配置文件](../resources/profile.md)中创建新的[educationalActivity](../resources/educationalactivity.md) 。</span><span class="sxs-lookup"><span data-stu-id="54fc1-105">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="54fc1-106">权限</span><span class="sxs-lookup"><span data-stu-id="54fc1-106">Permissions</span></span>

<span data-ttu-id="54fc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54fc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54fc1-109">Permission type</span></span>                        | <span data-ttu-id="54fc1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54fc1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54fc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54fc1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54fc1-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="54fc1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="54fc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54fc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54fc1-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="54fc1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="54fc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="54fc1-115">Application</span></span>                            | <span data-ttu-id="54fc1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54fc1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="54fc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54fc1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
POST /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="54fc1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="54fc1-118">Request headers</span></span>

| <span data-ttu-id="54fc1-119">名称</span><span class="sxs-lookup"><span data-stu-id="54fc1-119">Name</span></span>           |<span data-ttu-id="54fc1-120">说明</span><span class="sxs-lookup"><span data-stu-id="54fc1-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="54fc1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54fc1-121">Authorization</span></span>  | <span data-ttu-id="54fc1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54fc1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="54fc1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54fc1-124">Content-Type</span></span>   | <span data-ttu-id="54fc1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="54fc1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54fc1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54fc1-127">Request body</span></span>

<span data-ttu-id="54fc1-128">在请求正文中，提供 [educationalActivity](../resources/educationalactivity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54fc1-128">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

<span data-ttu-id="54fc1-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[educationalActivity](../resources/educationalactivity.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="54fc1-129">The following table shows the properties that are possible to set when creating a new [educationalActivity](../resources/educationalactivity.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="54fc1-130">属性</span><span class="sxs-lookup"><span data-stu-id="54fc1-130">Property</span></span>|<span data-ttu-id="54fc1-131">类型</span><span class="sxs-lookup"><span data-stu-id="54fc1-131">Type</span></span>|<span data-ttu-id="54fc1-132">说明</span><span class="sxs-lookup"><span data-stu-id="54fc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54fc1-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="54fc1-133">allowedAudiences</span></span>|<span data-ttu-id="54fc1-134">String</span><span class="sxs-lookup"><span data-stu-id="54fc1-134">String</span></span>|<span data-ttu-id="54fc1-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="54fc1-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="54fc1-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="54fc1-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="54fc1-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="54fc1-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="54fc1-138">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="54fc1-138">completionMonthYear</span></span>|<span data-ttu-id="54fc1-139">日期</span><span class="sxs-lookup"><span data-stu-id="54fc1-139">Date</span></span>|<span data-ttu-id="54fc1-140">用户逐步或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="54fc1-140">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="54fc1-141">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="54fc1-141">endMonthYear</span></span>|<span data-ttu-id="54fc1-142">日期</span><span class="sxs-lookup"><span data-stu-id="54fc1-142">Date</span></span>|<span data-ttu-id="54fc1-143">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="54fc1-143">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="54fc1-144">推导</span><span class="sxs-lookup"><span data-stu-id="54fc1-144">inference</span></span>|[<span data-ttu-id="54fc1-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="54fc1-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="54fc1-146">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="54fc1-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="54fc1-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="54fc1-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="54fc1-148">机构</span><span class="sxs-lookup"><span data-stu-id="54fc1-148">institution</span></span>|[<span data-ttu-id="54fc1-149">institutionData</span><span class="sxs-lookup"><span data-stu-id="54fc1-149">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="54fc1-150">包含在上研究的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="54fc1-150">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="54fc1-151">主程序</span><span class="sxs-lookup"><span data-stu-id="54fc1-151">program</span></span>|[<span data-ttu-id="54fc1-152">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="54fc1-152">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="54fc1-153">包含有关程序或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="54fc1-153">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="54fc1-154">source</span><span class="sxs-lookup"><span data-stu-id="54fc1-154">source</span></span>|[<span data-ttu-id="54fc1-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="54fc1-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="54fc1-156">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="54fc1-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="54fc1-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="54fc1-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="54fc1-158">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="54fc1-158">startMonthYear</span></span>|<span data-ttu-id="54fc1-159">日期</span><span class="sxs-lookup"><span data-stu-id="54fc1-159">Date</span></span>|<span data-ttu-id="54fc1-160">用户 commenced 引用的活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="54fc1-160">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="54fc1-161">响应</span><span class="sxs-lookup"><span data-stu-id="54fc1-161">Response</span></span>

<span data-ttu-id="54fc1-162">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [educationalActivity](../resources/educationalactivity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54fc1-162">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54fc1-163">示例</span><span class="sxs-lookup"><span data-stu-id="54fc1-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54fc1-164">请求</span><span class="sxs-lookup"><span data-stu-id="54fc1-164">Request</span></span>

<span data-ttu-id="54fc1-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54fc1-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54fc1-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="54fc1-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="54fc1-167">C#</span><span class="sxs-lookup"><span data-stu-id="54fc1-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationalactivity-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54fc1-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54fc1-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationalactivity-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54fc1-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54fc1-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationalactivity-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54fc1-170">Java</span><span class="sxs-lookup"><span data-stu-id="54fc1-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationalactivity-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54fc1-171">响应</span><span class="sxs-lookup"><span data-stu-id="54fc1-171">Response</span></span>

<span data-ttu-id="54fc1-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54fc1-172">The following is an example of the response.</span></span>

> <span data-ttu-id="54fc1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="54fc1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


