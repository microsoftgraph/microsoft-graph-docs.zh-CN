---
title: printer： restoreFactoryDefaults
description: 重置打印机的默认设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 64b8db4477e79918e863b80da236e42afec83f76
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517324"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="65c39-103">printer： restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="65c39-103">printer: restoreFactoryDefaults</span></span>
<span data-ttu-id="65c39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="65c39-105">将 [打印机](../resources/printer.md)的默认设置还原到制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="65c39-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="65c39-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="65c39-106">Permissions</span></span>
<span data-ttu-id="65c39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="65c39-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="65c39-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="65c39-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="65c39-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="65c39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65c39-111">Permission type</span></span> | <span data-ttu-id="65c39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65c39-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="65c39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65c39-113">Delegated (work or school account)</span></span>| <span data-ttu-id="65c39-114">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="65c39-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="65c39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65c39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65c39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65c39-116">Not Supported.</span></span>|
|<span data-ttu-id="65c39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65c39-117">Application</span></span>| <span data-ttu-id="65c39-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65c39-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65c39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65c39-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/restoreFactoryDefaults
```

## <a name="request-headers"></a><span data-ttu-id="65c39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65c39-120">Request headers</span></span>
|<span data-ttu-id="65c39-121">名称</span><span class="sxs-lookup"><span data-stu-id="65c39-121">Name</span></span>|<span data-ttu-id="65c39-122">说明</span><span class="sxs-lookup"><span data-stu-id="65c39-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65c39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65c39-123">Authorization</span></span>|<span data-ttu-id="65c39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65c39-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65c39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65c39-126">Request body</span></span>
<span data-ttu-id="65c39-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65c39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65c39-128">响应</span><span class="sxs-lookup"><span data-stu-id="65c39-128">Response</span></span>

<span data-ttu-id="65c39-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="65c39-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65c39-131">示例</span><span class="sxs-lookup"><span data-stu-id="65c39-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65c39-132">请求</span><span class="sxs-lookup"><span data-stu-id="65c39-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printer_restorefactorydefaults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/restoreFactoryDefaults
```


### <a name="response"></a><span data-ttu-id="65c39-133">响应</span><span class="sxs-lookup"><span data-stu-id="65c39-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

