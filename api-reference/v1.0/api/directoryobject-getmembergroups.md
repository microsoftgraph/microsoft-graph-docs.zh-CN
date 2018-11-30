---
title: 获取成员组
description: 返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。
ms.openlocfilehash: 370de10e1bba582270290877ba508ec4eebf47ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011015"
---
# <a name="get-member-groups"></a><span data-ttu-id="e6532-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="e6532-104">Get member groups</span></span>

<span data-ttu-id="e6532-p102">返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="e6532-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6532-107">权限</span><span class="sxs-lookup"><span data-stu-id="e6532-107">Permissions</span></span>
<span data-ttu-id="e6532-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6532-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6532-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6532-110">Permission type</span></span>      | <span data-ttu-id="e6532-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6532-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6532-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6532-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6532-113">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6532-113">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="e6532-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6532-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6532-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6532-115">Not supported.</span></span>    |
|<span data-ttu-id="e6532-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6532-116">Application</span></span> | <span data-ttu-id="e6532-117">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6532-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6532-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6532-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="e6532-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6532-119">Request headers</span></span>
| <span data-ttu-id="e6532-120">名称</span><span class="sxs-lookup"><span data-stu-id="e6532-120">Name</span></span>       | <span data-ttu-id="e6532-121">类型</span><span class="sxs-lookup"><span data-stu-id="e6532-121">Type</span></span> | <span data-ttu-id="e6532-122">说明</span><span class="sxs-lookup"><span data-stu-id="e6532-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6532-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6532-123">Authorization</span></span>  | <span data-ttu-id="e6532-124">string</span><span class="sxs-lookup"><span data-stu-id="e6532-124">string</span></span>  | <span data-ttu-id="e6532-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6532-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6532-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6532-127">Content-Type</span></span>   | <span data-ttu-id="e6532-128">string</span><span class="sxs-lookup"><span data-stu-id="e6532-128">string</span></span>  | <span data-ttu-id="e6532-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e6532-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6532-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6532-130">Request body</span></span>
<span data-ttu-id="e6532-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e6532-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6532-132">参数</span><span class="sxs-lookup"><span data-stu-id="e6532-132">Parameter</span></span>    | <span data-ttu-id="e6532-133">类型</span><span class="sxs-lookup"><span data-stu-id="e6532-133">Type</span></span>   |<span data-ttu-id="e6532-134">说明</span><span class="sxs-lookup"><span data-stu-id="e6532-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6532-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e6532-135">securityEnabledOnly</span></span>|<span data-ttu-id="e6532-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6532-136">Boolean</span></span>| <span data-ttu-id="e6532-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="e6532-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="e6532-139">响应</span><span class="sxs-lookup"><span data-stu-id="e6532-139">Response</span></span>

<span data-ttu-id="e6532-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="e6532-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6532-141">示例</span><span class="sxs-lookup"><span data-stu-id="e6532-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e6532-142">请求</span><span class="sxs-lookup"><span data-stu-id="e6532-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="e6532-143">响应</span><span class="sxs-lookup"><span data-stu-id="e6532-143">Response</span></span>
<span data-ttu-id="e6532-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6532-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
