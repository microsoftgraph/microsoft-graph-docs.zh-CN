---
title: 创建 teamworkTagMember
description: 创建新的 teamworkTagMember 对象。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9376b8ddb690d4aaee1d571c83e0d94b96482935
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210138"
---
# <a name="create-teamworktagmember"></a><span data-ttu-id="8e90c-103">创建 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="8e90c-103">Create teamworkTagMember</span></span>
<span data-ttu-id="8e90c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e90c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e90c-105">在团队 [中创建新的团队合作TagMember](../resources/teamworktagmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e90c-105">Create a new [teamworkTagMember](../resources/teamworktagmember.md) object in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e90c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8e90c-106">Permissions</span></span>
<span data-ttu-id="8e90c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e90c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e90c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e90c-109">Permission type</span></span>|<span data-ttu-id="8e90c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e90c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e90c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e90c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e90c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e90c-112">Not supported.</span></span>|
|<span data-ttu-id="8e90c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e90c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e90c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e90c-114">Not supported.</span></span>|
|<span data-ttu-id="8e90c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e90c-115">Application</span></span>|<span data-ttu-id="8e90c-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e90c-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e90c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e90c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a><span data-ttu-id="8e90c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e90c-118">Request headers</span></span>
|<span data-ttu-id="8e90c-119">名称</span><span class="sxs-lookup"><span data-stu-id="8e90c-119">Name</span></span>|<span data-ttu-id="8e90c-120">说明</span><span class="sxs-lookup"><span data-stu-id="8e90c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e90c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e90c-121">Authorization</span></span>|<span data-ttu-id="8e90c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e90c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8e90c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e90c-124">Content-Type</span></span>|<span data-ttu-id="8e90c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8e90c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e90c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e90c-127">Request body</span></span>
<span data-ttu-id="8e90c-128">在请求正文中，提供 [teamworkTagMember](../resources/teamworktagmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e90c-128">In the request body, supply a JSON representation of the [teamworkTagMember](../resources/teamworktagmember.md) object.</span></span>

<span data-ttu-id="8e90c-129">下表显示创建 [团队合作TagMember 时所需的属性](../resources/teamworktagmember.md)。</span><span class="sxs-lookup"><span data-stu-id="8e90c-129">The following table shows the properties that are required when you create the [teamworkTagMember](../resources/teamworktagmember.md).</span></span>

|<span data-ttu-id="8e90c-130">属性</span><span class="sxs-lookup"><span data-stu-id="8e90c-130">Property</span></span>|<span data-ttu-id="8e90c-131">类型</span><span class="sxs-lookup"><span data-stu-id="8e90c-131">Type</span></span>|<span data-ttu-id="8e90c-132">描述</span><span class="sxs-lookup"><span data-stu-id="8e90c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e90c-133">userId</span><span class="sxs-lookup"><span data-stu-id="8e90c-133">userId</span></span>|<span data-ttu-id="8e90c-134">String</span><span class="sxs-lookup"><span data-stu-id="8e90c-134">String</span></span>|<span data-ttu-id="8e90c-135">团队成员的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="8e90c-135">User identifier of the member of the team.</span></span>|



## <a name="response"></a><span data-ttu-id="8e90c-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e90c-136">Response</span></span>

<span data-ttu-id="8e90c-137">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [teamworkTagMember](../resources/teamworktagmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e90c-137">If successful, this method returns a `201 Created` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e90c-138">示例</span><span class="sxs-lookup"><span data-stu-id="8e90c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e90c-139">请求</span><span class="sxs-lookup"><span data-stu-id="8e90c-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8e90c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e90c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamworktagmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
Content-Type: application/json
Content-length: 144

{
    "userId":"97f62344-57dc-409c-88ad-c4af14158ff5"
}
```
# <a name="c"></a>[<span data-ttu-id="8e90c-141">C#</span><span class="sxs-lookup"><span data-stu-id="8e90c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-teamworktagmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e90c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e90c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamworktagmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e90c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e90c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamworktagmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e90c-144">Java</span><span class="sxs-lookup"><span data-stu-id="8e90c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-teamworktagmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8e90c-145">响应</span><span class="sxs-lookup"><span data-stu-id="8e90c-145">Response</span></span>
><span data-ttu-id="8e90c-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e90c-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Megan Bowen",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
}
```

