---
title: 获取团队合作标记
description: 读取团队合作Tag 对象的属性和关系。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: aa99a204fac9dbc2417d0e30d548638e0b63ebd6
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060662"
---
# <a name="get-teamworktag"></a><span data-ttu-id="ff59f-103">获取团队合作标记</span><span class="sxs-lookup"><span data-stu-id="ff59f-103">Get teamworkTag</span></span>
<span data-ttu-id="ff59f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff59f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff59f-105">读取 tag [对象的属性和](../resources/teamworktag.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ff59f-105">Read the properties and relationships of a [tag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff59f-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff59f-106">Permissions</span></span>
<span data-ttu-id="ff59f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff59f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff59f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff59f-109">Permission type</span></span>|<span data-ttu-id="ff59f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff59f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff59f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff59f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff59f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff59f-112">Not supported.</span></span>|
|<span data-ttu-id="ff59f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff59f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff59f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff59f-114">Not supported.</span></span>|
|<span data-ttu-id="ff59f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff59f-115">Application</span></span>|<span data-ttu-id="ff59f-116">TeamworkTag.Read.All、TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff59f-116">TeamworkTag.Read.All, TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff59f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff59f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff59f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ff59f-118">Optional query parameters</span></span>
<span data-ttu-id="ff59f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ff59f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff59f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ff59f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff59f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff59f-121">Request headers</span></span>
|<span data-ttu-id="ff59f-122">名称</span><span class="sxs-lookup"><span data-stu-id="ff59f-122">Name</span></span>|<span data-ttu-id="ff59f-123">说明</span><span class="sxs-lookup"><span data-stu-id="ff59f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ff59f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff59f-124">Authorization</span></span>|<span data-ttu-id="ff59f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff59f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff59f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff59f-127">Request body</span></span>
<span data-ttu-id="ff59f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff59f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff59f-129">响应</span><span class="sxs-lookup"><span data-stu-id="ff59f-129">Response</span></span>

<span data-ttu-id="ff59f-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [团队合作](../resources/teamworktag.md) Tag 对象。</span><span class="sxs-lookup"><span data-stu-id="ff59f-130">If successful, this method returns a `200 OK` response code and a [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff59f-131">示例</span><span class="sxs-lookup"><span data-stu-id="ff59f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff59f-132">请求</span><span class="sxs-lookup"><span data-stu-id="ff59f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="ff59f-133">响应</span><span class="sxs-lookup"><span data-stu-id="ff59f-133">Response</span></span>
><span data-ttu-id="ff59f-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ff59f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.teamworkTag",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
    "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
    "displayName": "IT Admins",
    "description": "Team admins and IT support",
    "memberCount": "2",
    "tagType": "standard"
  }
}
```

