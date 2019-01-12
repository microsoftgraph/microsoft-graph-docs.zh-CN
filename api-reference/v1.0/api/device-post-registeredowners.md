---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 94d286b88b32d0e86e70581c4d4b91f7408bde51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927644"
---
# <a name="create-registeredowner"></a><span data-ttu-id="7e4bf-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="7e4bf-103">Create registeredOwner</span></span>

<span data-ttu-id="7e4bf-104">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e4bf-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e4bf-105">Permissions</span></span>
<span data-ttu-id="7e4bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e4bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e4bf-108">Permission type</span></span>      | <span data-ttu-id="7e4bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e4bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e4bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e4bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e4bf-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e4bf-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e4bf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e4bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e4bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-113">Not supported.</span></span>    |
|<span data-ttu-id="7e4bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e4bf-114">Application</span></span> | <span data-ttu-id="7e4bf-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e4bf-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e4bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e4bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7e4bf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e4bf-117">Request headers</span></span>
| <span data-ttu-id="7e4bf-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e4bf-118">Name</span></span>       | <span data-ttu-id="7e4bf-119">类型</span><span class="sxs-lookup"><span data-stu-id="7e4bf-119">Type</span></span> | <span data-ttu-id="7e4bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e4bf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e4bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e4bf-121">Authorization</span></span>  | <span data-ttu-id="7e4bf-122">string</span><span class="sxs-lookup"><span data-stu-id="7e4bf-122">string</span></span>  | <span data-ttu-id="7e4bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e4bf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e4bf-125">Request body</span></span>
<span data-ttu-id="7e4bf-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e4bf-127">响应</span><span class="sxs-lookup"><span data-stu-id="7e4bf-127">Response</span></span>

<span data-ttu-id="7e4bf-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e4bf-129">示例</span><span class="sxs-lookup"><span data-stu-id="7e4bf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e4bf-130">请求</span><span class="sxs-lookup"><span data-stu-id="7e4bf-130">Request</span></span>
<span data-ttu-id="7e4bf-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="7e4bf-132">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7e4bf-133">响应</span><span class="sxs-lookup"><span data-stu-id="7e4bf-133">Response</span></span>
<span data-ttu-id="7e4bf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e4bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
