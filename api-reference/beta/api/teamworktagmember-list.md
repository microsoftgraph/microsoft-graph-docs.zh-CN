---
title: 列出 teamworkTagMembers
description: 获取 teamworkTagMember 对象及其属性的列表。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0eca6f9469f53cb639068d712421e85b27e185f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209158"
---
# <a name="list-members-in-a-teamworktag"></a><span data-ttu-id="54c57-103">列出团队合作标记中的成员</span><span class="sxs-lookup"><span data-stu-id="54c57-103">List members in a teamworkTag</span></span>
<span data-ttu-id="54c57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54c57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54c57-105">获取团队 [中标准](../resources/teamworktagmember.md) 标记的成员及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="54c57-105">Get a list of the [members](../resources/teamworktagmember.md) of a standard tag in a team and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="54c57-106">权限</span><span class="sxs-lookup"><span data-stu-id="54c57-106">Permissions</span></span>
<span data-ttu-id="54c57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54c57-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54c57-109">Permission type</span></span>|<span data-ttu-id="54c57-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54c57-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54c57-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54c57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54c57-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="54c57-112">Not supported.</span></span>|
|<span data-ttu-id="54c57-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54c57-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54c57-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="54c57-114">Not supported.</span></span>|
|<span data-ttu-id="54c57-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="54c57-115">Application</span></span>|<span data-ttu-id="54c57-116">TeamworkTag.Read.All、TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c57-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54c57-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54c57-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54c57-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54c57-118">Optional query parameters</span></span>
<span data-ttu-id="54c57-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54c57-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="54c57-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="54c57-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="54c57-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54c57-121">Request headers</span></span>
|<span data-ttu-id="54c57-122">名称</span><span class="sxs-lookup"><span data-stu-id="54c57-122">Name</span></span>|<span data-ttu-id="54c57-123">说明</span><span class="sxs-lookup"><span data-stu-id="54c57-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="54c57-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54c57-124">Authorization</span></span>|<span data-ttu-id="54c57-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54c57-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54c57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54c57-127">Request body</span></span>
<span data-ttu-id="54c57-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54c57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54c57-129">响应</span><span class="sxs-lookup"><span data-stu-id="54c57-129">Response</span></span>

<span data-ttu-id="54c57-130">如果成功，此方法在响应正文中返回 响应代码 `200 OK` [和 teamworkTagMember](../resources/teamworktagmember.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="54c57-130">If successful, this method returns a `200 OK` response code and a collection of [teamworkTagMember](../resources/teamworktagmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54c57-131">示例</span><span class="sxs-lookup"><span data-stu-id="54c57-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54c57-132">请求</span><span class="sxs-lookup"><span data-stu-id="54c57-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="54c57-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="54c57-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
```
# <a name="c"></a>[<span data-ttu-id="54c57-134">C#</span><span class="sxs-lookup"><span data-stu-id="54c57-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamworktagmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54c57-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54c57-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamworktagmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54c57-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54c57-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamworktagmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54c57-137">Java</span><span class="sxs-lookup"><span data-stu-id="54c57-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamworktagmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="54c57-138">响应</span><span class="sxs-lookup"><span data-stu-id="54c57-138">Response</span></span>
><span data-ttu-id="54c57-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54c57-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkTagMember",
      "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
      "displayName": "Grady Archie",
      "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
      "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
      "@odata.type": "#microsoft.graph.teamworkTagMember",
      "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLMW0N2YtNDViOS05NWYyLWIyZjJlZjYyGHVjZQ==",
      "displayName": "Lee Gu",
      "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",    
      "userId": "945fe02a-5dc1-4d28-bf5c-30a6147fe842"
    }
  ]
}
```
