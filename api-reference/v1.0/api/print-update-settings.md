---
title: 更新 printSettings
description: 更新通用打印服务的租户范围设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cc1af332871ef5d527bff235ef25906c4a739540
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517003"
---
# <a name="update-printsettings"></a><span data-ttu-id="eba4a-103">更新 printSettings</span><span class="sxs-lookup"><span data-stu-id="eba4a-103">Update printSettings</span></span>
<span data-ttu-id="eba4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="eba4a-105">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="eba4a-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="eba4a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eba4a-106">Permissions</span></span>
<span data-ttu-id="eba4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eba4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eba4a-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="eba4a-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="eba4a-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="eba4a-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="eba4a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eba4a-111">Permission type</span></span> | <span data-ttu-id="eba4a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eba4a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eba4a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eba4a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="eba4a-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba4a-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="eba4a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eba4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eba4a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eba4a-116">Not Supported.</span></span>|
|<span data-ttu-id="eba4a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eba4a-117">Application</span></span>|<span data-ttu-id="eba4a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eba4a-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eba4a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eba4a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="eba4a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eba4a-120">Request headers</span></span>
|<span data-ttu-id="eba4a-121">名称</span><span class="sxs-lookup"><span data-stu-id="eba4a-121">Name</span></span>|<span data-ttu-id="eba4a-122">说明</span><span class="sxs-lookup"><span data-stu-id="eba4a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eba4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eba4a-123">Authorization</span></span>|<span data-ttu-id="eba4a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eba4a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eba4a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba4a-126">Content-Type</span></span>|<span data-ttu-id="eba4a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eba4a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eba4a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="eba4a-129">Request body</span></span>
<span data-ttu-id="eba4a-130">在请求正文中，提供应更新的相关 [printSettings](../resources/printsettings.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="eba4a-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="eba4a-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="eba4a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eba4a-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="eba4a-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eba4a-133">属性</span><span class="sxs-lookup"><span data-stu-id="eba4a-133">Property</span></span>     | <span data-ttu-id="eba4a-134">类型</span><span class="sxs-lookup"><span data-stu-id="eba4a-134">Type</span></span>        | <span data-ttu-id="eba4a-135">Description</span><span class="sxs-lookup"><span data-stu-id="eba4a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eba4a-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="eba4a-136">documentConversionEnabled</span></span>|<span data-ttu-id="eba4a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="eba4a-137">Boolean</span></span>|<span data-ttu-id="eba4a-138">指定是否对租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="eba4a-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="eba4a-139">如果启用文档转换，通用打印服务将自动将文档转换为与打印机设备兼容的格式 (例如，XPS 转换为 PDF) 时。</span><span class="sxs-lookup"><span data-stu-id="eba4a-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="eba4a-140">响应</span><span class="sxs-lookup"><span data-stu-id="eba4a-140">Response</span></span>

<span data-ttu-id="eba4a-141">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="eba4a-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eba4a-142">示例</span><span class="sxs-lookup"><span data-stu-id="eba4a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eba4a-143">请求</span><span class="sxs-lookup"><span data-stu-id="eba4a-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="eba4a-144">响应</span><span class="sxs-lookup"><span data-stu-id="eba4a-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 204 No Content
```

