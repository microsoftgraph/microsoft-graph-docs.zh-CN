---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a392d1d9c998bad74d29ad4f8c74a3bec1c61ff4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437192"
---
# <a name="create-registeredowner"></a><span data-ttu-id="5a313-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="5a313-103">Create registeredOwner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a313-104">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="5a313-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a313-105">权限</span><span class="sxs-lookup"><span data-stu-id="5a313-105">Permissions</span></span>
<span data-ttu-id="5a313-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a313-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a313-108">Permission type</span></span>      | <span data-ttu-id="5a313-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a313-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a313-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a313-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a313-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a313-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a313-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a313-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a313-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a313-113">Not supported.</span></span>    |
|<span data-ttu-id="5a313-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a313-114">Application</span></span> | <span data-ttu-id="5a313-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a313-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a313-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a313-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="5a313-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a313-117">Request headers</span></span>
| <span data-ttu-id="5a313-118">名称</span><span class="sxs-lookup"><span data-stu-id="5a313-118">Name</span></span>       | <span data-ttu-id="5a313-119">类型</span><span class="sxs-lookup"><span data-stu-id="5a313-119">Type</span></span> | <span data-ttu-id="5a313-120">说明</span><span class="sxs-lookup"><span data-stu-id="5a313-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a313-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a313-121">Authorization</span></span>  | <span data-ttu-id="5a313-122">string</span><span class="sxs-lookup"><span data-stu-id="5a313-122">string</span></span>  | <span data-ttu-id="5a313-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a313-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a313-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a313-125">Request body</span></span>
<span data-ttu-id="5a313-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a313-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5a313-127">响应</span><span class="sxs-lookup"><span data-stu-id="5a313-127">Response</span></span>

<span data-ttu-id="5a313-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a313-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a313-129">示例</span><span class="sxs-lookup"><span data-stu-id="5a313-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a313-130">请求</span><span class="sxs-lookup"><span data-stu-id="5a313-130">Request</span></span>
<span data-ttu-id="5a313-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a313-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5a313-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5a313-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a313-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a313-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5a313-134">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a313-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5a313-135">响应</span><span class="sxs-lookup"><span data-stu-id="5a313-135">Response</span></span>
<span data-ttu-id="5a313-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a313-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
