---
title: 创建 registeredUser
description: 添加设备的已注册用户。
author: tfitzmac
ms.openlocfilehash: 83b03c8119c4d47b0ab47a4eefb3762f3f0a4ada
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336314"
---
# <a name="create-registereduser"></a><span data-ttu-id="80a99-103">创建 registeredUser</span><span class="sxs-lookup"><span data-stu-id="80a99-103">Create registeredUser</span></span>

> <span data-ttu-id="80a99-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80a99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80a99-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80a99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80a99-106">添加设备的已注册用户。</span><span class="sxs-lookup"><span data-stu-id="80a99-106">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="80a99-107">权限</span><span class="sxs-lookup"><span data-stu-id="80a99-107">Permissions</span></span>
<span data-ttu-id="80a99-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80a99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="80a99-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80a99-110">Permission type</span></span>      | <span data-ttu-id="80a99-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80a99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80a99-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80a99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80a99-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80a99-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80a99-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80a99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80a99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80a99-115">Not supported.</span></span>    |
|<span data-ttu-id="80a99-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80a99-116">Application</span></span> | <span data-ttu-id="80a99-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a99-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80a99-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80a99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="80a99-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="80a99-119">Request headers</span></span>
| <span data-ttu-id="80a99-120">Name</span><span class="sxs-lookup"><span data-stu-id="80a99-120">Name</span></span>       | <span data-ttu-id="80a99-121">类型</span><span class="sxs-lookup"><span data-stu-id="80a99-121">Type</span></span> | <span data-ttu-id="80a99-122">说明</span><span class="sxs-lookup"><span data-stu-id="80a99-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80a99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80a99-123">Authorization</span></span>  | <span data-ttu-id="80a99-124">string</span><span class="sxs-lookup"><span data-stu-id="80a99-124">string</span></span>  | <span data-ttu-id="80a99-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80a99-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80a99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80a99-127">Request body</span></span>
<span data-ttu-id="80a99-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a99-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="80a99-129">响应</span><span class="sxs-lookup"><span data-stu-id="80a99-129">Response</span></span>

<span data-ttu-id="80a99-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80a99-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a99-131">示例</span><span class="sxs-lookup"><span data-stu-id="80a99-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80a99-132">请求</span><span class="sxs-lookup"><span data-stu-id="80a99-132">Request</span></span>
<span data-ttu-id="80a99-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80a99-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="80a99-134">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a99-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="80a99-135">响应</span><span class="sxs-lookup"><span data-stu-id="80a99-135">Response</span></span>
<span data-ttu-id="80a99-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80a99-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->