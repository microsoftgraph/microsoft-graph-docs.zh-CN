---
title: 获取组设置
description: 检索特定组设置对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d47441a66ab0b2ed3602a69f4a92a06050708f67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577831"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="487f1-103">获取组设置</span><span class="sxs-lookup"><span data-stu-id="487f1-103">Get a group setting</span></span>

<span data-ttu-id="487f1-104">检索特定组设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="487f1-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="487f1-105">权限</span><span class="sxs-lookup"><span data-stu-id="487f1-105">Permissions</span></span>

<span data-ttu-id="487f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="487f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="487f1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="487f1-108">Permission type</span></span>      | <span data-ttu-id="487f1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="487f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="487f1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="487f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="487f1-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="487f1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="487f1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="487f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="487f1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="487f1-113">Not supported.</span></span>    |
|<span data-ttu-id="487f1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="487f1-114">Application</span></span> | <span data-ttu-id="487f1-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="487f1-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="487f1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="487f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="487f1-117">获取特定的租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="487f1-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="487f1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="487f1-118">Optional query parameters</span></span>
<span data-ttu-id="487f1-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="487f1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="487f1-120">注意：不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="487f1-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="487f1-121">请求头</span><span class="sxs-lookup"><span data-stu-id="487f1-121">Request headers</span></span>
| <span data-ttu-id="487f1-122">名称</span><span class="sxs-lookup"><span data-stu-id="487f1-122">Name</span></span> | <span data-ttu-id="487f1-123">说明</span><span class="sxs-lookup"><span data-stu-id="487f1-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="487f1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="487f1-124">Authorization</span></span> | <span data-ttu-id="487f1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="487f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="487f1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="487f1-127">Request body</span></span>

<span data-ttu-id="487f1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="487f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="487f1-129">响应</span><span class="sxs-lookup"><span data-stu-id="487f1-129">Response</span></span>

<span data-ttu-id="487f1-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[groupSetting](../resources/groupsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="487f1-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="487f1-131">示例</span><span class="sxs-lookup"><span data-stu-id="487f1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="487f1-132">请求</span><span class="sxs-lookup"><span data-stu-id="487f1-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="487f1-133">响应</span><span class="sxs-lookup"><span data-stu-id="487f1-133">Response</span></span>

<span data-ttu-id="487f1-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="487f1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
