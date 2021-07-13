---
title: 删除 tenantTag
description: 删除 tenantTag 对象。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e37bb368f5cd31222c1b3eaabd26fac3a5105fc7
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402240"
---
# <a name="delete-tenanttag"></a><span data-ttu-id="51dd6-103">删除 tenantTag</span><span class="sxs-lookup"><span data-stu-id="51dd6-103">Delete tenantTag</span></span>
<span data-ttu-id="51dd6-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="51dd6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51dd6-105">删除 [tenantTag](../resources/managedtenants-tenanttag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51dd6-105">Deletes a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51dd6-106">权限</span><span class="sxs-lookup"><span data-stu-id="51dd6-106">Permissions</span></span>
<span data-ttu-id="51dd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51dd6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="51dd6-109">Permission type</span></span>|<span data-ttu-id="51dd6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51dd6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51dd6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51dd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51dd6-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="51dd6-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="51dd6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51dd6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51dd6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dd6-114">Not supported.</span></span>|
|<span data-ttu-id="51dd6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="51dd6-115">Application</span></span>|<span data-ttu-id="51dd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dd6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51dd6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51dd6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="51dd6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="51dd6-118">Request headers</span></span>
|<span data-ttu-id="51dd6-119">名称</span><span class="sxs-lookup"><span data-stu-id="51dd6-119">Name</span></span>|<span data-ttu-id="51dd6-120">说明</span><span class="sxs-lookup"><span data-stu-id="51dd6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51dd6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51dd6-121">Authorization</span></span>|<span data-ttu-id="51dd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51dd6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51dd6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="51dd6-124">Request body</span></span>
<span data-ttu-id="51dd6-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51dd6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51dd6-126">响应</span><span class="sxs-lookup"><span data-stu-id="51dd6-126">Response</span></span>

<span data-ttu-id="51dd6-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="51dd6-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="51dd6-128">示例</span><span class="sxs-lookup"><span data-stu-id="51dd6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51dd6-129">请求</span><span class="sxs-lookup"><span data-stu-id="51dd6-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tenanttag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```


### <a name="response"></a><span data-ttu-id="51dd6-130">响应</span><span class="sxs-lookup"><span data-stu-id="51dd6-130">Response</span></span>
><span data-ttu-id="51dd6-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51dd6-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
