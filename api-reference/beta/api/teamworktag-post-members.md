---
title: 创建 teamworkTagMember
description: 创建新的 teamworkTagMember 对象。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28ae8ae4749e1ecca4f5e370858e88de45d2faf4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060660"
---
# <a name="create-teamworktagmember"></a><span data-ttu-id="8598a-103">创建 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="8598a-103">Create teamworkTagMember</span></span>
<span data-ttu-id="8598a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8598a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8598a-105">在团队 [中创建新的团队合作TagMember](../resources/teamworktagmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8598a-105">Create a new [teamworkTagMember](../resources/teamworktagmember.md) object in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="8598a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8598a-106">Permissions</span></span>
<span data-ttu-id="8598a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8598a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8598a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8598a-109">Permission type</span></span>|<span data-ttu-id="8598a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8598a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8598a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8598a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8598a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8598a-112">Not supported.</span></span>|
|<span data-ttu-id="8598a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8598a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8598a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8598a-114">Not supported.</span></span>|
|<span data-ttu-id="8598a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8598a-115">Application</span></span>|<span data-ttu-id="8598a-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8598a-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8598a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8598a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a><span data-ttu-id="8598a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8598a-118">Request headers</span></span>
|<span data-ttu-id="8598a-119">名称</span><span class="sxs-lookup"><span data-stu-id="8598a-119">Name</span></span>|<span data-ttu-id="8598a-120">说明</span><span class="sxs-lookup"><span data-stu-id="8598a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8598a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8598a-121">Authorization</span></span>|<span data-ttu-id="8598a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8598a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8598a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8598a-124">Content-Type</span></span>|<span data-ttu-id="8598a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8598a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8598a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8598a-127">Request body</span></span>
<span data-ttu-id="8598a-128">在请求正文中，提供 [teamworkTagMember](../resources/teamworktagmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8598a-128">In the request body, supply a JSON representation of the [teamworkTagMember](../resources/teamworktagmember.md) object.</span></span>

<span data-ttu-id="8598a-129">下表显示创建 [团队合作TagMember 时所需的属性](../resources/teamworktagmember.md)。</span><span class="sxs-lookup"><span data-stu-id="8598a-129">The following table shows the properties that are required when you create the [teamworkTagMember](../resources/teamworktagmember.md).</span></span>

|<span data-ttu-id="8598a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8598a-130">Property</span></span>|<span data-ttu-id="8598a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8598a-131">Type</span></span>|<span data-ttu-id="8598a-132">描述</span><span class="sxs-lookup"><span data-stu-id="8598a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8598a-133">userId</span><span class="sxs-lookup"><span data-stu-id="8598a-133">userId</span></span>|<span data-ttu-id="8598a-134">String</span><span class="sxs-lookup"><span data-stu-id="8598a-134">String</span></span>|<span data-ttu-id="8598a-135">团队成员的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="8598a-135">User identifier of the member of the team.</span></span>|



## <a name="response"></a><span data-ttu-id="8598a-136">响应</span><span class="sxs-lookup"><span data-stu-id="8598a-136">Response</span></span>

<span data-ttu-id="8598a-137">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [teamworkTagMember](../resources/teamworktagmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8598a-137">If successful, this method returns a `201 Created` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8598a-138">示例</span><span class="sxs-lookup"><span data-stu-id="8598a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8598a-139">请求</span><span class="sxs-lookup"><span data-stu-id="8598a-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="8598a-140">响应</span><span class="sxs-lookup"><span data-stu-id="8598a-140">Response</span></span>
><span data-ttu-id="8598a-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8598a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

