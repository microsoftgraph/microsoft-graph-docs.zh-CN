---
title: Permissions
description: '检索列表的、 由指定用户拥有的最近已删除项目。  '
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: da497fb3e919061db222c2247b59edadfca2d649
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829174"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="f7d59-103">**由用户拥有的删除列表项**</span><span class="sxs-lookup"><span data-stu-id="f7d59-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="f7d59-104">检索列表的、 由指定用户拥有的最近已删除项目。</span><span class="sxs-lookup"><span data-stu-id="f7d59-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="f7d59-105">目前，删除列表项功能的用户所拥有的[group](../resources/group.md)资源仅支持。</span><span class="sxs-lookup"><span data-stu-id="f7d59-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="f7d59-106">这是服务操作，这意味着它不支持分页。</span><span class="sxs-lookup"><span data-stu-id="f7d59-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="f7d59-107">API 返回多达 1,000 个用户，按 ID 排序所拥有的已删除的对象</span><span class="sxs-lookup"><span data-stu-id="f7d59-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>  <span data-ttu-id="f7d59-108">应用户拥有 1,000 个或多个删除对象，该 API 返回 nothing。</span><span class="sxs-lookup"><span data-stu-id="f7d59-108">Should the user own 1,000 or more deleted objects, the API returns nothing.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d59-109">权限</span><span class="sxs-lookup"><span data-stu-id="f7d59-109">Permissions</span></span>

<span data-ttu-id="f7d59-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="f7d59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="f7d59-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7d59-112">Permission type</span></span> | <span data-ttu-id="f7d59-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7d59-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="f7d59-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d59-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d59-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d59-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f7d59-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7d59-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7d59-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7d59-117">Not supported.</span></span> |
| <span data-ttu-id="f7d59-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7d59-118">Application</span></span> | <span data-ttu-id="f7d59-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d59-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f7d59-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7d59-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="f7d59-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7d59-121">Request headers</span></span>

| <span data-ttu-id="f7d59-122">**名称**</span><span class="sxs-lookup"><span data-stu-id="f7d59-122">**Name**</span></span>      | <span data-ttu-id="f7d59-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7d59-123">**Description**</span></span>           |
| ------------- | ------------------------- |
| <span data-ttu-id="f7d59-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7d59-124">Authorization</span></span> | <span data-ttu-id="f7d59-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7d59-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7d59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7d59-127">Request body</span></span>

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

<span data-ttu-id="f7d59-128">在请求正文需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="f7d59-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="f7d59-129">参数</span><span class="sxs-lookup"><span data-stu-id="f7d59-129">Parameter</span></span>    | <span data-ttu-id="f7d59-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7d59-130">Type</span></span> |<span data-ttu-id="f7d59-131">Description</span><span class="sxs-lookup"><span data-stu-id="f7d59-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d59-132">userId</span><span class="sxs-lookup"><span data-stu-id="f7d59-132">userId</span></span>|<span data-ttu-id="f7d59-133">String</span><span class="sxs-lookup"><span data-stu-id="f7d59-133">String</span></span>|<span data-ttu-id="f7d59-134">所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7d59-134">ID of the owner.</span></span>|
|<span data-ttu-id="f7d59-135">type</span><span class="sxs-lookup"><span data-stu-id="f7d59-135">type</span></span>|<span data-ttu-id="f7d59-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f7d59-136">String</span></span>|<span data-ttu-id="f7d59-137">要返回; 的拥有对象的类型`Group`目前唯一受支持的值。</span><span class="sxs-lookup"><span data-stu-id="f7d59-137">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|

## <a name="response"></a><span data-ttu-id="f7d59-138">响应</span><span class="sxs-lookup"><span data-stu-id="f7d59-138">Response</span></span>

<span data-ttu-id="f7d59-139">成功的请求返回`200 OK`响应代码;响应对象包含[目录 （已删除项）](../resources/directory.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="f7d59-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="f7d59-140">示例</span><span class="sxs-lookup"><span data-stu-id="f7d59-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7d59-141">请求</span><span class="sxs-lookup"><span data-stu-id="f7d59-141">Request</span></span>

<span data-ttu-id="f7d59-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7d59-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a><span data-ttu-id="f7d59-143">响应</span><span class="sxs-lookup"><span data-stu-id="f7d59-143">Response</span></span>

<span data-ttu-id="f7d59-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7d59-144">Here is an example of the response.</span></span> <span data-ttu-id="f7d59-145">注意： 为了简单起见，此响应对象可能被截断。</span><span class="sxs-lookup"><span data-stu-id="f7d59-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="f7d59-146">从实际的调用返回所有支持的属性。</span><span class="sxs-lookup"><span data-stu-id="f7d59-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
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


