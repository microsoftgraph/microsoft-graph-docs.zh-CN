---
title: 更新 b2cIdentityUserFlow
description: 更新 b2cIdentityUserFlow 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc030097cbfc6e57cbe841f6a0dd98660d1a12f7
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706229"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="dbff5-103">更新 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="dbff5-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="dbff5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbff5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbff5-105">更新 [b2cIdentityUserFlow 对象](../resources/b2cidentityuserflow.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="dbff5-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbff5-106">权限</span><span class="sxs-lookup"><span data-stu-id="dbff5-106">Permissions</span></span>

<span data-ttu-id="dbff5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbff5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbff5-109">Permission type</span></span>      | <span data-ttu-id="dbff5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbff5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbff5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbff5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbff5-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbff5-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="dbff5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbff5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dbff5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbff5-114">Not supported.</span></span>|
|<span data-ttu-id="dbff5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbff5-115">Application</span></span>|<span data-ttu-id="dbff5-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbff5-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="dbff5-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="dbff5-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="dbff5-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="dbff5-118">Global administrator</span></span>
* <span data-ttu-id="dbff5-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="dbff5-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="dbff5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbff5-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dbff5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbff5-121">Request headers</span></span>

|<span data-ttu-id="dbff5-122">名称</span><span class="sxs-lookup"><span data-stu-id="dbff5-122">Name</span></span>|<span data-ttu-id="dbff5-123">说明</span><span class="sxs-lookup"><span data-stu-id="dbff5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dbff5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbff5-124">Authorization</span></span>|<span data-ttu-id="dbff5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbff5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dbff5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbff5-127">Content-Type</span></span>|<span data-ttu-id="dbff5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="dbff5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbff5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbff5-130">Request body</span></span>

<span data-ttu-id="dbff5-131">在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbff5-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="dbff5-132">下表显示创建 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)后可以更新的属性。</span><span class="sxs-lookup"><span data-stu-id="dbff5-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="dbff5-133">属性</span><span class="sxs-lookup"><span data-stu-id="dbff5-133">Property</span></span>|<span data-ttu-id="dbff5-134">类型</span><span class="sxs-lookup"><span data-stu-id="dbff5-134">Type</span></span>|<span data-ttu-id="dbff5-135">说明</span><span class="sxs-lookup"><span data-stu-id="dbff5-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbff5-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="dbff5-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="dbff5-137">布尔</span><span class="sxs-lookup"><span data-stu-id="dbff5-137">Boolean</span></span>|<span data-ttu-id="dbff5-138">该属性确定是否在 B2C 用户流中启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="dbff5-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="dbff5-139">默认情况下，不会为 B2C 用户流启用语言自定义。</span><span class="sxs-lookup"><span data-stu-id="dbff5-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="dbff5-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="dbff5-140">defaultLanguageTag</span></span>|<span data-ttu-id="dbff5-141">字符串</span><span class="sxs-lookup"><span data-stu-id="dbff5-141">String</span></span>|<span data-ttu-id="dbff5-142">指示在请求中未指定标记时所使用的 b2cIdentityUserFlow `ui_locale` 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="dbff5-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="dbff5-143">此字段符合[RFC 5646。](https://tools.ietf.org/html/rfc5646)</span><span class="sxs-lookup"><span data-stu-id="dbff5-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="dbff5-144">响应</span><span class="sxs-lookup"><span data-stu-id="dbff5-144">Response</span></span>

<span data-ttu-id="dbff5-145">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新 [的 b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbff5-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbff5-146">示例</span><span class="sxs-lookup"><span data-stu-id="dbff5-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dbff5-147">请求</span><span class="sxs-lookup"><span data-stu-id="dbff5-147">Request</span></span>

<span data-ttu-id="dbff5-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dbff5-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```

### <a name="response"></a><span data-ttu-id="dbff5-149">响应</span><span class="sxs-lookup"><span data-stu-id="dbff5-149">Response</span></span>

<span data-ttu-id="dbff5-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dbff5-150">The following is an example of the response.</span></span>

<span data-ttu-id="dbff5-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dbff5-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
