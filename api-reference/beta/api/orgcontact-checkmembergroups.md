---
title: 'orgContact: checkMemberGroups'
description: 要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9345a1879789a3f96a3eb6b2bbe4d636c75ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523783"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="048bf-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="048bf-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="048bf-105">权限</span><span class="sxs-lookup"><span data-stu-id="048bf-105">Permissions</span></span>
<span data-ttu-id="048bf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="048bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="048bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="048bf-108">Permission type</span></span>      | <span data-ttu-id="048bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="048bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="048bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="048bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="048bf-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="048bf-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="048bf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="048bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="048bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="048bf-113">Not supported.</span></span>    |
|<span data-ttu-id="048bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="048bf-114">Application</span></span> | <span data-ttu-id="048bf-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="048bf-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="048bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="048bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="048bf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="048bf-117">Request headers</span></span>
| <span data-ttu-id="048bf-118">名称</span><span class="sxs-lookup"><span data-stu-id="048bf-118">Name</span></span>       | <span data-ttu-id="048bf-119">类型</span><span class="sxs-lookup"><span data-stu-id="048bf-119">Type</span></span> | <span data-ttu-id="048bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="048bf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="048bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="048bf-121">Authorization</span></span>  | <span data-ttu-id="048bf-122">string</span><span class="sxs-lookup"><span data-stu-id="048bf-122">string</span></span>  | <span data-ttu-id="048bf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="048bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="048bf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="048bf-125">Request body</span></span>
<span data-ttu-id="048bf-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="048bf-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="048bf-127">参数</span><span class="sxs-lookup"><span data-stu-id="048bf-127">Parameter</span></span>    | <span data-ttu-id="048bf-128">类型</span><span class="sxs-lookup"><span data-stu-id="048bf-128">Type</span></span>   |<span data-ttu-id="048bf-129">说明</span><span class="sxs-lookup"><span data-stu-id="048bf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="048bf-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="048bf-130">groupIds</span></span>|<span data-ttu-id="048bf-131">String</span><span class="sxs-lookup"><span data-stu-id="048bf-131">String</span></span>||

## <a name="response"></a><span data-ttu-id="048bf-132">响应</span><span class="sxs-lookup"><span data-stu-id="048bf-132">Response</span></span>

<span data-ttu-id="048bf-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="048bf-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="048bf-134">示例</span><span class="sxs-lookup"><span data-stu-id="048bf-134">Example</span></span>
<span data-ttu-id="048bf-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="048bf-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="048bf-136">请求</span><span class="sxs-lookup"><span data-stu-id="048bf-136">Request</span></span>
<span data-ttu-id="048bf-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="048bf-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="048bf-138">响应</span><span class="sxs-lookup"><span data-stu-id="048bf-138">Response</span></span>
<span data-ttu-id="048bf-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="048bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
