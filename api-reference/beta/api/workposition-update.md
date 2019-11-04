---
title: 更新 workPosition
description: 更新用户的配置文件中的 workPosition 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 93da22ac78163dbfc9b4eb48f3696a73f1870f16
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938097"
---
# <a name="update-workposition"></a><span data-ttu-id="673e8-103">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="673e8-103">Update workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="673e8-104">更新用户的[配置文件](../resources/profile.md)中的[workPosition](../resources/workposition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="673e8-104">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="673e8-105">权限</span><span class="sxs-lookup"><span data-stu-id="673e8-105">Permissions</span></span>

<span data-ttu-id="673e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="673e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="673e8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="673e8-108">Permission type</span></span>                        | <span data-ttu-id="673e8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="673e8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="673e8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="673e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="673e8-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="673e8-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="673e8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="673e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="673e8-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="673e8-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="673e8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="673e8-114">Application</span></span>                            | <span data-ttu-id="673e8-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673e8-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="673e8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="673e8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="673e8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="673e8-117">Request headers</span></span>

| <span data-ttu-id="673e8-118">名称</span><span class="sxs-lookup"><span data-stu-id="673e8-118">Name</span></span>           |<span data-ttu-id="673e8-119">说明</span><span class="sxs-lookup"><span data-stu-id="673e8-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="673e8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="673e8-120">Authorization</span></span>  | <span data-ttu-id="673e8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="673e8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="673e8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="673e8-123">Content-Type</span></span>   | <span data-ttu-id="673e8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="673e8-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="673e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="673e8-126">Request body</span></span>

<span data-ttu-id="673e8-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="673e8-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="673e8-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="673e8-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="673e8-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="673e8-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="673e8-130">属性</span><span class="sxs-lookup"><span data-stu-id="673e8-130">Property</span></span>     | <span data-ttu-id="673e8-131">类型</span><span class="sxs-lookup"><span data-stu-id="673e8-131">Type</span></span>                                        | <span data-ttu-id="673e8-132">描述</span><span class="sxs-lookup"><span data-stu-id="673e8-132">Description</span></span>                                                                                                 |
|:-------------|:--------------------------------------------|:------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="673e8-133">类别</span><span class="sxs-lookup"><span data-stu-id="673e8-133">categories</span></span>|<span data-ttu-id="673e8-134">String collection</span><span class="sxs-lookup"><span data-stu-id="673e8-134">String collection</span></span>                                | <span data-ttu-id="673e8-135">包含用户与位置相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="673e8-135">Contains categories a user has associated with the position.</span></span> <span data-ttu-id="673e8-136">（例如：数字转换、ms graph、人员）</span><span class="sxs-lookup"><span data-stu-id="673e8-136">(eg: digital transformation, ms graph, people)</span></span> |
|<span data-ttu-id="673e8-137">介绍</span><span class="sxs-lookup"><span data-stu-id="673e8-137">detail</span></span>    |[<span data-ttu-id="673e8-138">positionDetail</span><span class="sxs-lookup"><span data-stu-id="673e8-138">positionDetail</span></span>](../resources/positiondetail.md) | <span data-ttu-id="673e8-139">包含有关用户工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="673e8-139">Contains detail about a users work position.</span></span>                                                                |

## <a name="response"></a><span data-ttu-id="673e8-140">响应</span><span class="sxs-lookup"><span data-stu-id="673e8-140">Response</span></span>

<span data-ttu-id="673e8-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[workPosition](../resources/workposition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="673e8-141">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="673e8-142">示例</span><span class="sxs-lookup"><span data-stu-id="673e8-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="673e8-143">请求</span><span class="sxs-lookup"><span data-stu-id="673e8-143">Request</span></span>

<span data-ttu-id="673e8-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="673e8-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```

### <a name="response"></a><span data-ttu-id="673e8-145">响应</span><span class="sxs-lookup"><span data-stu-id="673e8-145">Response</span></span>

<span data-ttu-id="673e8-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="673e8-146">The following is an example of the response.</span></span>

> <span data-ttu-id="673e8-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="673e8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workposition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
