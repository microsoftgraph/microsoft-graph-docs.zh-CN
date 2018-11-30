---
title: 获取成员对象
description: " 返回所有的组、 管理单元和目录角色的用户、 组、 服务主体或目录对象的成员。 可传递此函数。 "
ms.openlocfilehash: f1bf68276fc4ed7d4694fadc73a08ae328047222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041658"
---
# <a name="get-member-objects"></a><span data-ttu-id="b103c-104">获取成员对象</span><span class="sxs-lookup"><span data-stu-id="b103c-104">Get member objects</span></span>

> <span data-ttu-id="b103c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b103c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b103c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b103c-106">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="b103c-107">返回所有的组、 管理单元和目录角色的用户、 组、 服务主体或目录对象的成员。</span><span class="sxs-lookup"><span data-stu-id="b103c-107">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="b103c-108">可传递此函数。</span><span class="sxs-lookup"><span data-stu-id="b103c-108">This function is transitive.</span></span> 
 > <span data-ttu-id="b103c-109">注意：只有用户可以是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="b103c-109">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="b103c-110">权限</span><span class="sxs-lookup"><span data-stu-id="b103c-110">Permissions</span></span>
<span data-ttu-id="b103c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b103c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b103c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b103c-113">Permission type</span></span>      | <span data-ttu-id="b103c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b103c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b103c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b103c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b103c-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b103c-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="b103c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b103c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b103c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b103c-118">Not supported.</span></span>    |
|<span data-ttu-id="b103c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b103c-119">Application</span></span> | <span data-ttu-id="b103c-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b103c-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b103c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b103c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="b103c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b103c-122">Request headers</span></span>
| <span data-ttu-id="b103c-123">名称</span><span class="sxs-lookup"><span data-stu-id="b103c-123">Name</span></span>       | <span data-ttu-id="b103c-124">类型</span><span class="sxs-lookup"><span data-stu-id="b103c-124">Type</span></span> | <span data-ttu-id="b103c-125">说明</span><span class="sxs-lookup"><span data-stu-id="b103c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b103c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b103c-126">Authorization</span></span>  | <span data-ttu-id="b103c-127">string</span><span class="sxs-lookup"><span data-stu-id="b103c-127">string</span></span>  | <span data-ttu-id="b103c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b103c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b103c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b103c-130">Content-Type</span></span>  | <span data-ttu-id="b103c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b103c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b103c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b103c-132">Request body</span></span>
<span data-ttu-id="b103c-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b103c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b103c-134">参数</span><span class="sxs-lookup"><span data-stu-id="b103c-134">Parameter</span></span>    | <span data-ttu-id="b103c-135">类型</span><span class="sxs-lookup"><span data-stu-id="b103c-135">Type</span></span>   |<span data-ttu-id="b103c-136">说明</span><span class="sxs-lookup"><span data-stu-id="b103c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b103c-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b103c-137">securityEnabledOnly</span></span>|<span data-ttu-id="b103c-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="b103c-138">Boolean</span></span>| <span data-ttu-id="b103c-p106">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="b103c-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="b103c-141">响应</span><span class="sxs-lookup"><span data-stu-id="b103c-141">Response</span></span>

<span data-ttu-id="b103c-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b103c-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b103c-143">示例</span><span class="sxs-lookup"><span data-stu-id="b103c-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b103c-144">请求</span><span class="sxs-lookup"><span data-stu-id="b103c-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="b103c-145">响应</span><span class="sxs-lookup"><span data-stu-id="b103c-145">Response</span></span>
<span data-ttu-id="b103c-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b103c-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
