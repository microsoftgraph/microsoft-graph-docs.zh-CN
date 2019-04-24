---
title: 检查成员组
description: 检查指定组列表中的成员身份, 并从该列表返回这些组
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53c89a6dd6fb0c16e0df7c6035ed0667c227787d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455189"
---
# <a name="check-member-groups"></a><span data-ttu-id="b0785-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="b0785-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0785-104">检查指定组列表中的成员身份, 并从该列表返回指定用户、组、服务主体或目录对象所属的组。</span><span class="sxs-lookup"><span data-stu-id="b0785-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="b0785-105">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b0785-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0785-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0785-106">Permissions</span></span>
<span data-ttu-id="b0785-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0785-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0785-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0785-109">Permission type</span></span>      | <span data-ttu-id="b0785-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0785-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0785-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0785-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0785-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0785-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="b0785-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0785-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0785-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0785-114">Not supported.</span></span>    |
|<span data-ttu-id="b0785-115">Application</span><span class="sxs-lookup"><span data-stu-id="b0785-115">Application</span></span> | <span data-ttu-id="b0785-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0785-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0785-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0785-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b0785-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0785-118">Request headers</span></span>
| <span data-ttu-id="b0785-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0785-119">Name</span></span>       | <span data-ttu-id="b0785-120">类型</span><span class="sxs-lookup"><span data-stu-id="b0785-120">Type</span></span> | <span data-ttu-id="b0785-121">说明</span><span class="sxs-lookup"><span data-stu-id="b0785-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0785-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0785-122">Authorization</span></span>  | <span data-ttu-id="b0785-123">string</span><span class="sxs-lookup"><span data-stu-id="b0785-123">string</span></span>  | <span data-ttu-id="b0785-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0785-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0785-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0785-126">Content-Type</span></span>  | <span data-ttu-id="b0785-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0785-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b0785-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0785-128">Request body</span></span>
<span data-ttu-id="b0785-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b0785-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b0785-130">参数</span><span class="sxs-lookup"><span data-stu-id="b0785-130">Parameter</span></span>    | <span data-ttu-id="b0785-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0785-131">Type</span></span>   |<span data-ttu-id="b0785-132">描述</span><span class="sxs-lookup"><span data-stu-id="b0785-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0785-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="b0785-133">groupIds</span></span>|<span data-ttu-id="b0785-134">String</span><span class="sxs-lookup"><span data-stu-id="b0785-134">String</span></span>|<span data-ttu-id="b0785-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="b0785-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b0785-137">响应</span><span class="sxs-lookup"><span data-stu-id="b0785-137">Response</span></span>

<span data-ttu-id="b0785-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b0785-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0785-139">示例</span><span class="sxs-lookup"><span data-stu-id="b0785-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0785-140">请求</span><span class="sxs-lookup"><span data-stu-id="b0785-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="b0785-141">响应</span><span class="sxs-lookup"><span data-stu-id="b0785-141">Response</span></span>
<span data-ttu-id="b0785-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0785-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
