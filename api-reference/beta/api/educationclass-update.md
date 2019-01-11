---
title: 更新 educationclass 属性
description: 更新课程属性。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 1c011a19371490bb8d00a7048a9809cc8a58beee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813991"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="c8589-103">更新 educationclass 属性</span><span class="sxs-lookup"><span data-stu-id="c8589-103">Update educationclass properties</span></span>

> <span data-ttu-id="c8589-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c8589-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8589-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8589-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8589-106">更新课程属性。</span><span class="sxs-lookup"><span data-stu-id="c8589-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8589-107">权限</span><span class="sxs-lookup"><span data-stu-id="c8589-107">Permissions</span></span>
<span data-ttu-id="c8589-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8589-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8589-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8589-110">Permission type</span></span>      | <span data-ttu-id="c8589-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8589-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8589-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8589-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8589-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8589-113">Not supported.</span></span>  |
|<span data-ttu-id="c8589-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8589-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8589-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8589-115">Not supported.</span></span>   |
|<span data-ttu-id="c8589-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8589-116">Application</span></span> | <span data-ttu-id="c8589-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8589-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c8589-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8589-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c8589-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8589-119">Request headers</span></span>
| <span data-ttu-id="c8589-120">标头</span><span class="sxs-lookup"><span data-stu-id="c8589-120">Header</span></span>       | <span data-ttu-id="c8589-121">值</span><span class="sxs-lookup"><span data-stu-id="c8589-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8589-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8589-122">Authorization</span></span>  | <span data-ttu-id="c8589-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8589-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c8589-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8589-125">Content-Type</span></span>  | <span data-ttu-id="c8589-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8589-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8589-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8589-127">Request body</span></span>
<span data-ttu-id="c8589-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c8589-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c8589-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c8589-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c8589-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c8589-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8589-131">属性</span><span class="sxs-lookup"><span data-stu-id="c8589-131">Property</span></span>     | <span data-ttu-id="c8589-132">类型</span><span class="sxs-lookup"><span data-stu-id="c8589-132">Type</span></span>   |<span data-ttu-id="c8589-133">说明</span><span class="sxs-lookup"><span data-stu-id="c8589-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8589-134">说明</span><span class="sxs-lookup"><span data-stu-id="c8589-134">description</span></span>|<span data-ttu-id="c8589-135">String</span><span class="sxs-lookup"><span data-stu-id="c8589-135">String</span></span>| <span data-ttu-id="c8589-136">课程说明。</span><span class="sxs-lookup"><span data-stu-id="c8589-136">Description of the class.</span></span>|
|<span data-ttu-id="c8589-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c8589-137">displayName</span></span>|<span data-ttu-id="c8589-138">String</span><span class="sxs-lookup"><span data-stu-id="c8589-138">String</span></span>| <span data-ttu-id="c8589-139">课程名称。</span><span class="sxs-lookup"><span data-stu-id="c8589-139">Name of the class.</span></span>|
|<span data-ttu-id="c8589-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c8589-140">mailNickname</span></span>|<span data-ttu-id="c8589-141">String</span><span class="sxs-lookup"><span data-stu-id="c8589-141">String</span></span>| <span data-ttu-id="c8589-142">用于向所有用户发送电子邮件的电子邮件别名（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="c8589-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="c8589-143"><!-- Please verify the revised description here. -->| classCode |字符串 |Class 代码使用学校。 || externalId |字符串 |从同步系统类的 ID。</span><span class="sxs-lookup"><span data-stu-id="c8589-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="c8589-144">| |externalName|String|同步系统中的课程名称。| |externalSource|string| 此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="c8589-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="c8589-145">可取值为：`sis`、`manual`、`enum_sentinel`。|</span><span class="sxs-lookup"><span data-stu-id="c8589-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="c8589-146">响应</span><span class="sxs-lookup"><span data-stu-id="c8589-146">Response</span></span>
<span data-ttu-id="c8589-147">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8589-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8589-148">示例</span><span class="sxs-lookup"><span data-stu-id="c8589-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8589-149">请求</span><span class="sxs-lookup"><span data-stu-id="c8589-149">Request</span></span>
<span data-ttu-id="c8589-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c8589-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="c8589-151">响应</span><span class="sxs-lookup"><span data-stu-id="c8589-151">Response</span></span>
<span data-ttu-id="c8589-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c8589-152">The following is an example of the response.</span></span> 

><span data-ttu-id="c8589-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8589-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
