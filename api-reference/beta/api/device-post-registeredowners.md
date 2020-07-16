---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 423fd07e20b71a221d593f0cbe142d2f399bf30f
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146692"
---
# <a name="create-registeredowner"></a><span data-ttu-id="c45bf-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="c45bf-103">Create registeredOwner</span></span>

<span data-ttu-id="c45bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c45bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c45bf-105">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="c45bf-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="c45bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="c45bf-106">Permissions</span></span>
<span data-ttu-id="c45bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c45bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c45bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c45bf-109">Permission type</span></span>      | <span data-ttu-id="c45bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c45bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c45bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c45bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c45bf-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c45bf-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c45bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c45bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c45bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c45bf-114">Not supported.</span></span>    |
|<span data-ttu-id="c45bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c45bf-115">Application</span></span> | <span data-ttu-id="c45bf-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45bf-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c45bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c45bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c45bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c45bf-118">Request headers</span></span>
| <span data-ttu-id="c45bf-119">名称</span><span class="sxs-lookup"><span data-stu-id="c45bf-119">Name</span></span>       | <span data-ttu-id="c45bf-120">类型</span><span class="sxs-lookup"><span data-stu-id="c45bf-120">Type</span></span> | <span data-ttu-id="c45bf-121">说明</span><span class="sxs-lookup"><span data-stu-id="c45bf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c45bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c45bf-122">Authorization</span></span>  | <span data-ttu-id="c45bf-123">string</span><span class="sxs-lookup"><span data-stu-id="c45bf-123">string</span></span>  | <span data-ttu-id="c45bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c45bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c45bf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c45bf-126">Request body</span></span>
<span data-ttu-id="c45bf-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c45bf-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c45bf-128">响应</span><span class="sxs-lookup"><span data-stu-id="c45bf-128">Response</span></span>

<span data-ttu-id="c45bf-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c45bf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c45bf-130">示例</span><span class="sxs-lookup"><span data-stu-id="c45bf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c45bf-131">请求</span><span class="sxs-lookup"><span data-stu-id="c45bf-131">Request</span></span>
<span data-ttu-id="c45bf-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c45bf-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c45bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c45bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c45bf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c45bf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c45bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="c45bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c45bf-136">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c45bf-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c45bf-137">响应</span><span class="sxs-lookup"><span data-stu-id="c45bf-137">Response</span></span>
<span data-ttu-id="c45bf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c45bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
