---
title: 创建 groupLifecyclePolicy
description: 新建 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9ba07aeaa0d9aabf63fb6d8598fb238e03c3586d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522677"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="80f3c-103">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="80f3c-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f3c-104">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="80f3c-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80f3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="80f3c-105">Permissions</span></span>

<span data-ttu-id="80f3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="80f3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="80f3c-108">Permission type</span></span>      | <span data-ttu-id="80f3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80f3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80f3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80f3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80f3c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f3c-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="80f3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f3c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="80f3c-113">Not supported</span></span> |
|<span data-ttu-id="80f3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="80f3c-114">Application</span></span> |  <span data-ttu-id="80f3c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f3c-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80f3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="80f3c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="80f3c-117">Request headers</span></span>

| <span data-ttu-id="80f3c-118">名称</span><span class="sxs-lookup"><span data-stu-id="80f3c-118">Name</span></span> | <span data-ttu-id="80f3c-119">说明</span><span class="sxs-lookup"><span data-stu-id="80f3c-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="80f3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="80f3c-120">Authorization</span></span> | <span data-ttu-id="80f3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80f3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80f3c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80f3c-123">Content-Type</span></span>  | <span data-ttu-id="80f3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80f3c-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="80f3c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80f3c-125">Request body</span></span>
<span data-ttu-id="80f3c-126">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80f3c-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="80f3c-127">响应</span><span class="sxs-lookup"><span data-stu-id="80f3c-127">Response</span></span>

<span data-ttu-id="80f3c-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80f3c-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f3c-129">示例</span><span class="sxs-lookup"><span data-stu-id="80f3c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80f3c-130">请求</span><span class="sxs-lookup"><span data-stu-id="80f3c-130">Request</span></span>

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
<span data-ttu-id="80f3c-131">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80f3c-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="80f3c-132">响应</span><span class="sxs-lookup"><span data-stu-id="80f3c-132">Response</span></span>

<span data-ttu-id="80f3c-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80f3c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
