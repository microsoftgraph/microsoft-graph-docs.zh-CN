---
title: 更新团队合作标记
description: 更新团队合作Tag 对象的属性。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 93e78b863c0b03f475c0d6e52a12316d4eee580d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210105"
---
# <a name="update-teamworktag"></a><span data-ttu-id="e4f96-103">更新团队合作标记</span><span class="sxs-lookup"><span data-stu-id="e4f96-103">Update teamworkTag</span></span>
<span data-ttu-id="e4f96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f96-105">更新团队合作 [Tag 对象](../resources/teamworktag.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e4f96-105">Update the properties of a [teamworkTag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f96-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4f96-106">Permissions</span></span>
<span data-ttu-id="e4f96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4f96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4f96-109">Permission type</span></span>|<span data-ttu-id="e4f96-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4f96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4f96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4f96-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f96-112">Not supported.</span></span>|
|<span data-ttu-id="e4f96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4f96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f96-114">Not supported.</span></span>|
|<span data-ttu-id="e4f96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4f96-115">Application</span></span>|<span data-ttu-id="e4f96-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f96-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4f96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4f96-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="e4f96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4f96-118">Request headers</span></span>
|<span data-ttu-id="e4f96-119">名称</span><span class="sxs-lookup"><span data-stu-id="e4f96-119">Name</span></span>|<span data-ttu-id="e4f96-120">说明</span><span class="sxs-lookup"><span data-stu-id="e4f96-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4f96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f96-121">Authorization</span></span>|<span data-ttu-id="e4f96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4f96-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4f96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4f96-124">Content-Type</span></span>|<span data-ttu-id="e4f96-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e4f96-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4f96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4f96-127">Request body</span></span>
<span data-ttu-id="e4f96-128">在请求正文中，提供 [teamworkTag](../resources/teamworktag.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f96-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="e4f96-129">下表显示更新团队合作标记 时所需的 [属性](../resources/teamworktag.md)。</span><span class="sxs-lookup"><span data-stu-id="e4f96-129">The following table shows the properties that are required when you update the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="e4f96-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4f96-130">Property</span></span>|<span data-ttu-id="e4f96-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4f96-131">Type</span></span>|<span data-ttu-id="e4f96-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4f96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f96-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e4f96-133">displayName</span></span>|<span data-ttu-id="e4f96-134">String</span><span class="sxs-lookup"><span data-stu-id="e4f96-134">String</span></span>|<span data-ttu-id="e4f96-135">标记的名称。</span><span class="sxs-lookup"><span data-stu-id="e4f96-135">Name of the tag.</span></span> <span data-ttu-id="e4f96-136">该值不能超过 40 个字符。</span><span class="sxs-lookup"><span data-stu-id="e4f96-136">The value can't be more than 40 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="e4f96-137">响应</span><span class="sxs-lookup"><span data-stu-id="e4f96-137">Response</span></span>

<span data-ttu-id="e4f96-138">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [teamworkTag](../resources/teamworktag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4f96-138">If successful, this method returns a `200 OK` response code and an updated [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4f96-139">示例</span><span class="sxs-lookup"><span data-stu-id="e4f96-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4f96-140">请求</span><span class="sxs-lookup"><span data-stu-id="e4f96-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4f96-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f96-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamworktag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
Content-Type: application/json
Content-length: 185

{
  "displayName": "Finance"
}
```
# <a name="c"></a>[<span data-ttu-id="e4f96-142">C#</span><span class="sxs-lookup"><span data-stu-id="e4f96-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4f96-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4f96-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4f96-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4f96-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4f96-145">Java</span><span class="sxs-lookup"><span data-stu-id="e4f96-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e4f96-146">响应</span><span class="sxs-lookup"><span data-stu-id="e4f96-146">Response</span></span>
><span data-ttu-id="e4f96-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4f96-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Finance",
  "memberCount": 2,
  "tagType": "standard"
}
```
