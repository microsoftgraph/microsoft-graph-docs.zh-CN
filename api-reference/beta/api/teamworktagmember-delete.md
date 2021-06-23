---
title: 删除 teamworkTagMember
description: 删除 teamworkTagMember 对象。
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab64e7053757fed77a086bbdbde4c408813b1879
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060657"
---
# <a name="delete-teamworktagmember"></a><span data-ttu-id="ec55e-103">删除 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="ec55e-103">Delete teamworkTagMember</span></span>
<span data-ttu-id="ec55e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec55e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec55e-105">从 [团队](../resources/teamworktagmember.md) 中的标准标记中删除成员。</span><span class="sxs-lookup"><span data-stu-id="ec55e-105">Delete a [member](../resources/teamworktagmember.md) from a standard tag in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ec55e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec55e-106">Permissions</span></span>
<span data-ttu-id="ec55e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec55e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec55e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec55e-109">Permission type</span></span>|<span data-ttu-id="ec55e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec55e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec55e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec55e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec55e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec55e-112">Not supported.</span></span>|
|<span data-ttu-id="ec55e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec55e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec55e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec55e-114">Not supported.</span></span>|
|<span data-ttu-id="ec55e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec55e-115">Application</span></span>|<span data-ttu-id="ec55e-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec55e-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec55e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec55e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="request-headers"></a><span data-ttu-id="ec55e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec55e-118">Request headers</span></span>
|<span data-ttu-id="ec55e-119">名称</span><span class="sxs-lookup"><span data-stu-id="ec55e-119">Name</span></span>|<span data-ttu-id="ec55e-120">说明</span><span class="sxs-lookup"><span data-stu-id="ec55e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec55e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec55e-121">Authorization</span></span>|<span data-ttu-id="ec55e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec55e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec55e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec55e-124">Request body</span></span>
<span data-ttu-id="ec55e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec55e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec55e-126">响应</span><span class="sxs-lookup"><span data-stu-id="ec55e-126">Response</span></span>

<span data-ttu-id="ec55e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ec55e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ec55e-128">示例</span><span class="sxs-lookup"><span data-stu-id="ec55e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec55e-129">请求</span><span class="sxs-lookup"><span data-stu-id="ec55e-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktagmember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```


### <a name="response"></a><span data-ttu-id="ec55e-130">响应</span><span class="sxs-lookup"><span data-stu-id="ec55e-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
