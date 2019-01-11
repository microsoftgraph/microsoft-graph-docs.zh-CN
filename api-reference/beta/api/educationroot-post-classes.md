---
title: 创建 educationClass
description: 创建新课程。 此操作还会创建通用组。 当您使用此 API 创建的类时，它将添加到组，这将特殊属性
localization_priority: Normal
ms.openlocfilehash: b75ce58b1d56fe1ba231299b9c2c943ca28e0403
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843468"
---
# <a name="create-educationclass"></a><span data-ttu-id="5c425-105">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="5c425-105">Create educationClass</span></span>

> <span data-ttu-id="5c425-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c425-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c425-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c425-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c425-108">创建新课程。</span><span class="sxs-lookup"><span data-stu-id="5c425-108">Create a new class.</span></span> <span data-ttu-id="5c425-109">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="5c425-109">This will also create a universal group.</span></span> <span data-ttu-id="5c425-110">当使用此 API 创建课程时，会向组添加特殊属性，继而在 Microsoft Teams 中添加分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="5c425-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c425-111">权限</span><span class="sxs-lookup"><span data-stu-id="5c425-111">Permissions</span></span>
<span data-ttu-id="5c425-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c425-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c425-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c425-114">Permission type</span></span>      | <span data-ttu-id="5c425-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c425-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c425-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c425-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="5c425-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c425-117">Not supported.</span></span>  |
|<span data-ttu-id="5c425-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c425-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5c425-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c425-119">Not supported.</span></span>  |
|<span data-ttu-id="5c425-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c425-120">Application</span></span> | <span data-ttu-id="5c425-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c425-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5c425-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c425-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="5c425-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c425-123">Request headers</span></span>
| <span data-ttu-id="5c425-124">标头</span><span class="sxs-lookup"><span data-stu-id="5c425-124">Header</span></span>       | <span data-ttu-id="5c425-125">值</span><span class="sxs-lookup"><span data-stu-id="5c425-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c425-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c425-126">Authorization</span></span>  | <span data-ttu-id="5c425-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c425-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c425-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c425-129">Content-Type</span></span>  | <span data-ttu-id="5c425-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5c425-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c425-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c425-131">Request body</span></span>
<span data-ttu-id="5c425-132">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c425-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5c425-133">响应</span><span class="sxs-lookup"><span data-stu-id="5c425-133">Response</span></span>
<span data-ttu-id="5c425-134">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c425-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c425-135">示例</span><span class="sxs-lookup"><span data-stu-id="5c425-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c425-136">请求</span><span class="sxs-lookup"><span data-stu-id="5c425-136">Request</span></span>
<span data-ttu-id="5c425-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c425-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="5c425-138">响应</span><span class="sxs-lookup"><span data-stu-id="5c425-138">Response</span></span>
<span data-ttu-id="5c425-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c425-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5c425-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5c425-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
