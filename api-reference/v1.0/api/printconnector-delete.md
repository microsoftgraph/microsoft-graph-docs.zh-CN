---
title: 删除 printConnector
description: 删除 (printConnector) 注册。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4366aa9f3ab674861c404a4ce0f9c329a06b23e9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516994"
---
# <a name="delete-printconnector"></a><span data-ttu-id="c51b7-103">删除 printConnector</span><span class="sxs-lookup"><span data-stu-id="c51b7-103">Delete printConnector</span></span>
<span data-ttu-id="c51b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c51b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c51b7-105">删除 (注销 **) Connector。**</span><span class="sxs-lookup"><span data-stu-id="c51b7-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c51b7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c51b7-106">Permissions</span></span>
<span data-ttu-id="c51b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c51b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c51b7-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="c51b7-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c51b7-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="c51b7-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c51b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c51b7-111">Permission type</span></span> | <span data-ttu-id="c51b7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c51b7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c51b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c51b7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c51b7-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51b7-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="c51b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c51b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c51b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c51b7-116">Not Supported.</span></span>|
|<span data-ttu-id="c51b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c51b7-117">Application</span></span>|<span data-ttu-id="c51b7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c51b7-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c51b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c51b7-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c51b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c51b7-120">Request headers</span></span>
|<span data-ttu-id="c51b7-121">名称</span><span class="sxs-lookup"><span data-stu-id="c51b7-121">Name</span></span>|<span data-ttu-id="c51b7-122">说明</span><span class="sxs-lookup"><span data-stu-id="c51b7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c51b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51b7-123">Authorization</span></span>|<span data-ttu-id="c51b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c51b7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c51b7-126">Request body</span></span>
<span data-ttu-id="c51b7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c51b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c51b7-128">响应</span><span class="sxs-lookup"><span data-stu-id="c51b7-128">Response</span></span>
<span data-ttu-id="c51b7-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c51b7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="c51b7-131">错误条件和消息</span><span class="sxs-lookup"><span data-stu-id="c51b7-131">Error conditions and messages</span></span>

|<span data-ttu-id="c51b7-132">应用场景</span><span class="sxs-lookup"><span data-stu-id="c51b7-132">Scenario</span></span>|<span data-ttu-id="c51b7-133">Method</span><span class="sxs-lookup"><span data-stu-id="c51b7-133">Method</span></span>|<span data-ttu-id="c51b7-134">代码</span><span class="sxs-lookup"><span data-stu-id="c51b7-134">Code</span></span>|<span data-ttu-id="c51b7-135">消息</span><span class="sxs-lookup"><span data-stu-id="c51b7-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="c51b7-136">用户尝试删除已注册一个或多个打印机的连接器</span><span class="sxs-lookup"><span data-stu-id="c51b7-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="c51b7-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="c51b7-137">DELETE</span></span>|<span data-ttu-id="c51b7-138">409</span><span class="sxs-lookup"><span data-stu-id="c51b7-138">409</span></span>|<span data-ttu-id="c51b7-139">删除连接器之前，请注销关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="c51b7-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="c51b7-140">示例</span><span class="sxs-lookup"><span data-stu-id="c51b7-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c51b7-141">请求</span><span class="sxs-lookup"><span data-stu-id="c51b7-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```


### <a name="response"></a><span data-ttu-id="c51b7-142">响应</span><span class="sxs-lookup"><span data-stu-id="c51b7-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

