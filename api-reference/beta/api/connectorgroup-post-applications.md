---
title: 创建应用程序
description: 使用此 API 创建新的应用程序。
localization_priority: Normal
ms.openlocfilehash: e9d1c76f153c27ab3df24a93b44a570c2c1d836a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824666"
---
# <a name="create-application"></a><span data-ttu-id="c4aad-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="c4aad-103">Create application</span></span>

> <span data-ttu-id="c4aad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c4aad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4aad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c4aad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4aad-106">使用此 API 创建新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c4aad-106">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4aad-107">权限</span><span class="sxs-lookup"><span data-stu-id="c4aad-107">Permissions</span></span>
<span data-ttu-id="c4aad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4aad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4aad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4aad-110">Permission type</span></span>      | <span data-ttu-id="c4aad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4aad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4aad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4aad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4aad-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4aad-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4aad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4aad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4aad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4aad-115">Not supported.</span></span>    |
|<span data-ttu-id="c4aad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4aad-116">Application</span></span> | <span data-ttu-id="c4aad-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4aad-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4aad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4aad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="c4aad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4aad-119">Request headers</span></span>
| <span data-ttu-id="c4aad-120">名称</span><span class="sxs-lookup"><span data-stu-id="c4aad-120">Name</span></span>       | <span data-ttu-id="c4aad-121">说明</span><span class="sxs-lookup"><span data-stu-id="c4aad-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4aad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4aad-122">Authorization</span></span>  | <span data-ttu-id="c4aad-123">持有者。</span><span class="sxs-lookup"><span data-stu-id="c4aad-123">Bearer.</span></span> <span data-ttu-id="c4aad-124">是否必需</span><span class="sxs-lookup"><span data-stu-id="c4aad-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4aad-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4aad-125">Request body</span></span>
<span data-ttu-id="c4aad-126">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4aad-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c4aad-127">响应</span><span class="sxs-lookup"><span data-stu-id="c4aad-127">Response</span></span>

<span data-ttu-id="c4aad-128">如果成功，此方法返回`201 Created`响应正文中的响应代码和[应用程序](../resources/application.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4aad-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4aad-129">示例</span><span class="sxs-lookup"><span data-stu-id="c4aad-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4aad-130">请求</span><span class="sxs-lookup"><span data-stu-id="c4aad-130">Request</span></span>
<span data-ttu-id="c4aad-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4aad-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="c4aad-132">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4aad-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c4aad-133">响应</span><span class="sxs-lookup"><span data-stu-id="c4aad-133">Response</span></span>
<span data-ttu-id="c4aad-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4aad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
