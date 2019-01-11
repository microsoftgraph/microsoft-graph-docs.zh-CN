---
title: 列表同步的现有模板
description: 列出与给定应用程序或服务主体关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: 49e9e257322886fe294807207276f8b6d6919909
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839436"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="4bdcd-103">列表同步的现有模板</span><span class="sxs-lookup"><span data-stu-id="4bdcd-103">List existing synchronization templates</span></span>

> <span data-ttu-id="4bdcd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bdcd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bdcd-106">列出与给定应用程序或服务主体关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-106">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bdcd-107">权限</span><span class="sxs-lookup"><span data-stu-id="4bdcd-107">Permissions</span></span>
<span data-ttu-id="4bdcd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bdcd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bdcd-110">Permission type</span></span>                        | <span data-ttu-id="4bdcd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bdcd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bdcd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bdcd-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4bdcd-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdcd-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4bdcd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bdcd-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4bdcd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-115">Not supported.</span></span>|
|<span data-ttu-id="4bdcd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bdcd-116">Application</span></span>                            |<span data-ttu-id="4bdcd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="4bdcd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bdcd-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="4bdcd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bdcd-119">Request headers</span></span>

| <span data-ttu-id="4bdcd-120">名称</span><span class="sxs-lookup"><span data-stu-id="4bdcd-120">Name</span></span>           | <span data-ttu-id="4bdcd-121">类型</span><span class="sxs-lookup"><span data-stu-id="4bdcd-121">Type</span></span>    | <span data-ttu-id="4bdcd-122">说明</span><span class="sxs-lookup"><span data-stu-id="4bdcd-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4bdcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bdcd-123">Authorization</span></span>  | <span data-ttu-id="4bdcd-124">string</span><span class="sxs-lookup"><span data-stu-id="4bdcd-124">string</span></span>  | <span data-ttu-id="4bdcd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bdcd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bdcd-127">Request body</span></span>

<span data-ttu-id="4bdcd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4bdcd-129">响应</span><span class="sxs-lookup"><span data-stu-id="4bdcd-129">Response</span></span>

<span data-ttu-id="4bdcd-130">如果成功，此方法返回`200 OK`响应代码和 acollection 的响应正文中的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-130">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="4bdcd-131">示例</span><span class="sxs-lookup"><span data-stu-id="4bdcd-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4bdcd-132">请求</span><span class="sxs-lookup"><span data-stu-id="4bdcd-132">Request</span></span>
<span data-ttu-id="4bdcd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="4bdcd-134">响应</span><span class="sxs-lookup"><span data-stu-id="4bdcd-134">Response</span></span>
<span data-ttu-id="4bdcd-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-135">The following is an example of a response.</span></span>
><span data-ttu-id="4bdcd-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4bdcd-137">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="4bdcd-137">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
