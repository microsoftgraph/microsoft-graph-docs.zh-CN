---
title: 创建应用程序
description: 使用此 API 创建新的应用程序。
localization_priority: Normal
ms.openlocfilehash: 350e5f0fcb45f7404a670c1a0af4e4ddd02a97c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514241"
---
# <a name="create-application"></a><span data-ttu-id="1a7fc-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="1a7fc-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a7fc-104">使用此 API 创建新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a7fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="1a7fc-105">Permissions</span></span>
<span data-ttu-id="1a7fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a7fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a7fc-108">Permission type</span></span>      | <span data-ttu-id="1a7fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a7fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a7fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a7fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a7fc-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a7fc-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a7fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a7fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a7fc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-113">Not supported.</span></span>    |
|<span data-ttu-id="1a7fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a7fc-114">Application</span></span> | <span data-ttu-id="1a7fc-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a7fc-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a7fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a7fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="1a7fc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a7fc-117">Request headers</span></span>
| <span data-ttu-id="1a7fc-118">名称</span><span class="sxs-lookup"><span data-stu-id="1a7fc-118">Name</span></span>       | <span data-ttu-id="1a7fc-119">说明</span><span class="sxs-lookup"><span data-stu-id="1a7fc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a7fc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a7fc-120">Authorization</span></span>  | <span data-ttu-id="1a7fc-121">Bearer </span><span class="sxs-lookup"><span data-stu-id="1a7fc-121">Bearer.</span></span> <span data-ttu-id="1a7fc-122">必需</span><span class="sxs-lookup"><span data-stu-id="1a7fc-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7fc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a7fc-123">Request body</span></span>
<span data-ttu-id="1a7fc-124">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a7fc-125">响应</span><span class="sxs-lookup"><span data-stu-id="1a7fc-125">Response</span></span>

<span data-ttu-id="1a7fc-126">如果成功，此方法返回`201 Created`响应正文中的响应代码和[应用程序](../resources/application.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a7fc-127">示例</span><span class="sxs-lookup"><span data-stu-id="1a7fc-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a7fc-128">请求</span><span class="sxs-lookup"><span data-stu-id="1a7fc-128">Request</span></span>
<span data-ttu-id="1a7fc-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="1a7fc-130">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1a7fc-131">响应</span><span class="sxs-lookup"><span data-stu-id="1a7fc-131">Response</span></span>
<span data-ttu-id="1a7fc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a7fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
