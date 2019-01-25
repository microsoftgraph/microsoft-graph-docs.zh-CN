---
title: 获取成员对象
description: " 返回所有的组、 管理单元和目录角色的用户、 组、 服务主体或目录对象的成员。 可传递此函数。 "
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2425ef4f94188c39b0964f627dd05a98b3ad5ab2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527946"
---
# <a name="get-member-objects"></a><span data-ttu-id="d35be-104">获取成员对象</span><span class="sxs-lookup"><span data-stu-id="d35be-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="d35be-105">返回所有的组、 管理单元和目录角色的用户、 组、 服务主体或目录对象的成员。</span><span class="sxs-lookup"><span data-stu-id="d35be-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="d35be-106">可传递此函数。</span><span class="sxs-lookup"><span data-stu-id="d35be-106">This function is transitive.</span></span> 
 > <span data-ttu-id="d35be-107">注意：只有用户可以是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="d35be-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="d35be-108">权限</span><span class="sxs-lookup"><span data-stu-id="d35be-108">Permissions</span></span>
<span data-ttu-id="d35be-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d35be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d35be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d35be-111">Permission type</span></span>      | <span data-ttu-id="d35be-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d35be-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d35be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d35be-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d35be-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d35be-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="d35be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d35be-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d35be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d35be-116">Not supported.</span></span>    |
|<span data-ttu-id="d35be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d35be-117">Application</span></span> | <span data-ttu-id="d35be-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d35be-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d35be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d35be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d35be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d35be-120">Request headers</span></span>
| <span data-ttu-id="d35be-121">名称</span><span class="sxs-lookup"><span data-stu-id="d35be-121">Name</span></span>       | <span data-ttu-id="d35be-122">类型</span><span class="sxs-lookup"><span data-stu-id="d35be-122">Type</span></span> | <span data-ttu-id="d35be-123">说明</span><span class="sxs-lookup"><span data-stu-id="d35be-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d35be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d35be-124">Authorization</span></span>  | <span data-ttu-id="d35be-125">string</span><span class="sxs-lookup"><span data-stu-id="d35be-125">string</span></span>  | <span data-ttu-id="d35be-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d35be-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d35be-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d35be-128">Content-Type</span></span>  | <span data-ttu-id="d35be-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d35be-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d35be-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d35be-130">Request body</span></span>
<span data-ttu-id="d35be-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d35be-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d35be-132">参数</span><span class="sxs-lookup"><span data-stu-id="d35be-132">Parameter</span></span>    | <span data-ttu-id="d35be-133">类型</span><span class="sxs-lookup"><span data-stu-id="d35be-133">Type</span></span>   |<span data-ttu-id="d35be-134">说明</span><span class="sxs-lookup"><span data-stu-id="d35be-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d35be-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d35be-135">securityEnabledOnly</span></span>|<span data-ttu-id="d35be-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d35be-136">Boolean</span></span>| <span data-ttu-id="d35be-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="d35be-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="d35be-139">响应</span><span class="sxs-lookup"><span data-stu-id="d35be-139">Response</span></span>

<span data-ttu-id="d35be-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="d35be-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d35be-141">示例</span><span class="sxs-lookup"><span data-stu-id="d35be-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d35be-142">请求</span><span class="sxs-lookup"><span data-stu-id="d35be-142">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="d35be-143">响应</span><span class="sxs-lookup"><span data-stu-id="d35be-143">Response</span></span>
<span data-ttu-id="d35be-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d35be-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
