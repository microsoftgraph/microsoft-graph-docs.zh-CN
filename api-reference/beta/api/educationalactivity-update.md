---
title: 更新 educationalactivity
description: 更新 educationalActivity 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: baf9164dba41a70d8603d6c26cbae7f9bedc1e65
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199527"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="9ed38-103">更新 educationalactivity</span><span class="sxs-lookup"><span data-stu-id="9ed38-103">Update educationalactivity</span></span>

<span data-ttu-id="9ed38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ed38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed38-105">更新用户的[配置文件](../resources/profile.md)中的[educationalActivity](../resources/educationalactivity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ed38-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed38-106">权限</span><span class="sxs-lookup"><span data-stu-id="9ed38-106">Permissions</span></span>

<span data-ttu-id="9ed38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ed38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ed38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ed38-109">Permission type</span></span>                        | <span data-ttu-id="9ed38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ed38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ed38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ed38-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9ed38-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9ed38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed38-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9ed38-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9ed38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ed38-115">Application</span></span>                            | <span data-ttu-id="9ed38-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed38-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9ed38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ed38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="9ed38-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ed38-118">Request headers</span></span>

| <span data-ttu-id="9ed38-119">名称</span><span class="sxs-lookup"><span data-stu-id="9ed38-119">Name</span></span>           |<span data-ttu-id="9ed38-120">说明</span><span class="sxs-lookup"><span data-stu-id="9ed38-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9ed38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed38-121">Authorization</span></span>  | <span data-ttu-id="9ed38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ed38-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9ed38-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ed38-124">Content-Type</span></span>   | <span data-ttu-id="9ed38-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9ed38-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed38-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ed38-127">Request body</span></span>

<span data-ttu-id="9ed38-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9ed38-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9ed38-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9ed38-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9ed38-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9ed38-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ed38-131">属性</span><span class="sxs-lookup"><span data-stu-id="9ed38-131">Property</span></span>           | <span data-ttu-id="9ed38-132">类型</span><span class="sxs-lookup"><span data-stu-id="9ed38-132">Type</span></span>                                                                  | <span data-ttu-id="9ed38-133">说明</span><span class="sxs-lookup"><span data-stu-id="9ed38-133">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="9ed38-134">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="9ed38-134">completionMonthYear</span></span> |<span data-ttu-id="9ed38-135">日期</span><span class="sxs-lookup"><span data-stu-id="9ed38-135">Date</span></span>                                                                   | <span data-ttu-id="9ed38-136">用户逐步或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="9ed38-136">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="9ed38-137">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="9ed38-137">endMonthYear</span></span>        |<span data-ttu-id="9ed38-138">日期</span><span class="sxs-lookup"><span data-stu-id="9ed38-138">Date</span></span>                                                                   | <span data-ttu-id="9ed38-139">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="9ed38-139">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="9ed38-140">机构</span><span class="sxs-lookup"><span data-stu-id="9ed38-140">institution</span></span>         |[<span data-ttu-id="9ed38-141">institutionData</span><span class="sxs-lookup"><span data-stu-id="9ed38-141">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="9ed38-142">包含在上研究的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9ed38-142">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="9ed38-143">主程序</span><span class="sxs-lookup"><span data-stu-id="9ed38-143">program</span></span>             |[<span data-ttu-id="9ed38-144">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="9ed38-144">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="9ed38-145">包含有关程序或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="9ed38-145">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="9ed38-146">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="9ed38-146">startMonthYear</span></span>      |<span data-ttu-id="9ed38-147">日期</span><span class="sxs-lookup"><span data-stu-id="9ed38-147">Date</span></span>                                                                   | <span data-ttu-id="9ed38-148">用户 commenced 引用的活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="9ed38-148">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="9ed38-149">响应</span><span class="sxs-lookup"><span data-stu-id="9ed38-149">Response</span></span>

<span data-ttu-id="9ed38-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ed38-150">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ed38-151">示例</span><span class="sxs-lookup"><span data-stu-id="9ed38-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ed38-152">请求</span><span class="sxs-lookup"><span data-stu-id="9ed38-152">Request</span></span>

<span data-ttu-id="9ed38-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed38-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed38-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed38-154">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="9ed38-155">C#</span><span class="sxs-lookup"><span data-stu-id="9ed38-155">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed38-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed38-156">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed38-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed38-157">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9ed38-158">响应</span><span class="sxs-lookup"><span data-stu-id="9ed38-158">Response</span></span>

<span data-ttu-id="9ed38-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed38-159">The following is an example of the response.</span></span>

> <span data-ttu-id="9ed38-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ed38-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
