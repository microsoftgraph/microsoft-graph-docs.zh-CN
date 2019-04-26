---
title: 列出现有同步模板
description: 列出与给定应用程序或服务主体相关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: 385d7b34c3efd1c7236b7d57dc1239acb328421e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330146"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="6b416-103">列出现有同步模板</span><span class="sxs-lookup"><span data-stu-id="6b416-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b416-104">列出与给定应用程序或服务主体相关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="6b416-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b416-105">权限</span><span class="sxs-lookup"><span data-stu-id="6b416-105">Permissions</span></span>
<span data-ttu-id="6b416-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b416-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b416-108">Permission type</span></span>                        | <span data-ttu-id="6b416-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b416-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b416-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b416-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="6b416-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b416-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6b416-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b416-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6b416-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b416-113">Not supported.</span></span>|
|<span data-ttu-id="6b416-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b416-114">Application</span></span>                            |<span data-ttu-id="6b416-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b416-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="6b416-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b416-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="6b416-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b416-117">Request headers</span></span>

| <span data-ttu-id="6b416-118">名称</span><span class="sxs-lookup"><span data-stu-id="6b416-118">Name</span></span>           | <span data-ttu-id="6b416-119">类型</span><span class="sxs-lookup"><span data-stu-id="6b416-119">Type</span></span>    | <span data-ttu-id="6b416-120">说明</span><span class="sxs-lookup"><span data-stu-id="6b416-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6b416-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b416-121">Authorization</span></span>  | <span data-ttu-id="6b416-122">string</span><span class="sxs-lookup"><span data-stu-id="6b416-122">string</span></span>  | <span data-ttu-id="6b416-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b416-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b416-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b416-125">Request body</span></span>

<span data-ttu-id="6b416-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b416-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6b416-127">响应</span><span class="sxs-lookup"><span data-stu-id="6b416-127">Response</span></span>

<span data-ttu-id="6b416-128">如果成功, 此方法在响应`200 OK`正文中返回[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象的响应代码和集合。</span><span class="sxs-lookup"><span data-stu-id="6b416-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="6b416-129">示例</span><span class="sxs-lookup"><span data-stu-id="6b416-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6b416-130">请求</span><span class="sxs-lookup"><span data-stu-id="6b416-130">Request</span></span>
<span data-ttu-id="6b416-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="6b416-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="6b416-132">响应</span><span class="sxs-lookup"><span data-stu-id="6b416-132">Response</span></span>
<span data-ttu-id="6b416-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="6b416-133">The following is an example of a response.</span></span>
><span data-ttu-id="6b416-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b416-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6b416-135">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="6b416-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
