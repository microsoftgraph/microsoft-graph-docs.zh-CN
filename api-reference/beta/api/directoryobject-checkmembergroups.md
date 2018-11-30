---
title: 检查成员组
description: 检查这些组的组和从该列表中的返回指定列表中的成员资格
ms.openlocfilehash: b7baccd19b9d5a84ecbca4d75bca053eb51bc3f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041360"
---
# <a name="check-member-groups"></a><span data-ttu-id="5d5d7-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="5d5d7-103">Check member groups</span></span>

> <span data-ttu-id="5d5d7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d5d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d5d7-106">检查成员资格组和从该列表中的返回指定列表中指定的用户、 组、 服务主体或目录对象所属的这些组。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="5d5d7-107">可传递此函数。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d5d7-108">权限</span><span class="sxs-lookup"><span data-stu-id="5d5d7-108">Permissions</span></span>
<span data-ttu-id="5d5d7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5d5d7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d5d7-111">Permission type</span></span>      | <span data-ttu-id="5d5d7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d5d7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5d5d7-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d5d7-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="5d5d7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d5d7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-116">Not supported.</span></span>    |
|<span data-ttu-id="5d5d7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d5d7-117">Application</span></span> | <span data-ttu-id="5d5d7-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d5d7-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d5d7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d5d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="5d5d7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d5d7-120">Request headers</span></span>
| <span data-ttu-id="5d5d7-121">名称</span><span class="sxs-lookup"><span data-stu-id="5d5d7-121">Name</span></span>       | <span data-ttu-id="5d5d7-122">类型</span><span class="sxs-lookup"><span data-stu-id="5d5d7-122">Type</span></span> | <span data-ttu-id="5d5d7-123">说明</span><span class="sxs-lookup"><span data-stu-id="5d5d7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d5d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d5d7-124">Authorization</span></span>  | <span data-ttu-id="5d5d7-125">string</span><span class="sxs-lookup"><span data-stu-id="5d5d7-125">string</span></span>  | <span data-ttu-id="5d5d7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d5d7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d5d7-128">Content-Type</span></span>  | <span data-ttu-id="5d5d7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5d5d7-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d5d7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d5d7-130">Request body</span></span>
<span data-ttu-id="5d5d7-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d5d7-132">参数</span><span class="sxs-lookup"><span data-stu-id="5d5d7-132">Parameter</span></span>    | <span data-ttu-id="5d5d7-133">类型</span><span class="sxs-lookup"><span data-stu-id="5d5d7-133">Type</span></span>   |<span data-ttu-id="5d5d7-134">说明</span><span class="sxs-lookup"><span data-stu-id="5d5d7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d5d7-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="5d5d7-135">groupIds</span></span>|<span data-ttu-id="5d5d7-136">String</span><span class="sxs-lookup"><span data-stu-id="5d5d7-136">String</span></span>|<span data-ttu-id="5d5d7-p105">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="5d5d7-139">响应</span><span class="sxs-lookup"><span data-stu-id="5d5d7-139">Response</span></span>

<span data-ttu-id="5d5d7-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d5d7-141">示例</span><span class="sxs-lookup"><span data-stu-id="5d5d7-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d5d7-142">请求</span><span class="sxs-lookup"><span data-stu-id="5d5d7-142">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5d5d7-143">响应</span><span class="sxs-lookup"><span data-stu-id="5d5d7-143">Response</span></span>
<span data-ttu-id="5d5d7-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d5d7-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
