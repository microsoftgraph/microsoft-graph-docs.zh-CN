---
title: 更新组设置
description: 更新特定组设置对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1ebea83f26bd3fcf54e530e80173c830fbde7ba8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941686"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="112ca-103">更新组设置</span><span class="sxs-lookup"><span data-stu-id="112ca-103">Update a group setting</span></span>

<span data-ttu-id="112ca-104">更新特定组设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="112ca-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="112ca-105">权限</span><span class="sxs-lookup"><span data-stu-id="112ca-105">Permissions</span></span>

<span data-ttu-id="112ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="112ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="112ca-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="112ca-108">Permission type</span></span>      | <span data-ttu-id="112ca-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="112ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="112ca-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="112ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="112ca-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="112ca-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="112ca-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="112ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="112ca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="112ca-113">Not supported.</span></span>    |
|<span data-ttu-id="112ca-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="112ca-114">Application</span></span> | <span data-ttu-id="112ca-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="112ca-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="112ca-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="112ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="112ca-117">更新租户范围或组特定设置。</span><span class="sxs-lookup"><span data-stu-id="112ca-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="112ca-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="112ca-118">Optional request headers</span></span>
| <span data-ttu-id="112ca-119">名称</span><span class="sxs-lookup"><span data-stu-id="112ca-119">Name</span></span> | <span data-ttu-id="112ca-120">说明</span><span class="sxs-lookup"><span data-stu-id="112ca-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="112ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="112ca-121">Authorization</span></span>  | <span data-ttu-id="112ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="112ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="112ca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="112ca-124">Content-Type</span></span>  | <span data-ttu-id="112ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="112ca-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="112ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="112ca-126">Request body</span></span>
<span data-ttu-id="112ca-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="112ca-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="112ca-128">属性</span><span class="sxs-lookup"><span data-stu-id="112ca-128">Property</span></span> | <span data-ttu-id="112ca-129">类型</span><span class="sxs-lookup"><span data-stu-id="112ca-129">Type</span></span> | <span data-ttu-id="112ca-130">说明</span><span class="sxs-lookup"><span data-stu-id="112ca-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="112ca-131">values</span><span class="sxs-lookup"><span data-stu-id="112ca-131">values</span></span> | <span data-ttu-id="112ca-132">settingValue 集合</span><span class="sxs-lookup"><span data-stu-id="112ca-132">settingValue collection</span></span> | <span data-ttu-id="112ca-p103">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="112ca-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="112ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="112ca-136">Response</span></span>

<span data-ttu-id="112ca-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="112ca-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="112ca-138">示例</span><span class="sxs-lookup"><span data-stu-id="112ca-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="112ca-139">请求</span><span class="sxs-lookup"><span data-stu-id="112ca-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="112ca-140">响应</span><span class="sxs-lookup"><span data-stu-id="112ca-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
