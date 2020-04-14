---
title: 创建 registeredUser
description: 添加设备的已注册用户。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ab9c4a526faa5aa7d5f899bcc3655dae74033c8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381741"
---
# <a name="create-registereduser"></a><span data-ttu-id="131d7-103">创建 registeredUser</span><span class="sxs-lookup"><span data-stu-id="131d7-103">Create registeredUser</span></span>

<span data-ttu-id="131d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="131d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131d7-105">添加设备的已注册用户。</span><span class="sxs-lookup"><span data-stu-id="131d7-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="131d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="131d7-106">Permissions</span></span>
<span data-ttu-id="131d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="131d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="131d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="131d7-109">Permission type</span></span>      | <span data-ttu-id="131d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="131d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="131d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="131d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="131d7-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="131d7-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="131d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="131d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="131d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="131d7-114">Not supported.</span></span>    |
|<span data-ttu-id="131d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="131d7-115">Application</span></span> | <span data-ttu-id="131d7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="131d7-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="131d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="131d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="131d7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="131d7-118">Request headers</span></span>
| <span data-ttu-id="131d7-119">名称</span><span class="sxs-lookup"><span data-stu-id="131d7-119">Name</span></span>       | <span data-ttu-id="131d7-120">类型</span><span class="sxs-lookup"><span data-stu-id="131d7-120">Type</span></span> | <span data-ttu-id="131d7-121">说明</span><span class="sxs-lookup"><span data-stu-id="131d7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="131d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="131d7-122">Authorization</span></span>  | <span data-ttu-id="131d7-123">string</span><span class="sxs-lookup"><span data-stu-id="131d7-123">string</span></span>  | <span data-ttu-id="131d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="131d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="131d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="131d7-126">Request body</span></span>
<span data-ttu-id="131d7-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="131d7-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="131d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="131d7-128">Response</span></span>

<span data-ttu-id="131d7-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="131d7-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="131d7-130">示例</span><span class="sxs-lookup"><span data-stu-id="131d7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="131d7-131">请求</span><span class="sxs-lookup"><span data-stu-id="131d7-131">Request</span></span>
<span data-ttu-id="131d7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="131d7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="131d7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="131d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="131d7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="131d7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="131d7-135">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="131d7-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="131d7-136">响应</span><span class="sxs-lookup"><span data-stu-id="131d7-136">Response</span></span>
<span data-ttu-id="131d7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="131d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
