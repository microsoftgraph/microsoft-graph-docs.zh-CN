---
title: 创建 connectedOrganization
description: 创建新的 connectedOrganization。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 47e8ba9564b1810da99e212ab9832142656d18f0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509998"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="9eec8-103">创建 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="9eec8-103">Create connectedOrganization</span></span>

<span data-ttu-id="9eec8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eec8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eec8-105">创建新的[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9eec8-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9eec8-106">权限</span><span class="sxs-lookup"><span data-stu-id="9eec8-106">Permissions</span></span>

<span data-ttu-id="9eec8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9eec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eec8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9eec8-109">Permission type</span></span>|<span data-ttu-id="9eec8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9eec8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="9eec8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9eec8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9eec8-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eec8-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9eec8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9eec8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eec8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eec8-114">Not supported.</span></span> |
| <span data-ttu-id="9eec8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9eec8-115">Application</span></span>                            | <span data-ttu-id="9eec8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eec8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eec8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9eec8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="9eec8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9eec8-118">Request headers</span></span>

|<span data-ttu-id="9eec8-119">名称</span><span class="sxs-lookup"><span data-stu-id="9eec8-119">Name</span></span>|<span data-ttu-id="9eec8-120">说明</span><span class="sxs-lookup"><span data-stu-id="9eec8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9eec8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eec8-121">Authorization</span></span>|<span data-ttu-id="9eec8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9eec8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9eec8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9eec8-124">Content-Type</span></span>|<span data-ttu-id="9eec8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9eec8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eec8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9eec8-127">Request body</span></span>
<span data-ttu-id="9eec8-128">在请求正文中，提供[connectedOrganization](../resources/connectedorganization.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9eec8-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="9eec8-129">下表显示创建[connectedOrganization](../resources/connectedorganization.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9eec8-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="9eec8-130">属性</span><span class="sxs-lookup"><span data-stu-id="9eec8-130">Property</span></span>|<span data-ttu-id="9eec8-131">类型</span><span class="sxs-lookup"><span data-stu-id="9eec8-131">Type</span></span>|<span data-ttu-id="9eec8-132">说明</span><span class="sxs-lookup"><span data-stu-id="9eec8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eec8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9eec8-133">displayName</span></span>|<span data-ttu-id="9eec8-134">String</span><span class="sxs-lookup"><span data-stu-id="9eec8-134">String</span></span>|<span data-ttu-id="9eec8-135">连接的组织名称。</span><span class="sxs-lookup"><span data-stu-id="9eec8-135">The connected organization name.</span></span> |
|<span data-ttu-id="9eec8-136">说明</span><span class="sxs-lookup"><span data-stu-id="9eec8-136">description</span></span>|<span data-ttu-id="9eec8-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9eec8-137">String</span></span>|<span data-ttu-id="9eec8-138">连接的组织说明。</span><span class="sxs-lookup"><span data-stu-id="9eec8-138">The connected organization description.</span></span>|
|<span data-ttu-id="9eec8-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="9eec8-139">identitySources</span></span>|<span data-ttu-id="9eec8-140">[identitySource](../resources/identitysource.md)集合</span><span class="sxs-lookup"><span data-stu-id="9eec8-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="9eec8-141">包含一个元素（此连接组织中的初始标识源）的集合。</span><span class="sxs-lookup"><span data-stu-id="9eec8-141">A collection with one element, the initial identity source in this connected organization.</span></span>|


## <a name="response"></a><span data-ttu-id="9eec8-142">响应</span><span class="sxs-lookup"><span data-stu-id="9eec8-142">Response</span></span>

<span data-ttu-id="9eec8-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9eec8-143">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9eec8-144">示例</span><span class="sxs-lookup"><span data-stu-id="9eec8-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9eec8-145">请求</span><span class="sxs-lookup"><span data-stu-id="9eec8-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9eec8-146">响应</span><span class="sxs-lookup"><span data-stu-id="9eec8-146">Response</span></span>
<span data-ttu-id="9eec8-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9eec8-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-06-08T20:13:53.7099947Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
