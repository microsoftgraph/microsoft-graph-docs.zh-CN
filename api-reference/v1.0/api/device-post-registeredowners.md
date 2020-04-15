---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 085e2ccf71f26b3a34a0eb2daceed1bcbb60ac22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466702"
---
# <a name="create-registeredowner"></a><span data-ttu-id="9f0db-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="9f0db-103">Create registeredOwner</span></span>

<span data-ttu-id="9f0db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f0db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f0db-105">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="9f0db-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f0db-106">权限</span><span class="sxs-lookup"><span data-stu-id="9f0db-106">Permissions</span></span>
<span data-ttu-id="9f0db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f0db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9f0db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f0db-109">Permission type</span></span>      | <span data-ttu-id="9f0db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f0db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f0db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f0db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f0db-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f0db-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f0db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f0db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f0db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f0db-114">Not supported.</span></span>    |
|<span data-ttu-id="9f0db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f0db-115">Application</span></span> | <span data-ttu-id="9f0db-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f0db-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f0db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f0db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9f0db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f0db-118">Request headers</span></span>
| <span data-ttu-id="9f0db-119">名称</span><span class="sxs-lookup"><span data-stu-id="9f0db-119">Name</span></span>       | <span data-ttu-id="9f0db-120">类型</span><span class="sxs-lookup"><span data-stu-id="9f0db-120">Type</span></span> | <span data-ttu-id="9f0db-121">说明</span><span class="sxs-lookup"><span data-stu-id="9f0db-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f0db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f0db-122">Authorization</span></span>  | <span data-ttu-id="9f0db-123">string</span><span class="sxs-lookup"><span data-stu-id="9f0db-123">string</span></span>  | <span data-ttu-id="9f0db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f0db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f0db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f0db-126">Request body</span></span>
<span data-ttu-id="9f0db-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f0db-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f0db-128">响应</span><span class="sxs-lookup"><span data-stu-id="9f0db-128">Response</span></span>

<span data-ttu-id="9f0db-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f0db-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f0db-130">示例</span><span class="sxs-lookup"><span data-stu-id="9f0db-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f0db-131">请求</span><span class="sxs-lookup"><span data-stu-id="9f0db-131">Request</span></span>
<span data-ttu-id="9f0db-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f0db-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f0db-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f0db-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="9f0db-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f0db-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9f0db-135">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f0db-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f0db-136">响应</span><span class="sxs-lookup"><span data-stu-id="9f0db-136">Response</span></span>
<span data-ttu-id="9f0db-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f0db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
