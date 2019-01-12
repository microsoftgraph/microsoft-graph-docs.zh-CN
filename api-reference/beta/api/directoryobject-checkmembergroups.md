---
title: 检查成员组
description: 检查这些组的组和从该列表中的返回指定列表中的成员资格
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93ff0a0cb215e489490e50bde40f56e5b562be95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971086"
---
# <a name="check-member-groups"></a><span data-ttu-id="d908f-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="d908f-103">Check member groups</span></span>

> <span data-ttu-id="d908f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d908f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d908f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d908f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d908f-106">检查成员资格组和从该列表中的返回指定列表中指定的用户、 组、 服务主体或目录对象所属的这些组。</span><span class="sxs-lookup"><span data-stu-id="d908f-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="d908f-107">可传递此函数。</span><span class="sxs-lookup"><span data-stu-id="d908f-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d908f-108">权限</span><span class="sxs-lookup"><span data-stu-id="d908f-108">Permissions</span></span>
<span data-ttu-id="d908f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d908f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d908f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d908f-111">Permission type</span></span>      | <span data-ttu-id="d908f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d908f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d908f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d908f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d908f-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d908f-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="d908f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d908f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d908f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d908f-116">Not supported.</span></span>    |
|<span data-ttu-id="d908f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d908f-117">Application</span></span> | <span data-ttu-id="d908f-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d908f-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d908f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d908f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="d908f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d908f-120">Request headers</span></span>
| <span data-ttu-id="d908f-121">名称</span><span class="sxs-lookup"><span data-stu-id="d908f-121">Name</span></span>       | <span data-ttu-id="d908f-122">类型</span><span class="sxs-lookup"><span data-stu-id="d908f-122">Type</span></span> | <span data-ttu-id="d908f-123">说明</span><span class="sxs-lookup"><span data-stu-id="d908f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d908f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d908f-124">Authorization</span></span>  | <span data-ttu-id="d908f-125">string</span><span class="sxs-lookup"><span data-stu-id="d908f-125">string</span></span>  | <span data-ttu-id="d908f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d908f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d908f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d908f-128">Content-Type</span></span>  | <span data-ttu-id="d908f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d908f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d908f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d908f-130">Request body</span></span>
<span data-ttu-id="d908f-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d908f-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d908f-132">参数</span><span class="sxs-lookup"><span data-stu-id="d908f-132">Parameter</span></span>    | <span data-ttu-id="d908f-133">类型</span><span class="sxs-lookup"><span data-stu-id="d908f-133">Type</span></span>   |<span data-ttu-id="d908f-134">说明</span><span class="sxs-lookup"><span data-stu-id="d908f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d908f-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="d908f-135">groupIds</span></span>|<span data-ttu-id="d908f-136">String</span><span class="sxs-lookup"><span data-stu-id="d908f-136">String</span></span>|<span data-ttu-id="d908f-p105">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="d908f-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="d908f-139">响应</span><span class="sxs-lookup"><span data-stu-id="d908f-139">Response</span></span>

<span data-ttu-id="d908f-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="d908f-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d908f-141">示例</span><span class="sxs-lookup"><span data-stu-id="d908f-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d908f-142">请求</span><span class="sxs-lookup"><span data-stu-id="d908f-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d908f-143">响应</span><span class="sxs-lookup"><span data-stu-id="d908f-143">Response</span></span>
<span data-ttu-id="d908f-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d908f-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
