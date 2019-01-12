---
title: 列出组设置
description: 检索组设置对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8cb245c786ef1fbede3e305fd73df74eb574393c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932362"
---
# <a name="list-group-settings"></a><span data-ttu-id="7469b-103">列出组设置</span><span class="sxs-lookup"><span data-stu-id="7469b-103">List group settings</span></span>

<span data-ttu-id="7469b-104">检索组设置对象列表。</span><span class="sxs-lookup"><span data-stu-id="7469b-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7469b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7469b-105">Permissions</span></span>

<span data-ttu-id="7469b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7469b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7469b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7469b-108">Permission type</span></span>      | <span data-ttu-id="7469b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7469b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7469b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7469b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7469b-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7469b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7469b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7469b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7469b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7469b-113">Not supported.</span></span>    |
|<span data-ttu-id="7469b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7469b-114">Application</span></span> | <span data-ttu-id="7469b-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7469b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7469b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7469b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7469b-117">列出租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="7469b-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7469b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7469b-118">Optional query parameters</span></span>
<span data-ttu-id="7469b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7469b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="7469b-120">注意：不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="7469b-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7469b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7469b-121">Request headers</span></span>
| <span data-ttu-id="7469b-122">名称</span><span class="sxs-lookup"><span data-stu-id="7469b-122">Name</span></span> | <span data-ttu-id="7469b-123">说明</span><span class="sxs-lookup"><span data-stu-id="7469b-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7469b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7469b-124">Authorization</span></span>  | <span data-ttu-id="7469b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7469b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7469b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7469b-127">Request body</span></span>
<span data-ttu-id="7469b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7469b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7469b-129">响应</span><span class="sxs-lookup"><span data-stu-id="7469b-129">Response</span></span>

<span data-ttu-id="7469b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7469b-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7469b-131">示例</span><span class="sxs-lookup"><span data-stu-id="7469b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7469b-132">请求</span><span class="sxs-lookup"><span data-stu-id="7469b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="7469b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7469b-133">Response</span></span>

<span data-ttu-id="7469b-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7469b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
