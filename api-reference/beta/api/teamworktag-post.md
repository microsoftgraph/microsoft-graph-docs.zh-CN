---
title: 创建团队合作标记
description: 创建新的团队合作标记对象。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b379037f01b5d28c867de0083ec6f7a581f0ea80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060659"
---
# <a name="create-teamworktag"></a><span data-ttu-id="b7772-103">创建团队合作标记</span><span class="sxs-lookup"><span data-stu-id="b7772-103">Create teamworkTag</span></span>
<span data-ttu-id="b7772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7772-105">为团队 [中的成员](../resources/teamworktag.md) 创建标准标记。</span><span class="sxs-lookup"><span data-stu-id="b7772-105">Create a standard [tag](../resources/teamworktag.md) for members in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b7772-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7772-106">Permissions</span></span>
<span data-ttu-id="b7772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7772-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7772-109">Permission type</span></span>|<span data-ttu-id="b7772-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7772-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7772-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7772-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7772-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7772-112">Not supported.</span></span>|
|<span data-ttu-id="b7772-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7772-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7772-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7772-114">Not supported.</span></span>|
|<span data-ttu-id="b7772-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7772-115">Application</span></span>|<span data-ttu-id="b7772-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7772-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7772-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7772-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags
```

## <a name="request-headers"></a><span data-ttu-id="b7772-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7772-118">Request headers</span></span>
|<span data-ttu-id="b7772-119">名称</span><span class="sxs-lookup"><span data-stu-id="b7772-119">Name</span></span>|<span data-ttu-id="b7772-120">说明</span><span class="sxs-lookup"><span data-stu-id="b7772-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7772-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7772-121">Authorization</span></span>|<span data-ttu-id="b7772-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7772-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b7772-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7772-124">Content-Type</span></span>|<span data-ttu-id="b7772-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b7772-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7772-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7772-127">Request body</span></span>
<span data-ttu-id="b7772-128">在请求正文中，提供 [teamworkTag](../resources/teamworktag.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7772-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="b7772-129">下表显示创建团队合作标记 时所需的 [属性](../resources/teamworktag.md)。</span><span class="sxs-lookup"><span data-stu-id="b7772-129">The following table shows the properties that are required when you create the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="b7772-130">属性</span><span class="sxs-lookup"><span data-stu-id="b7772-130">Property</span></span>|<span data-ttu-id="b7772-131">类型</span><span class="sxs-lookup"><span data-stu-id="b7772-131">Type</span></span>|<span data-ttu-id="b7772-132">说明</span><span class="sxs-lookup"><span data-stu-id="b7772-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7772-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b7772-133">displayName</span></span>|<span data-ttu-id="b7772-134">String</span><span class="sxs-lookup"><span data-stu-id="b7772-134">String</span></span>|<span data-ttu-id="b7772-135">标记的名称。</span><span class="sxs-lookup"><span data-stu-id="b7772-135">Name of the tag.</span></span> <span data-ttu-id="b7772-136">该值不能超过 40 个字符。</span><span class="sxs-lookup"><span data-stu-id="b7772-136">The value cannot be more than 40 characters.</span></span>|
|<span data-ttu-id="b7772-137">members</span><span class="sxs-lookup"><span data-stu-id="b7772-137">members</span></span>| <span data-ttu-id="b7772-138">[teamworkTagMember](../resources/teamworktagmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7772-138">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span> |<span data-ttu-id="b7772-139">要添加到标记的团队成员。</span><span class="sxs-lookup"><span data-stu-id="b7772-139">Members of the team to add to the tag.</span></span> <span data-ttu-id="b7772-140">设置每个成员的用户标识符属性。</span><span class="sxs-lookup"><span data-stu-id="b7772-140">Set the user identifier property of each member.</span></span> <span data-ttu-id="b7772-141">成员计数不应超过 25。</span><span class="sxs-lookup"><span data-stu-id="b7772-141">Members count should not be more than 25.</span></span>|



## <a name="response"></a><span data-ttu-id="b7772-142">响应</span><span class="sxs-lookup"><span data-stu-id="b7772-142">Response</span></span>

<span data-ttu-id="b7772-143">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [团队合作](../resources/teamworktag.md) Tag 对象。</span><span class="sxs-lookup"><span data-stu-id="b7772-143">If successful, this method returns a `201 Created` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7772-144">示例</span><span class="sxs-lookup"><span data-stu-id="b7772-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7772-145">请求</span><span class="sxs-lookup"><span data-stu-id="b7772-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamworktag_from"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
Content-Type: application/json

{
  "displayName": "Finance",
  "members":[
    {
        "userId":"92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
        "userId":"085d800c-b86b-4bfc-a857-9371ad1caf29"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="b7772-146">响应</span><span class="sxs-lookup"><span data-stu-id="b7772-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Financee",
  "memberCount": 2,
  "tagType": "standard"
}
```

