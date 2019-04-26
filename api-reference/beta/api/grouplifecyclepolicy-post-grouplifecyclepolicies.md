---
title: 创建 groupLifecyclePolicy
description: 新建 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 311b2b5e499bcfea0622f457d76c7a60aaef2741
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328486"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="ade4a-103">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ade4a-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade4a-104">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="ade4a-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ade4a-105">权限</span><span class="sxs-lookup"><span data-stu-id="ade4a-105">Permissions</span></span>

<span data-ttu-id="ade4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ade4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ade4a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ade4a-108">Permission type</span></span>      | <span data-ttu-id="ade4a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ade4a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ade4a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ade4a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ade4a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade4a-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ade4a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ade4a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ade4a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="ade4a-113">Not supported</span></span> |
|<span data-ttu-id="ade4a-114">Application</span><span class="sxs-lookup"><span data-stu-id="ade4a-114">Application</span></span> |  <span data-ttu-id="ade4a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade4a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ade4a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ade4a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="ade4a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ade4a-117">Request headers</span></span>

| <span data-ttu-id="ade4a-118">名称</span><span class="sxs-lookup"><span data-stu-id="ade4a-118">Name</span></span> | <span data-ttu-id="ade4a-119">说明</span><span class="sxs-lookup"><span data-stu-id="ade4a-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ade4a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade4a-120">Authorization</span></span> | <span data-ttu-id="ade4a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ade4a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ade4a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ade4a-123">Content-Type</span></span>  | <span data-ttu-id="ade4a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ade4a-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ade4a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ade4a-125">Request body</span></span>
<span data-ttu-id="ade4a-126">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade4a-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ade4a-127">响应</span><span class="sxs-lookup"><span data-stu-id="ade4a-127">Response</span></span>

<span data-ttu-id="ade4a-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ade4a-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade4a-129">示例</span><span class="sxs-lookup"><span data-stu-id="ade4a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ade4a-130">请求</span><span class="sxs-lookup"><span data-stu-id="ade4a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="ade4a-131">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade4a-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ade4a-132">响应</span><span class="sxs-lookup"><span data-stu-id="ade4a-132">Response</span></span>

<span data-ttu-id="ade4a-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ade4a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
