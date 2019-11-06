---
title: 更新 educationalactivity
description: 更新 educationalactivity 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 68d9c6d2499b3610361ab0fdc2b78c188853b65b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994753"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="71bf8-103">更新 educationalactivity</span><span class="sxs-lookup"><span data-stu-id="71bf8-103">Update educationalactivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71bf8-104">更新用户的[配置文件](../resources/profile.md)中的[educationalActivity](../resources/educationalactivity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71bf8-104">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71bf8-105">权限</span><span class="sxs-lookup"><span data-stu-id="71bf8-105">Permissions</span></span>

<span data-ttu-id="71bf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71bf8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="71bf8-108">Permission type</span></span>                        | <span data-ttu-id="71bf8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71bf8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71bf8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71bf8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="71bf8-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="71bf8-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="71bf8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71bf8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bf8-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="71bf8-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="71bf8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="71bf8-114">Application</span></span>                            | <span data-ttu-id="71bf8-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bf8-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="71bf8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71bf8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="71bf8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="71bf8-117">Request headers</span></span>

| <span data-ttu-id="71bf8-118">名称</span><span class="sxs-lookup"><span data-stu-id="71bf8-118">Name</span></span>           |<span data-ttu-id="71bf8-119">说明</span><span class="sxs-lookup"><span data-stu-id="71bf8-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="71bf8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bf8-120">Authorization</span></span>  | <span data-ttu-id="71bf8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71bf8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="71bf8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71bf8-123">Content-Type</span></span>   | <span data-ttu-id="71bf8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="71bf8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71bf8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71bf8-126">Request body</span></span>

<span data-ttu-id="71bf8-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="71bf8-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="71bf8-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="71bf8-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="71bf8-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="71bf8-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71bf8-130">属性</span><span class="sxs-lookup"><span data-stu-id="71bf8-130">Property</span></span>           | <span data-ttu-id="71bf8-131">类型</span><span class="sxs-lookup"><span data-stu-id="71bf8-131">Type</span></span>                                                                  | <span data-ttu-id="71bf8-132">说明</span><span class="sxs-lookup"><span data-stu-id="71bf8-132">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="71bf8-133">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="71bf8-133">completionMonthYear</span></span> |<span data-ttu-id="71bf8-134">日期</span><span class="sxs-lookup"><span data-stu-id="71bf8-134">Date</span></span>                                                                   | <span data-ttu-id="71bf8-135">用户逐步或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="71bf8-135">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="71bf8-136">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="71bf8-136">endMonthYear</span></span>        |<span data-ttu-id="71bf8-137">日期</span><span class="sxs-lookup"><span data-stu-id="71bf8-137">Date</span></span>                                                                   | <span data-ttu-id="71bf8-138">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="71bf8-138">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="71bf8-139">机构</span><span class="sxs-lookup"><span data-stu-id="71bf8-139">institution</span></span>         |[<span data-ttu-id="71bf8-140">institutionData</span><span class="sxs-lookup"><span data-stu-id="71bf8-140">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="71bf8-141">包含在上研究的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="71bf8-141">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="71bf8-142">主程序</span><span class="sxs-lookup"><span data-stu-id="71bf8-142">program</span></span>             |[<span data-ttu-id="71bf8-143">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="71bf8-143">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="71bf8-144">包含有关程序或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="71bf8-144">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="71bf8-145">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="71bf8-145">startMonthYear</span></span>      |<span data-ttu-id="71bf8-146">日期</span><span class="sxs-lookup"><span data-stu-id="71bf8-146">Date</span></span>                                                                   | <span data-ttu-id="71bf8-147">用户 commenced 引用的活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="71bf8-147">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="71bf8-148">响应</span><span class="sxs-lookup"><span data-stu-id="71bf8-148">Response</span></span>

<span data-ttu-id="71bf8-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71bf8-149">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71bf8-150">示例</span><span class="sxs-lookup"><span data-stu-id="71bf8-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71bf8-151">请求</span><span class="sxs-lookup"><span data-stu-id="71bf8-151">Request</span></span>

<span data-ttu-id="71bf8-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71bf8-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="71bf8-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="71bf8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71bf8-154">C#</span><span class="sxs-lookup"><span data-stu-id="71bf8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71bf8-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71bf8-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71bf8-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71bf8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71bf8-157">响应</span><span class="sxs-lookup"><span data-stu-id="71bf8-157">Response</span></span>

<span data-ttu-id="71bf8-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71bf8-158">The following is an example of the response.</span></span>

> <span data-ttu-id="71bf8-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71bf8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationalactivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
