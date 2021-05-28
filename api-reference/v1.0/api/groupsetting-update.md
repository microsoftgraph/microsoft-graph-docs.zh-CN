---
title: 更新组设置
description: 更新特定组设置对象的属性。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a2a504aa8c736df33ef35d3bd131b6329fd499c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679755"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="54fa7-103">更新组设置</span><span class="sxs-lookup"><span data-stu-id="54fa7-103">Update a group setting</span></span>

<span data-ttu-id="54fa7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54fa7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54fa7-105">为租户范围的组设置或特定组设置更新[groupSetting](../resources/groupsetting.md)对象的属性。 [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="54fa7-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="54fa7-106">权限</span><span class="sxs-lookup"><span data-stu-id="54fa7-106">Permissions</span></span>

<span data-ttu-id="54fa7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54fa7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54fa7-109">Permission type</span></span>      | <span data-ttu-id="54fa7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54fa7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54fa7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54fa7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54fa7-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54fa7-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54fa7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54fa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54fa7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="54fa7-114">Not supported.</span></span>    |
|<span data-ttu-id="54fa7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="54fa7-115">Application</span></span> | <span data-ttu-id="54fa7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54fa7-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54fa7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54fa7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="54fa7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="54fa7-118">Request headers</span></span>
| <span data-ttu-id="54fa7-119">名称</span><span class="sxs-lookup"><span data-stu-id="54fa7-119">Name</span></span> | <span data-ttu-id="54fa7-120">说明</span><span class="sxs-lookup"><span data-stu-id="54fa7-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="54fa7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54fa7-121">Authorization</span></span>  | <span data-ttu-id="54fa7-122">{token}。</span><span class="sxs-lookup"><span data-stu-id="54fa7-122">{token}.</span></span> <span data-ttu-id="54fa7-123">必需。</span><span class="sxs-lookup"><span data-stu-id="54fa7-123">Required.</span></span> |
| <span data-ttu-id="54fa7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54fa7-124">Content-Type</span></span>  | <span data-ttu-id="54fa7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54fa7-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54fa7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54fa7-126">Request body</span></span>
<span data-ttu-id="54fa7-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="54fa7-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="54fa7-128">属性</span><span class="sxs-lookup"><span data-stu-id="54fa7-128">Property</span></span> | <span data-ttu-id="54fa7-129">类型</span><span class="sxs-lookup"><span data-stu-id="54fa7-129">Type</span></span> | <span data-ttu-id="54fa7-130">说明</span><span class="sxs-lookup"><span data-stu-id="54fa7-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="54fa7-131">值</span><span class="sxs-lookup"><span data-stu-id="54fa7-131">values</span></span> | <span data-ttu-id="54fa7-132">[settingValue](../resources/settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54fa7-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="54fa7-133">更新的值集。</span><span class="sxs-lookup"><span data-stu-id="54fa7-133">The updated set of values.</span></span> <span data-ttu-id="54fa7-134">必须包含整个集合集。</span><span class="sxs-lookup"><span data-stu-id="54fa7-134">You must include the entire collection set.</span></span> <span data-ttu-id="54fa7-135">无法更新一组值。</span><span class="sxs-lookup"><span data-stu-id="54fa7-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="54fa7-136">响应</span><span class="sxs-lookup"><span data-stu-id="54fa7-136">Response</span></span>

<span data-ttu-id="54fa7-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54fa7-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="54fa7-138">示例</span><span class="sxs-lookup"><span data-stu-id="54fa7-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="54fa7-139">示例 1：更新租户范围的组设置</span><span class="sxs-lookup"><span data-stu-id="54fa7-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="54fa7-140">此示例中， `{id}` 是租户范围内 groupSetting 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="54fa7-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="54fa7-141">请求</span><span class="sxs-lookup"><span data-stu-id="54fa7-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54fa7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="54fa7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenant_setting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json

{
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "EnableMIPLabels",
      "value": "false"
    },
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "false"
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
      "value": "false"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "true"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": ""
    },
    {
      "name": "AllowToAddGuests",
      "value": "true"
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
      "value": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="54fa7-143">C#</span><span class="sxs-lookup"><span data-stu-id="54fa7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-setting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54fa7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54fa7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-setting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54fa7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54fa7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-setting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54fa7-146">Java</span><span class="sxs-lookup"><span data-stu-id="54fa7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-setting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54fa7-147">响应</span><span class="sxs-lookup"><span data-stu-id="54fa7-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="54fa7-148">示例 2：更新特定组设置</span><span class="sxs-lookup"><span data-stu-id="54fa7-148">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="54fa7-149">此示例中，请求的第一个为组的标识符，第二 `{id}` `{id}` 个为 groupSetting 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="54fa7-149">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="54fa7-150">请求</span><span class="sxs-lookup"><span data-stu-id="54fa7-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54fa7-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="54fa7-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/settings/{id}
Content-type: application/json

{
  "displayName": "GroupSettings",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
            "name": "AllowToAddGuests",
            "value": "false"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="54fa7-152">C#</span><span class="sxs-lookup"><span data-stu-id="54fa7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54fa7-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54fa7-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54fa7-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54fa7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54fa7-155">Java</span><span class="sxs-lookup"><span data-stu-id="54fa7-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54fa7-156">响应</span><span class="sxs-lookup"><span data-stu-id="54fa7-156">Response</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

