---
title: 更新 synchronizationTemplate
description: Update (override) 与给定应用程序关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: 152186afd9f7b7cce2a04170de7148d454525d80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536860"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="d31b6-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="d31b6-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d31b6-104">Update (override) 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="d31b6-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d31b6-105">权限</span><span class="sxs-lookup"><span data-stu-id="d31b6-105">Permissions</span></span>
<span data-ttu-id="d31b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d31b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d31b6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d31b6-108">Permission type</span></span>                        | <span data-ttu-id="d31b6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d31b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d31b6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d31b6-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="d31b6-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d31b6-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d31b6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d31b6-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d31b6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d31b6-113">Not supported.</span></span>|
|<span data-ttu-id="d31b6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d31b6-114">Application</span></span>                            |<span data-ttu-id="d31b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d31b6-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="d31b6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d31b6-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="d31b6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d31b6-117">Request headers</span></span>

| <span data-ttu-id="d31b6-118">名称</span><span class="sxs-lookup"><span data-stu-id="d31b6-118">Name</span></span>           | <span data-ttu-id="d31b6-119">类型</span><span class="sxs-lookup"><span data-stu-id="d31b6-119">Type</span></span>    | <span data-ttu-id="d31b6-120">说明</span><span class="sxs-lookup"><span data-stu-id="d31b6-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d31b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d31b6-121">Authorization</span></span>  | <span data-ttu-id="d31b6-122">string</span><span class="sxs-lookup"><span data-stu-id="d31b6-122">string</span></span>  | <span data-ttu-id="d31b6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d31b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d31b6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d31b6-125">Request body</span></span>

<span data-ttu-id="d31b6-126">在请求正文中, 提供[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="d31b6-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="d31b6-127">请确保提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="d31b6-127">Make sure all properties are provided.</span></span> <span data-ttu-id="d31b6-128">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="d31b6-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="d31b6-129">响应</span><span class="sxs-lookup"><span data-stu-id="d31b6-129">Response</span></span>

<span data-ttu-id="d31b6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d31b6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="d31b6-132">示例</span><span class="sxs-lookup"><span data-stu-id="d31b6-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="d31b6-133">请求</span><span class="sxs-lookup"><span data-stu-id="d31b6-133">Request</span></span>
<span data-ttu-id="d31b6-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d31b6-134">The following is an example of a request.</span></span> 

><span data-ttu-id="d31b6-135">**注意:** 为了提高可读性, 此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="d31b6-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="d31b6-136">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="d31b6-136">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="d31b6-137">响应</span><span class="sxs-lookup"><span data-stu-id="d31b6-137">Response</span></span>
<span data-ttu-id="d31b6-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d31b6-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
