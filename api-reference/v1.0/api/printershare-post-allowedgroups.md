---
title: 为 printerShare 创建 allowedGroup
description: 授予指定的组访问权限，以将打印作业提交到关联的打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8db8facb302863ec96107c333b8e17f59f2b27a4
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573857"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="c73d5-103">为 printerShare 创建 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="c73d5-103">Create allowedGroup for printerShare</span></span>
<span data-ttu-id="c73d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c73d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c73d5-105">授予指定的组访问权限，以将打印作业提交到关联的[printerShare。](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c73d5-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c73d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c73d5-106">Permissions</span></span>
<span data-ttu-id="c73d5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c73d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c73d5-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="c73d5-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c73d5-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="c73d5-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c73d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c73d5-111">Permission type</span></span> | <span data-ttu-id="c73d5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c73d5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c73d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c73d5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c73d5-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c73d5-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c73d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c73d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c73d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c73d5-116">Not Supported.</span></span>|
|<span data-ttu-id="c73d5-117">Application</span><span class="sxs-lookup"><span data-stu-id="c73d5-117">Application</span></span>|<span data-ttu-id="c73d5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c73d5-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c73d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c73d5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c73d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c73d5-120">Request headers</span></span>
|<span data-ttu-id="c73d5-121">名称</span><span class="sxs-lookup"><span data-stu-id="c73d5-121">Name</span></span>|<span data-ttu-id="c73d5-122">说明</span><span class="sxs-lookup"><span data-stu-id="c73d5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c73d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c73d5-123">Authorization</span></span>|<span data-ttu-id="c73d5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c73d5-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c73d5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c73d5-126">Content-Type</span></span>|<span data-ttu-id="c73d5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c73d5-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c73d5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c73d5-129">Request body</span></span>
<span data-ttu-id="c73d5-130">在请求正文中，使用格式提供对组实体的引用， `@odata.id` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="c73d5-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="c73d5-131">响应</span><span class="sxs-lookup"><span data-stu-id="c73d5-131">Response</span></span>

<span data-ttu-id="c73d5-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c73d5-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c73d5-133">示例</span><span class="sxs-lookup"><span data-stu-id="c73d5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c73d5-134">请求</span><span class="sxs-lookup"><span data-stu-id="c73d5-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/$ref
Content-Type: application/json
Content-length: 47

{
  "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}"
}
```


### <a name="response"></a><span data-ttu-id="c73d5-135">响应</span><span class="sxs-lookup"><span data-stu-id="c73d5-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 204 No Content
```

