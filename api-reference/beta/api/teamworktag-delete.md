---
title: 删除团队合作标记
description: 删除团队合作标记对象。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 3e23cd6e55122c81973e634cbc47ddaf88402c2d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060700"
---
# <a name="delete-teamworktag"></a><span data-ttu-id="6c6be-103">删除团队合作标记</span><span class="sxs-lookup"><span data-stu-id="6c6be-103">Delete teamworkTag</span></span>
<span data-ttu-id="6c6be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c6be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c6be-105">删除 [tag](../resources/teamworktag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c6be-105">Delete a [tag](../resources/teamworktag.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6c6be-106">权限</span><span class="sxs-lookup"><span data-stu-id="6c6be-106">Permissions</span></span>
<span data-ttu-id="6c6be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c6be-109">Permission type</span></span>|<span data-ttu-id="6c6be-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c6be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c6be-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c6be-112">Not supported.</span></span>|
|<span data-ttu-id="6c6be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c6be-114">Not supported.</span></span>|
|<span data-ttu-id="6c6be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c6be-115">Application</span></span>|<span data-ttu-id="6c6be-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6be-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c6be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="6c6be-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c6be-118">Request headers</span></span>
|<span data-ttu-id="6c6be-119">名称</span><span class="sxs-lookup"><span data-stu-id="6c6be-119">Name</span></span>|<span data-ttu-id="6c6be-120">说明</span><span class="sxs-lookup"><span data-stu-id="6c6be-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c6be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6be-121">Authorization</span></span>|<span data-ttu-id="6c6be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c6be-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6be-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c6be-124">Request body</span></span>
<span data-ttu-id="6c6be-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c6be-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c6be-126">响应</span><span class="sxs-lookup"><span data-stu-id="6c6be-126">Response</span></span>

<span data-ttu-id="6c6be-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6c6be-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6c6be-128">示例</span><span class="sxs-lookup"><span data-stu-id="6c6be-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c6be-129">请求</span><span class="sxs-lookup"><span data-stu-id="6c6be-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="6c6be-130">响应</span><span class="sxs-lookup"><span data-stu-id="6c6be-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

