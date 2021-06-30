---
title: 获取 teamworkTagMember
description: 读取团队合作TagMember 对象的属性和关系。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 91d9fb93306affa987faf73032ba182ef2b1689e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209956"
---
# <a name="get-teamworktagmember"></a><span data-ttu-id="34cdd-103">获取 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="34cdd-103">Get teamworkTagMember</span></span>
<span data-ttu-id="34cdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34cdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34cdd-105">获取团队中标准 [标记](../resources/teamworktagmember.md) 的成员的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34cdd-105">Get the properties and relationships of a [member](../resources/teamworktagmember.md) of a standard tag in a team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="34cdd-106">权限</span><span class="sxs-lookup"><span data-stu-id="34cdd-106">Permissions</span></span>
<span data-ttu-id="34cdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34cdd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34cdd-109">Permission type</span></span>|<span data-ttu-id="34cdd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34cdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34cdd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34cdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34cdd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="34cdd-112">Not supported.</span></span>|
|<span data-ttu-id="34cdd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34cdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34cdd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34cdd-114">Not supported.</span></span>|
|<span data-ttu-id="34cdd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34cdd-115">Application</span></span>|<span data-ttu-id="34cdd-116">TeamworkTag.Read.All、TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34cdd-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34cdd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34cdd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34cdd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="34cdd-118">Optional query parameters</span></span>
<span data-ttu-id="34cdd-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="34cdd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="34cdd-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="34cdd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34cdd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="34cdd-121">Request headers</span></span>
|<span data-ttu-id="34cdd-122">名称</span><span class="sxs-lookup"><span data-stu-id="34cdd-122">Name</span></span>|<span data-ttu-id="34cdd-123">说明</span><span class="sxs-lookup"><span data-stu-id="34cdd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="34cdd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34cdd-124">Authorization</span></span>|<span data-ttu-id="34cdd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34cdd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34cdd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34cdd-127">Request body</span></span>
<span data-ttu-id="34cdd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34cdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34cdd-129">响应</span><span class="sxs-lookup"><span data-stu-id="34cdd-129">Response</span></span>

<span data-ttu-id="34cdd-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamworkTagMember](../resources/teamworktagmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34cdd-130">If successful, this method returns a `200 OK` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34cdd-131">示例</span><span class="sxs-lookup"><span data-stu-id="34cdd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34cdd-132">请求</span><span class="sxs-lookup"><span data-stu-id="34cdd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="34cdd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="34cdd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworktagmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```
# <a name="c"></a>[<span data-ttu-id="34cdd-134">C#</span><span class="sxs-lookup"><span data-stu-id="34cdd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworktagmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34cdd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34cdd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworktagmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34cdd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34cdd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworktagmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34cdd-137">Java</span><span class="sxs-lookup"><span data-stu-id="34cdd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworktagmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="34cdd-138">响应</span><span class="sxs-lookup"><span data-stu-id="34cdd-138">Response</span></span>
><span data-ttu-id="34cdd-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="34cdd-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Alex Wilbur",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
  }
}
```
