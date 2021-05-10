---
title: unifiedRoleAssignmentScheduleRequest：cancel
description: 取消 unifiedRoleAssignmentScheduleRequest。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 801e5aa26043a4291bdbacba7d99ca26d06245d8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299220"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a><span data-ttu-id="0e6b6-103">unifiedRoleAssignmentScheduleRequest：cancel</span><span class="sxs-lookup"><span data-stu-id="0e6b6-103">unifiedRoleAssignmentScheduleRequest: cancel</span></span>
<span data-ttu-id="0e6b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e6b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e6b6-105">立即取消 [unifiedRoleAssignmentScheduleRequest，](../resources/unifiedroleassignmentschedulerequest.md) 并要求系统在 30 天后自动删除已取消的请求。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-105">Immediately cancel a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e6b6-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e6b6-106">Permissions</span></span>
<span data-ttu-id="0e6b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e6b6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e6b6-109">Permission type</span></span>|<span data-ttu-id="0e6b6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e6b6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e6b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e6b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e6b6-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0e6b6-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="0e6b6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e6b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e6b6-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0e6b6-114">Not supported</span></span>|
|<span data-ttu-id="0e6b6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e6b6-115">Application</span></span>|<span data-ttu-id="0e6b6-116">不支持</span><span class="sxs-lookup"><span data-stu-id="0e6b6-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e6b6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e6b6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="0e6b6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e6b6-118">Request headers</span></span>
|<span data-ttu-id="0e6b6-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e6b6-119">Name</span></span>|<span data-ttu-id="0e6b6-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e6b6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e6b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e6b6-121">Authorization</span></span>|<span data-ttu-id="0e6b6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e6b6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e6b6-124">Request body</span></span>
<span data-ttu-id="0e6b6-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e6b6-126">响应</span><span class="sxs-lookup"><span data-stu-id="0e6b6-126">Response</span></span>

<span data-ttu-id="0e6b6-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0e6b6-128">示例</span><span class="sxs-lookup"><span data-stu-id="0e6b6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e6b6-129">请求</span><span class="sxs-lookup"><span data-stu-id="0e6b6-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```


### <a name="response"></a><span data-ttu-id="0e6b6-130">响应</span><span class="sxs-lookup"><span data-stu-id="0e6b6-130">Response</span></span>
<span data-ttu-id="0e6b6-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e6b6-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

