---
title: 获取成员组
description: 返回指定的用户、 组、 服务主体或目录对象是成员的所有组。 可传递此函数。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53d52ae4d877f3367fa6b08ea73cefa1fea492cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935862"
---
# <a name="get-member-groups"></a><span data-ttu-id="6eb11-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="6eb11-104">Get member groups</span></span>

> <span data-ttu-id="6eb11-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6eb11-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb11-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6eb11-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6eb11-107">返回指定的用户、 组、 服务主体或目录对象是成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="6eb11-107">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="6eb11-108">可传递此函数。</span><span class="sxs-lookup"><span data-stu-id="6eb11-108">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6eb11-109">权限</span><span class="sxs-lookup"><span data-stu-id="6eb11-109">Permissions</span></span>
<span data-ttu-id="6eb11-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eb11-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6eb11-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eb11-112">Permission type</span></span>      | <span data-ttu-id="6eb11-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eb11-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6eb11-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb11-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb11-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6eb11-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="6eb11-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb11-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb11-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb11-117">Not supported.</span></span>    |
|<span data-ttu-id="6eb11-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6eb11-118">Application</span></span> | <span data-ttu-id="6eb11-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6eb11-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eb11-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eb11-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="6eb11-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eb11-121">Request headers</span></span>
| <span data-ttu-id="6eb11-122">名称</span><span class="sxs-lookup"><span data-stu-id="6eb11-122">Name</span></span>       | <span data-ttu-id="6eb11-123">类型</span><span class="sxs-lookup"><span data-stu-id="6eb11-123">Type</span></span> | <span data-ttu-id="6eb11-124">说明</span><span class="sxs-lookup"><span data-stu-id="6eb11-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6eb11-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb11-125">Authorization</span></span>  | <span data-ttu-id="6eb11-126">string</span><span class="sxs-lookup"><span data-stu-id="6eb11-126">string</span></span>  | <span data-ttu-id="6eb11-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6eb11-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6eb11-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6eb11-129">Content-Type</span></span>  | <span data-ttu-id="6eb11-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb11-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6eb11-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eb11-131">Request body</span></span>
<span data-ttu-id="6eb11-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6eb11-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6eb11-133">参数</span><span class="sxs-lookup"><span data-stu-id="6eb11-133">Parameter</span></span>    | <span data-ttu-id="6eb11-134">类型</span><span class="sxs-lookup"><span data-stu-id="6eb11-134">Type</span></span>   |<span data-ttu-id="6eb11-135">说明</span><span class="sxs-lookup"><span data-stu-id="6eb11-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6eb11-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6eb11-136">securityEnabledOnly</span></span>|<span data-ttu-id="6eb11-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eb11-137">Boolean</span></span>| <span data-ttu-id="6eb11-p106">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="6eb11-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="6eb11-140">响应</span><span class="sxs-lookup"><span data-stu-id="6eb11-140">Response</span></span>

<span data-ttu-id="6eb11-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="6eb11-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb11-142">示例</span><span class="sxs-lookup"><span data-stu-id="6eb11-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6eb11-143">请求</span><span class="sxs-lookup"><span data-stu-id="6eb11-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="6eb11-144">响应</span><span class="sxs-lookup"><span data-stu-id="6eb11-144">Response</span></span>
<span data-ttu-id="6eb11-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6eb11-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
