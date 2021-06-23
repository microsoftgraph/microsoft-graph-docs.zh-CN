---
title: 列出团队合作标记
description: 获取 teamworkTag 对象及其属性的列表。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 0a5e008e32565675982ec7d120be3d6d3bad98ed
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060661"
---
# <a name="list-teamworktags"></a><span data-ttu-id="0e859-103">列出团队合作标记</span><span class="sxs-lookup"><span data-stu-id="0e859-103">List teamworkTags</span></span>
<span data-ttu-id="0e859-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e859-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e859-105">获取标记对象 [及其](../resources/teamworktag.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0e859-105">Get a list of the [tags](../resources/teamworktag.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e859-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e859-106">Permissions</span></span>
<span data-ttu-id="0e859-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e859-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e859-109">Permission type</span></span>|<span data-ttu-id="0e859-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e859-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e859-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e859-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e859-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e859-112">Not supported.</span></span>|
|<span data-ttu-id="0e859-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e859-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e859-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e859-114">Not supported.</span></span>|
|<span data-ttu-id="0e859-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e859-115">Application</span></span>|<span data-ttu-id="0e859-116">TeamworkTag.Read.All、TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e859-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e859-117">关系</span><span class="sxs-lookup"><span data-stu-id="0e859-117">Relationships</span></span>
|<span data-ttu-id="0e859-118">关系</span><span class="sxs-lookup"><span data-stu-id="0e859-118">Relationship</span></span>|<span data-ttu-id="0e859-119">类型</span><span class="sxs-lookup"><span data-stu-id="0e859-119">Type</span></span>|<span data-ttu-id="0e859-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e859-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e859-121">成员</span><span class="sxs-lookup"><span data-stu-id="0e859-121">members</span></span>|<span data-ttu-id="0e859-122">[teamworkTag](../resources/teamworktag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e859-122">[teamworkTag](../resources/teamworktag.md) collection</span></span>|<span data-ttu-id="0e859-123">分配给团队的标记。</span><span class="sxs-lookup"><span data-stu-id="0e859-123">Tags assigned to a team.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e859-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e859-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e859-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e859-125">Optional query parameters</span></span>
<span data-ttu-id="0e859-126">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e859-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e859-127">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0e859-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e859-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e859-128">Request headers</span></span>
|<span data-ttu-id="0e859-129">名称</span><span class="sxs-lookup"><span data-stu-id="0e859-129">Name</span></span>|<span data-ttu-id="0e859-130">说明</span><span class="sxs-lookup"><span data-stu-id="0e859-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e859-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e859-131">Authorization</span></span>|<span data-ttu-id="0e859-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e859-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e859-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e859-134">Request body</span></span>
<span data-ttu-id="0e859-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e859-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e859-136">响应</span><span class="sxs-lookup"><span data-stu-id="0e859-136">Response</span></span>

<span data-ttu-id="0e859-137">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamworkTag](../resources/teamworktag.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0e859-137">If successful, this method returns a `200 OK` response code and a collection of [teamworkTag](../resources/teamworktag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e859-138">示例</span><span class="sxs-lookup"><span data-stu-id="0e859-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e859-139">请求</span><span class="sxs-lookup"><span data-stu-id="0e859-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
```


### <a name="response"></a><span data-ttu-id="0e859-140">响应</span><span class="sxs-lookup"><span data-stu-id="0e859-140">Response</span></span>
><span data-ttu-id="0e859-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e859-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamworkTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Finance",
        "description": "Finance Team for Mach 8 Project",
        "memberCount": 2,
        "tagType": "standard"
    },
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjIzk3ZjYyMzQ0LTU3ZGMtNDA5Yy04OGFkLWM0YWYxNDE1OGZmNQ==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Legal",
        "description": "Legal experts, ask us your legal questions",
        "memberCount": 4,
        "tagType": "standard"
    }
  ]
}
```

