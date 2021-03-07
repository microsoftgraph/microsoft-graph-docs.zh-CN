---
title: 创建 printerShare
description: 为指定的打印机创建新的打印机共享。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f22101ff6a621a48285f8064595916e491eb996d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517006"
---
# <a name="create-printershare"></a><span data-ttu-id="d813d-103">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="d813d-103">Create printerShare</span></span>
<span data-ttu-id="d813d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d813d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d813d-105">为指定的 **打印机创建新的 printerShare。** [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="d813d-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d813d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d813d-106">Permissions</span></span>
<span data-ttu-id="d813d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d813d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d813d-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="d813d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="d813d-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="d813d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d813d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d813d-111">Permission type</span></span> | <span data-ttu-id="d813d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d813d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d813d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d813d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d813d-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d813d-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="d813d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d813d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d813d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d813d-116">Not Supported.</span></span>|
|<span data-ttu-id="d813d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d813d-117">Application</span></span>|<span data-ttu-id="d813d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d813d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d813d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d813d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## <a name="request-headers"></a><span data-ttu-id="d813d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d813d-120">Request headers</span></span>
|<span data-ttu-id="d813d-121">名称</span><span class="sxs-lookup"><span data-stu-id="d813d-121">Name</span></span>|<span data-ttu-id="d813d-122">说明</span><span class="sxs-lookup"><span data-stu-id="d813d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d813d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d813d-123">Authorization</span></span>|<span data-ttu-id="d813d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d813d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d813d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d813d-126">Content-Type</span></span>|<span data-ttu-id="d813d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d813d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d813d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d813d-129">Request body</span></span>
<span data-ttu-id="d813d-130">在请求正文中，提供 [printerShare](../resources/printershare.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d813d-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="d813d-131">下表显示创建 [printerShare](../resources/printershare.md)时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="d813d-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="d813d-132">属性</span><span class="sxs-lookup"><span data-stu-id="d813d-132">Property</span></span>|<span data-ttu-id="d813d-133">类型</span><span class="sxs-lookup"><span data-stu-id="d813d-133">Type</span></span>|<span data-ttu-id="d813d-134">Description</span><span class="sxs-lookup"><span data-stu-id="d813d-134">Description</span></span>|<span data-ttu-id="d813d-135">是否必需？</span><span class="sxs-lookup"><span data-stu-id="d813d-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="d813d-136">打印机</span><span class="sxs-lookup"><span data-stu-id="d813d-136">printer</span></span>|<span data-ttu-id="d813d-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="d813d-137">microsoft.graph.printer</span></span>|<span data-ttu-id="d813d-138">此打印机共享相关的打印机。</span><span class="sxs-lookup"><span data-stu-id="d813d-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="d813d-139">使用 `printer@odata.bind` 语法，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="d813d-139">Use the `printer@odata.bind` syntax, as shown in the following example.</span></span>|<span data-ttu-id="d813d-140">是</span><span class="sxs-lookup"><span data-stu-id="d813d-140">Yes</span></span>|
|<span data-ttu-id="d813d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d813d-141">displayName</span></span>|<span data-ttu-id="d813d-142">String</span><span class="sxs-lookup"><span data-stu-id="d813d-142">String</span></span>|<span data-ttu-id="d813d-143">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="d813d-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="d813d-144">允许的最大长度为 50 个字符。</span><span class="sxs-lookup"><span data-stu-id="d813d-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="d813d-145">是</span><span class="sxs-lookup"><span data-stu-id="d813d-145">Yes</span></span>|
|<span data-ttu-id="d813d-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="d813d-146">allowAllUsers</span></span>|<span data-ttu-id="d813d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d813d-147">Boolean</span></span>|<span data-ttu-id="d813d-148">If `true` ， all users and groups will be granted access to this printer share.</span><span class="sxs-lookup"><span data-stu-id="d813d-148">If `true`, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="d813d-149">这将取代 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="d813d-149">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|<span data-ttu-id="d813d-150">否</span><span class="sxs-lookup"><span data-stu-id="d813d-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="d813d-151">响应</span><span class="sxs-lookup"><span data-stu-id="d813d-151">Response</span></span>

<span data-ttu-id="d813d-152">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d813d-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d813d-153">示例</span><span class="sxs-lookup"><span data-stu-id="d813d-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d813d-154">请求</span><span class="sxs-lookup"><span data-stu-id="d813d-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares
Content-Type: application/json
Content-length: 509

{
  "displayName": "ShareName",
  "allowAllUsers": false,
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
}
```

### <a name="response"></a><span data-ttu-id="d813d-155">响应</span><span class="sxs-lookup"><span data-stu-id="d813d-155">Response</span></span>
<span data-ttu-id="d813d-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d813d-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "ready",
    "details": [],
    "description": ""
  }
}
```

