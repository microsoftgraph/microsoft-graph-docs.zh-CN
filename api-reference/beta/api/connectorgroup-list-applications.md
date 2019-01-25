---
title: 应用程序列表
description: 检索与 connectorGroup 关联的应用程序对象的列表。
localization_priority: Normal
ms.openlocfilehash: 47be81d4f154d87865113fa02b04a58151545507
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519358"
---
# <a name="list-applications"></a><span data-ttu-id="56dae-103">应用程序列表</span><span class="sxs-lookup"><span data-stu-id="56dae-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56dae-104">检索与 connectorGroup 关联的应用程序对象的列表。</span><span class="sxs-lookup"><span data-stu-id="56dae-104">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="56dae-105">权限</span><span class="sxs-lookup"><span data-stu-id="56dae-105">Permissions</span></span>
<span data-ttu-id="56dae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56dae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56dae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56dae-108">Permission type</span></span>      | <span data-ttu-id="56dae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56dae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56dae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56dae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56dae-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56dae-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56dae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56dae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56dae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56dae-113">Not supported.</span></span>    |
|<span data-ttu-id="56dae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="56dae-114">Application</span></span> | <span data-ttu-id="56dae-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56dae-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56dae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56dae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56dae-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56dae-117">Optional query parameters</span></span>
<span data-ttu-id="56dae-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56dae-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56dae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="56dae-119">Request headers</span></span>
| <span data-ttu-id="56dae-120">名称</span><span class="sxs-lookup"><span data-stu-id="56dae-120">Name</span></span>      |<span data-ttu-id="56dae-121">说明</span><span class="sxs-lookup"><span data-stu-id="56dae-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56dae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="56dae-122">Authorization</span></span>  | <span data-ttu-id="56dae-123">Bearer </span><span class="sxs-lookup"><span data-stu-id="56dae-123">Bearer.</span></span> <span data-ttu-id="56dae-124">必需</span><span class="sxs-lookup"><span data-stu-id="56dae-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="56dae-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="56dae-125">Request body</span></span>
<span data-ttu-id="56dae-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56dae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56dae-127">响应</span><span class="sxs-lookup"><span data-stu-id="56dae-127">Response</span></span>

<span data-ttu-id="56dae-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[应用程序](../resources/application.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="56dae-128">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56dae-129">示例</span><span class="sxs-lookup"><span data-stu-id="56dae-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56dae-130">请求</span><span class="sxs-lookup"><span data-stu-id="56dae-130">Request</span></span>
<span data-ttu-id="56dae-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56dae-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="56dae-132">响应</span><span class="sxs-lookup"><span data-stu-id="56dae-132">Response</span></span>
<span data-ttu-id="56dae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56dae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-list-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
