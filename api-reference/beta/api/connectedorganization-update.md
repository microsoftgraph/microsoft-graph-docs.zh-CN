---
title: 更新 connectedOrganization 对象
description: 更新 connectedOrganization 对象。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c8662beaba895c8d9b29af3cb584307e3f6fe05
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509999"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="59b48-103">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="59b48-103">Update connectedOrganization</span></span>

<span data-ttu-id="59b48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59b48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59b48-105">更新[connectedOrganization](../resources/connectedorganization.md)对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="59b48-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="59b48-106">权限</span><span class="sxs-lookup"><span data-stu-id="59b48-106">Permissions</span></span>
<span data-ttu-id="59b48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b48-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="59b48-109">Permission type</span></span>|<span data-ttu-id="59b48-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59b48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59b48-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59b48-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59b48-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b48-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="59b48-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59b48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b48-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59b48-114">Not supported.</span></span> |
|<span data-ttu-id="59b48-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="59b48-115">Application</span></span>                            | <span data-ttu-id="59b48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59b48-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59b48-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59b48-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="59b48-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="59b48-118">Request headers</span></span>
|<span data-ttu-id="59b48-119">名称</span><span class="sxs-lookup"><span data-stu-id="59b48-119">Name</span></span>|<span data-ttu-id="59b48-120">说明</span><span class="sxs-lookup"><span data-stu-id="59b48-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59b48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59b48-121">Authorization</span></span>|<span data-ttu-id="59b48-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59b48-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59b48-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59b48-124">Content-Type</span></span>|<span data-ttu-id="59b48-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="59b48-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59b48-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59b48-127">Request body</span></span>
<span data-ttu-id="59b48-128">在请求正文中，提供[connectedOrganization](../resources/connectedorganization.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59b48-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="59b48-129">下表显示了在更新[connectedOrganization](../resources/connectedorganization.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59b48-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="59b48-130">属性</span><span class="sxs-lookup"><span data-stu-id="59b48-130">Property</span></span>|<span data-ttu-id="59b48-131">类型</span><span class="sxs-lookup"><span data-stu-id="59b48-131">Type</span></span>|<span data-ttu-id="59b48-132">说明</span><span class="sxs-lookup"><span data-stu-id="59b48-132">Description</span></span>|
|:---|:---|:---|
| `displayName`  |`String` | <span data-ttu-id="59b48-133">连接的组织名称。</span><span class="sxs-lookup"><span data-stu-id="59b48-133">The connected organization name.</span></span>  |
| `description`  |`String` | <span data-ttu-id="59b48-134">连接的组织说明。</span><span class="sxs-lookup"><span data-stu-id="59b48-134">The connected organization description.</span></span> |

## <a name="response"></a><span data-ttu-id="59b48-135">响应</span><span class="sxs-lookup"><span data-stu-id="59b48-135">Response</span></span>

<span data-ttu-id="59b48-136">如果成功，此方法 `204 Accepted` 在响应正文中返回响应代码和[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59b48-136">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59b48-137">示例</span><span class="sxs-lookup"><span data-stu-id="59b48-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59b48-138">请求</span><span class="sxs-lookup"><span data-stu-id="59b48-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectedorganization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```


### <a name="response"></a><span data-ttu-id="59b48-139">响应</span><span class="sxs-lookup"><span data-stu-id="59b48-139">Response</span></span>
<span data-ttu-id="59b48-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="59b48-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 204 Accepted
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
