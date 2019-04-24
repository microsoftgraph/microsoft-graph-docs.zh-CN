---
title: 获取 calendarGroup
description: 检索 calendargroup 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5444677ac2b2f4f8428203b7ef0cbc5027132751
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453288"
---
# <a name="get-calendargroup"></a><span data-ttu-id="e2974-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e2974-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2974-104">检索 calendargroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2974-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2974-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2974-105">Permissions</span></span>

<span data-ttu-id="e2974-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2974-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2974-108">Permission type</span></span>                        | <span data-ttu-id="e2974-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2974-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e2974-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2974-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2974-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2974-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="e2974-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2974-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2974-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2974-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="e2974-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2974-114">Application</span></span>                            | <span data-ttu-id="e2974-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2974-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="e2974-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2974-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e2974-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="e2974-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2974-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2974-118">Optional query parameters</span></span>

<span data-ttu-id="e2974-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2974-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2974-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2974-120">Request headers</span></span>

| <span data-ttu-id="e2974-121">名称</span><span class="sxs-lookup"><span data-stu-id="e2974-121">Name</span></span>          | <span data-ttu-id="e2974-122">类型</span><span class="sxs-lookup"><span data-stu-id="e2974-122">Type</span></span>   | <span data-ttu-id="e2974-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2974-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="e2974-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2974-124">Authorization</span></span> | <span data-ttu-id="e2974-125">string</span><span class="sxs-lookup"><span data-stu-id="e2974-125">string</span></span> | <span data-ttu-id="e2974-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2974-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2974-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2974-128">Request body</span></span>

<span data-ttu-id="e2974-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2974-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2974-130">响应</span><span class="sxs-lookup"><span data-stu-id="e2974-130">Response</span></span>

<span data-ttu-id="e2974-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2974-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2974-132">示例</span><span class="sxs-lookup"><span data-stu-id="e2974-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2974-133">请求</span><span class="sxs-lookup"><span data-stu-id="e2974-133">Request</span></span>

<span data-ttu-id="e2974-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2974-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="e2974-135">响应</span><span class="sxs-lookup"><span data-stu-id="e2974-135">Response</span></span>

<span data-ttu-id="e2974-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2974-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendargroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
