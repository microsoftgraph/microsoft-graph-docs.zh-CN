---
title: 更新团队合作标记
description: 更新团队合作Tag 对象的属性。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: a17fcca078e66251a6532b2d3862352485f3cb2f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060658"
---
# <a name="update-teamworktag"></a><span data-ttu-id="82b3f-103">更新团队合作标记</span><span class="sxs-lookup"><span data-stu-id="82b3f-103">Update teamworkTag</span></span>
<span data-ttu-id="82b3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82b3f-105">更新团队合作 [Tag 对象](../resources/teamworktag.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="82b3f-105">Update the properties of a [teamworkTag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82b3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="82b3f-106">Permissions</span></span>
<span data-ttu-id="82b3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82b3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82b3f-109">Permission type</span></span>|<span data-ttu-id="82b3f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82b3f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82b3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82b3f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="82b3f-112">Not supported.</span></span>|
|<span data-ttu-id="82b3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82b3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b3f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82b3f-114">Not supported.</span></span>|
|<span data-ttu-id="82b3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82b3f-115">Application</span></span>|<span data-ttu-id="82b3f-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b3f-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b3f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82b3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="82b3f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="82b3f-118">Request headers</span></span>
|<span data-ttu-id="82b3f-119">名称</span><span class="sxs-lookup"><span data-stu-id="82b3f-119">Name</span></span>|<span data-ttu-id="82b3f-120">说明</span><span class="sxs-lookup"><span data-stu-id="82b3f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82b3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82b3f-121">Authorization</span></span>|<span data-ttu-id="82b3f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82b3f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="82b3f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82b3f-124">Content-Type</span></span>|<span data-ttu-id="82b3f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="82b3f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b3f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82b3f-127">Request body</span></span>
<span data-ttu-id="82b3f-128">在请求正文中，提供 [teamworkTag](../resources/teamworktag.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82b3f-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="82b3f-129">下表显示更新团队合作标记 时所需的 [属性](../resources/teamworktag.md)。</span><span class="sxs-lookup"><span data-stu-id="82b3f-129">The following table shows the properties that are required when you update the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="82b3f-130">属性</span><span class="sxs-lookup"><span data-stu-id="82b3f-130">Property</span></span>|<span data-ttu-id="82b3f-131">类型</span><span class="sxs-lookup"><span data-stu-id="82b3f-131">Type</span></span>|<span data-ttu-id="82b3f-132">说明</span><span class="sxs-lookup"><span data-stu-id="82b3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b3f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="82b3f-133">displayName</span></span>|<span data-ttu-id="82b3f-134">String</span><span class="sxs-lookup"><span data-stu-id="82b3f-134">String</span></span>|<span data-ttu-id="82b3f-135">标记的名称。</span><span class="sxs-lookup"><span data-stu-id="82b3f-135">Name of the tag.</span></span> <span data-ttu-id="82b3f-136">值不能超过 40 个字符。</span><span class="sxs-lookup"><span data-stu-id="82b3f-136">The value can not be more than 40 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="82b3f-137">响应</span><span class="sxs-lookup"><span data-stu-id="82b3f-137">Response</span></span>

<span data-ttu-id="82b3f-138">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [teamworkTag](../resources/teamworktag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82b3f-138">If successful, this method returns a `200 OK` response code and an updated [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82b3f-139">示例</span><span class="sxs-lookup"><span data-stu-id="82b3f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82b3f-140">请求</span><span class="sxs-lookup"><span data-stu-id="82b3f-140">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="82b3f-141">响应</span><span class="sxs-lookup"><span data-stu-id="82b3f-141">Response</span></span>
><span data-ttu-id="82b3f-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82b3f-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
