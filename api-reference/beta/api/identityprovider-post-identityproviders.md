---
title: 创建 identityProvider
description: 通过指定显示名称、 identityProvider 类型、 客户端 ID 和客户端机密创建新 identityProvider。
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514647"
---
# <a name="create-identityprovider"></a><span data-ttu-id="95123-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="95123-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95123-104">通过指定显示名称、 identityProvider 类型、 客户端 ID 和客户端机密创建新[identityProvider](../resources/identityprovider.md) 。</span><span class="sxs-lookup"><span data-stu-id="95123-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="95123-105">权限</span><span class="sxs-lookup"><span data-stu-id="95123-105">Permissions</span></span>

<span data-ttu-id="95123-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95123-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="95123-108">Permission type</span></span>      | <span data-ttu-id="95123-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95123-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95123-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95123-110">Delegated (work or school account)</span></span>|<span data-ttu-id="95123-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95123-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="95123-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95123-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="95123-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="95123-113">Not supported.</span></span>|
|<span data-ttu-id="95123-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="95123-114">Application</span></span>|<span data-ttu-id="95123-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95123-115">Not supported.</span></span>|

<span data-ttu-id="95123-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="95123-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="95123-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95123-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="95123-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="95123-118">Request headers</span></span>

|<span data-ttu-id="95123-119">名称</span><span class="sxs-lookup"><span data-stu-id="95123-119">Name</span></span>|<span data-ttu-id="95123-120">说明</span><span class="sxs-lookup"><span data-stu-id="95123-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="95123-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95123-121">Authorization</span></span>|<span data-ttu-id="95123-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95123-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="95123-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95123-124">Content-Type</span></span>|<span data-ttu-id="95123-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="95123-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95123-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95123-127">Request body</span></span>

<span data-ttu-id="95123-128">在请求正文中，提供[identityProvider](../resources/identityprovider.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95123-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="95123-129">下表中列出的所有属性都是必需的。</span><span class="sxs-lookup"><span data-stu-id="95123-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="95123-130">属性</span><span class="sxs-lookup"><span data-stu-id="95123-130">Property</span></span>|<span data-ttu-id="95123-131">类型</span><span class="sxs-lookup"><span data-stu-id="95123-131">Type</span></span>|<span data-ttu-id="95123-132">说明</span><span class="sxs-lookup"><span data-stu-id="95123-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95123-133">clientId</span><span class="sxs-lookup"><span data-stu-id="95123-133">clientId</span></span>|<span data-ttu-id="95123-134">String</span><span class="sxs-lookup"><span data-stu-id="95123-134">String</span></span>|<span data-ttu-id="95123-135">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="95123-135">The client ID for the application.</span></span> <span data-ttu-id="95123-136">这是注册的标识提供程序的应用程序时所获得的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="95123-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="95123-137">client_secret</span><span class="sxs-lookup"><span data-stu-id="95123-137">clientSecret</span></span>|<span data-ttu-id="95123-138">String</span><span class="sxs-lookup"><span data-stu-id="95123-138">String</span></span>|<span data-ttu-id="95123-139">应用程序客户端机密。</span><span class="sxs-lookup"><span data-stu-id="95123-139">The client secret for the application.</span></span> <span data-ttu-id="95123-140">这是注册的标识提供程序的应用程序时所获得的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="95123-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="95123-141">name</span><span class="sxs-lookup"><span data-stu-id="95123-141">name</span></span>|<span data-ttu-id="95123-142">String</span><span class="sxs-lookup"><span data-stu-id="95123-142">String</span></span>|<span data-ttu-id="95123-143">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="95123-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="95123-144">type</span><span class="sxs-lookup"><span data-stu-id="95123-144">type</span></span>|<span data-ttu-id="95123-145">String</span><span class="sxs-lookup"><span data-stu-id="95123-145">String</span></span>|<span data-ttu-id="95123-146">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="95123-146">The identity provider type.</span></span> <span data-ttu-id="95123-147">它必须是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="95123-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="95123-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="95123-148">Microsoft</span></span><li/><span data-ttu-id="95123-149">Google</span><span class="sxs-lookup"><span data-stu-id="95123-149">Google</span></span><li/><span data-ttu-id="95123-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="95123-150">Amazon</span></span><li/><span data-ttu-id="95123-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="95123-151">LinkedIn</span></span><li/><span data-ttu-id="95123-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="95123-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="95123-153">响应</span><span class="sxs-lookup"><span data-stu-id="95123-153">Response</span></span>

<span data-ttu-id="95123-154">如果成功，此方法返回`201 Created`响应正文中的响应代码和[identityProvider](../resources/identityprovider.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95123-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="95123-155">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="95123-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="95123-156">示例</span><span class="sxs-lookup"><span data-stu-id="95123-156">Example</span></span>

<span data-ttu-id="95123-157">下面的示例创建**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="95123-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="95123-158">请求</span><span class="sxs-lookup"><span data-stu-id="95123-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="95123-159">响应</span><span class="sxs-lookup"><span data-stu-id="95123-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
