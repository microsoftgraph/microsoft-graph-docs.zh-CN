---
title: 删除 openShift
description: 删除 openShift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bfd5af23293b82dbac18448ef7948057eb76db08
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155101"
---
# <a name="delete-openshift"></a><span data-ttu-id="719c6-103">删除 openShift</span><span class="sxs-lookup"><span data-stu-id="719c6-103">Delete openShift</span></span>

<span data-ttu-id="719c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="719c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="719c6-105">删除[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="719c6-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="719c6-106">权限</span><span class="sxs-lookup"><span data-stu-id="719c6-106">Permissions</span></span>

<span data-ttu-id="719c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="719c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="719c6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="719c6-109">Permission type</span></span>                        | <span data-ttu-id="719c6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="719c6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="719c6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="719c6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="719c6-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="719c6-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="719c6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="719c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="719c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="719c6-114">Not supported.</span></span> |
| <span data-ttu-id="719c6-115">Application</span><span class="sxs-lookup"><span data-stu-id="719c6-115">Application</span></span>                            | <span data-ttu-id="719c6-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="719c6-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="719c6-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="719c6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="719c6-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="719c6-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="719c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="719c6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="719c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="719c6-120">Request headers</span></span>

| <span data-ttu-id="719c6-121">名称</span><span class="sxs-lookup"><span data-stu-id="719c6-121">Name</span></span>          | <span data-ttu-id="719c6-122">说明</span><span class="sxs-lookup"><span data-stu-id="719c6-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="719c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="719c6-123">Authorization</span></span> | <span data-ttu-id="719c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="719c6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="719c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="719c6-126">Request body</span></span>

<span data-ttu-id="719c6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="719c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="719c6-128">响应</span><span class="sxs-lookup"><span data-stu-id="719c6-128">Response</span></span>

<span data-ttu-id="719c6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="719c6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="719c6-131">示例</span><span class="sxs-lookup"><span data-stu-id="719c6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="719c6-132">请求</span><span class="sxs-lookup"><span data-stu-id="719c6-132">Request</span></span>

<span data-ttu-id="719c6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="719c6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="719c6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="719c6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
---


### <a name="response"></a><span data-ttu-id="719c6-135">响应</span><span class="sxs-lookup"><span data-stu-id="719c6-135">Response</span></span>

<span data-ttu-id="719c6-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="719c6-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
