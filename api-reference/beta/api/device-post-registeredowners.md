---
title: 创建 registeredOwner
description: 将用户添加为设备的已注册所有者。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e1c8151f43ea7c4eb8e1235727a6b9f40f193853
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824260"
---
# <a name="create-registeredowner"></a><span data-ttu-id="57b1f-103">创建 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="57b1f-103">Create registeredOwner</span></span>

> <span data-ttu-id="57b1f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="57b1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57b1f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57b1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57b1f-106">将用户添加为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="57b1f-106">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="57b1f-107">权限</span><span class="sxs-lookup"><span data-stu-id="57b1f-107">Permissions</span></span>
<span data-ttu-id="57b1f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57b1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57b1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57b1f-110">Permission type</span></span>      | <span data-ttu-id="57b1f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57b1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57b1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57b1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57b1f-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57b1f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57b1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57b1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57b1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57b1f-115">Not supported.</span></span>    |
|<span data-ttu-id="57b1f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57b1f-116">Application</span></span> | <span data-ttu-id="57b1f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b1f-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57b1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57b1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="57b1f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57b1f-119">Request headers</span></span>
| <span data-ttu-id="57b1f-120">名称</span><span class="sxs-lookup"><span data-stu-id="57b1f-120">Name</span></span>       | <span data-ttu-id="57b1f-121">类型</span><span class="sxs-lookup"><span data-stu-id="57b1f-121">Type</span></span> | <span data-ttu-id="57b1f-122">说明</span><span class="sxs-lookup"><span data-stu-id="57b1f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57b1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57b1f-123">Authorization</span></span>  | <span data-ttu-id="57b1f-124">string</span><span class="sxs-lookup"><span data-stu-id="57b1f-124">string</span></span>  | <span data-ttu-id="57b1f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57b1f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57b1f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="57b1f-127">Request body</span></span>
<span data-ttu-id="57b1f-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57b1f-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57b1f-129">响应</span><span class="sxs-lookup"><span data-stu-id="57b1f-129">Response</span></span>

<span data-ttu-id="57b1f-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57b1f-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57b1f-131">示例</span><span class="sxs-lookup"><span data-stu-id="57b1f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57b1f-132">请求</span><span class="sxs-lookup"><span data-stu-id="57b1f-132">Request</span></span>
<span data-ttu-id="57b1f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57b1f-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="57b1f-134">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57b1f-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="57b1f-135">响应</span><span class="sxs-lookup"><span data-stu-id="57b1f-135">Response</span></span>
<span data-ttu-id="57b1f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57b1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
