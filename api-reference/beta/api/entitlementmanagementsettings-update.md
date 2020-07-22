---
title: 更新 entitlementManagementSettings
description: 更新 entitlementManagementSettings 对象以更改其一个或多个属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23d37c089e9c81939ba9342a7f5747dd979b8bec
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225066"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="6505b-103">更新 entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6505b-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="6505b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6505b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6505b-105">更新现有[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="6505b-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="6505b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6505b-106">Permissions</span></span>
<span data-ttu-id="6505b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6505b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6505b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6505b-109">Permission type</span></span>                        | <span data-ttu-id="6505b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6505b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6505b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6505b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6505b-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6505b-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="6505b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6505b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6505b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6505b-114">Not supported.</span></span> |
|<span data-ttu-id="6505b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6505b-115">Application</span></span>                            | <span data-ttu-id="6505b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6505b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6505b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6505b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="6505b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6505b-118">Request headers</span></span>
| <span data-ttu-id="6505b-119">名称</span><span class="sxs-lookup"><span data-stu-id="6505b-119">Name</span></span>         | <span data-ttu-id="6505b-120">说明</span><span class="sxs-lookup"><span data-stu-id="6505b-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="6505b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6505b-121">Authorization</span></span> | <span data-ttu-id="6505b-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="6505b-122">Bearer \{token\}.</span></span> <span data-ttu-id="6505b-123">必需。</span><span class="sxs-lookup"><span data-stu-id="6505b-123">Required.</span></span> |
| <span data-ttu-id="6505b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6505b-124">Content-Type</span></span>  | <span data-ttu-id="6505b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6505b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6505b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6505b-127">Request body</span></span>
<span data-ttu-id="6505b-128">在请求正文中，提供[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6505b-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6505b-129">响应</span><span class="sxs-lookup"><span data-stu-id="6505b-129">Response</span></span>
<span data-ttu-id="6505b-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6505b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6505b-131">示例</span><span class="sxs-lookup"><span data-stu-id="6505b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6505b-132">请求</span><span class="sxs-lookup"><span data-stu-id="6505b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```

### <a name="response"></a><span data-ttu-id="6505b-133">响应</span><span class="sxs-lookup"><span data-stu-id="6505b-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
