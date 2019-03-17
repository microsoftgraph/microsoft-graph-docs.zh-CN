---
title: 创建 schedulingGroup
description: 创建新的 schedulingGroup。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: da8d93f955fcac0530d093a33d9018930767e710
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657516"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="27227-103">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="27227-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27227-104">创建新的[schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="27227-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27227-105">权限</span><span class="sxs-lookup"><span data-stu-id="27227-105">Permissions</span></span>

<span data-ttu-id="27227-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27227-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="27227-108">Permission type</span></span>      | <span data-ttu-id="27227-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27227-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27227-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27227-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27227-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27227-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="27227-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27227-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27227-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="27227-113">Not supported.</span></span>    |
|<span data-ttu-id="27227-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="27227-114">Application</span></span> | <span data-ttu-id="27227-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27227-115">Not supported.</span></span> |

> <span data-ttu-id="27227-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="27227-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="27227-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="27227-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="27227-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27227-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="27227-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="27227-119">Request headers</span></span>

| <span data-ttu-id="27227-120">标头</span><span class="sxs-lookup"><span data-stu-id="27227-120">Header</span></span>       | <span data-ttu-id="27227-121">值</span><span class="sxs-lookup"><span data-stu-id="27227-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27227-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27227-122">Authorization</span></span>  | <span data-ttu-id="27227-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27227-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27227-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27227-125">Content-Type</span></span>  | <span data-ttu-id="27227-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27227-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="27227-127">响应</span><span class="sxs-lookup"><span data-stu-id="27227-127">Response</span></span>

<span data-ttu-id="27227-128">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27227-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27227-129">示例</span><span class="sxs-lookup"><span data-stu-id="27227-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="27227-130">请求</span><span class="sxs-lookup"><span data-stu-id="27227-130">Request</span></span>

<span data-ttu-id="27227-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="27227-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="27227-132">响应</span><span class="sxs-lookup"><span data-stu-id="27227-132">Response</span></span>

<span data-ttu-id="27227-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="27227-133">The following is an example of the response.</span></span> 

><span data-ttu-id="27227-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="27227-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
