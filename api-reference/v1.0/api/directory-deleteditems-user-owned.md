---
title: 列出用户拥有的已删除项目
description: '检索指定用户拥有的最近删除的项目的列表。  '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 168667566f880ecc2b2aafea63d95179e8c5c6a4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869947"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="9ec11-103">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="9ec11-103">List deleted items owned by a user</span></span>

<span data-ttu-id="9ec11-104">检索指定用户拥有的最近删除的项目的列表。</span><span class="sxs-lookup"><span data-stu-id="9ec11-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="9ec11-105">目前，列出已删除项目仅支持用户拥有的[应用程序](../resources/application.md)和[组](../resources/group.md)资源的功能。</span><span class="sxs-lookup"><span data-stu-id="9ec11-105">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="9ec11-106">这是一个服务操作，这意味着它不支持分页。</span><span class="sxs-lookup"><span data-stu-id="9ec11-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="9ec11-107">API 返回最大为1000个已删除的对象，这些对象归用户所有，按 ID 排序。</span><span class="sxs-lookup"><span data-stu-id="9ec11-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec11-108">权限</span><span class="sxs-lookup"><span data-stu-id="9ec11-108">Permissions</span></span>

<span data-ttu-id="9ec11-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="9ec11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="9ec11-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ec11-111">Permission type</span></span> | <span data-ttu-id="9ec11-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ec11-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="9ec11-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec11-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9ec11-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec11-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9ec11-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec11-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ec11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ec11-116">Not supported.</span></span> |
| <span data-ttu-id="9ec11-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ec11-117">Application</span></span> | <span data-ttu-id="9ec11-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec11-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9ec11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ec11-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="9ec11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ec11-120">Request headers</span></span>

| <span data-ttu-id="9ec11-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ec11-121">Name</span></span>          | <span data-ttu-id="9ec11-122">说明</span><span class="sxs-lookup"><span data-stu-id="9ec11-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="9ec11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec11-123">Authorization</span></span> | <span data-ttu-id="9ec11-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ec11-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ec11-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ec11-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="9ec11-127">请求正文需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="9ec11-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="9ec11-128">参数</span><span class="sxs-lookup"><span data-stu-id="9ec11-128">Parameter</span></span>    | <span data-ttu-id="9ec11-129">类型</span><span class="sxs-lookup"><span data-stu-id="9ec11-129">Type</span></span> |<span data-ttu-id="9ec11-130">说明</span><span class="sxs-lookup"><span data-stu-id="9ec11-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ec11-131">userId</span><span class="sxs-lookup"><span data-stu-id="9ec11-131">userId</span></span>|<span data-ttu-id="9ec11-132">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-132">String</span></span>|<span data-ttu-id="9ec11-133">所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="9ec11-133">ID of the owner.</span></span>|
|<span data-ttu-id="9ec11-134">type</span><span class="sxs-lookup"><span data-stu-id="9ec11-134">type</span></span>|<span data-ttu-id="9ec11-135">字符串</span><span class="sxs-lookup"><span data-stu-id="9ec11-135">String</span></span>|<span data-ttu-id="9ec11-136">要返回的所拥有的对象的类型;`Group`目前是唯一受支持的值。</span><span class="sxs-lookup"><span data-stu-id="9ec11-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="9ec11-137">响应</span><span class="sxs-lookup"><span data-stu-id="9ec11-137">Response</span></span>

<span data-ttu-id="9ec11-138">成功的请求`200 OK`返回响应代码;response 对象包括[目录（已删除项目）](../resources/directory.md)属性。</span><span class="sxs-lookup"><span data-stu-id="9ec11-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="9ec11-139">示例</span><span class="sxs-lookup"><span data-stu-id="9ec11-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9ec11-140">请求</span><span class="sxs-lookup"><span data-stu-id="9ec11-140">Request</span></span>

<span data-ttu-id="9ec11-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ec11-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="9ec11-142">响应</span><span class="sxs-lookup"><span data-stu-id="9ec11-142">Response</span></span>

<span data-ttu-id="9ec11-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9ec11-143">Here is an example of the response.</span></span> <span data-ttu-id="9ec11-144">注意：为简洁起见，可能会截断此响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ec11-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="9ec11-145">所有受支持的属性都从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ec11-145">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


