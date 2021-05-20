---
title: 更新 mobileDeviceManagementPolicy
description: 更新移动设备管理对象的属性。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 112c76fbb240e8ff30b47b47de3f6d2966af8a11
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547326"
---
# <a name="update-mobiledevicemanagementpolicy"></a><span data-ttu-id="52f74-103">更新 mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="52f74-103">Update mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="52f74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52f74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f74-105">更新 [mobilityManagementPolicy 对象](../resources/mobilitymanagementpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="52f74-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f74-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="52f74-106">Permissions</span></span>

<span data-ttu-id="52f74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52f74-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52f74-109">Permission type</span></span>|<span data-ttu-id="52f74-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52f74-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52f74-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52f74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52f74-112">Policy.Read.All、Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f74-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="52f74-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52f74-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f74-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52f74-114">Not supported.</span></span>|
|<span data-ttu-id="52f74-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52f74-115">Application</span></span> | <span data-ttu-id="52f74-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52f74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f74-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52f74-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="52f74-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="52f74-118">Request headers</span></span>

|<span data-ttu-id="52f74-119">名称</span><span class="sxs-lookup"><span data-stu-id="52f74-119">Name</span></span>|<span data-ttu-id="52f74-120">说明</span><span class="sxs-lookup"><span data-stu-id="52f74-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52f74-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52f74-121">Authorization</span></span>|<span data-ttu-id="52f74-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52f74-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="52f74-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f74-124">Content-Type</span></span>|<span data-ttu-id="52f74-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="52f74-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="52f74-127">Request body</span></span>

<span data-ttu-id="52f74-128">在请求正文中，提供 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52f74-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="52f74-129">在请求正文中，提供下面列出的应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="52f74-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="52f74-130">**注意：** 不能将 `PATCH` 操作用于 `appliesTo` 其他属性。</span><span class="sxs-lookup"><span data-stu-id="52f74-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="52f74-131">属性</span><span class="sxs-lookup"><span data-stu-id="52f74-131">Property</span></span>|<span data-ttu-id="52f74-132">类型</span><span class="sxs-lookup"><span data-stu-id="52f74-132">Type</span></span>|<span data-ttu-id="52f74-133">说明</span><span class="sxs-lookup"><span data-stu-id="52f74-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f74-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="52f74-134">appliesTo</span></span>|<span data-ttu-id="52f74-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="52f74-135">policyScope</span></span>|<span data-ttu-id="52f74-136">确定此策略设置应用于的组。</span><span class="sxs-lookup"><span data-stu-id="52f74-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="52f74-137">可能的值是 `none` `all` `selected` **：、、重要：** `selected` 指定此属性时不能使用。</span><span class="sxs-lookup"><span data-stu-id="52f74-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="52f74-138">使用 [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) 添加特定组。</span><span class="sxs-lookup"><span data-stu-id="52f74-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) to add specific groups.</span></span> <span data-ttu-id="52f74-139">使用 `all` 将删除任何现有组。</span><span class="sxs-lookup"><span data-stu-id="52f74-139">Using `all` will remove any existing groups.</span></span>|
|<span data-ttu-id="52f74-140">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="52f74-140">complianceUrl</span></span>|<span data-ttu-id="52f74-141">String</span><span class="sxs-lookup"><span data-stu-id="52f74-141">String</span></span>|<span data-ttu-id="52f74-142">移动管理应用程序的合规性 URL</span><span class="sxs-lookup"><span data-stu-id="52f74-142">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="52f74-143">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="52f74-143">discoveryUrl</span></span>|<span data-ttu-id="52f74-144">String</span><span class="sxs-lookup"><span data-stu-id="52f74-144">String</span></span>|<span data-ttu-id="52f74-145">移动管理应用程序的发现 URL</span><span class="sxs-lookup"><span data-stu-id="52f74-145">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="52f74-146">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="52f74-146">termsOfUseUrl</span></span>|<span data-ttu-id="52f74-147">String</span><span class="sxs-lookup"><span data-stu-id="52f74-147">String</span></span>|<span data-ttu-id="52f74-148">移动管理应用程序的使用条款 URL</span><span class="sxs-lookup"><span data-stu-id="52f74-148">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="52f74-149">响应</span><span class="sxs-lookup"><span data-stu-id="52f74-149">Response</span></span>

<span data-ttu-id="52f74-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52f74-150">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52f74-151">示例</span><span class="sxs-lookup"><span data-stu-id="52f74-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52f74-152">请求</span><span class="sxs-lookup"><span data-stu-id="52f74-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a><span data-ttu-id="52f74-153">响应</span><span class="sxs-lookup"><span data-stu-id="52f74-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
