---
title: 权限
description: '检索列表的、 由指定用户拥有的最近已删除项目。  '
author: lleonard-msft
ms.openlocfilehash: 9ce487d957f4bdaa2684d00865aeac7ea293ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351168"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="e346f-103">**由用户拥有的删除列表项**</span><span class="sxs-lookup"><span data-stu-id="e346f-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="e346f-104">检索列表的、 由指定用户拥有的最近已删除项目。</span><span class="sxs-lookup"><span data-stu-id="e346f-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="e346f-105">目前，删除列表项功能的用户所拥有的[group](../resources/group.md)资源仅支持。</span><span class="sxs-lookup"><span data-stu-id="e346f-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="e346f-106">这是服务操作，这意味着它不支持分页。</span><span class="sxs-lookup"><span data-stu-id="e346f-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="e346f-107">API 返回多达 1,000 个用户，按 ID 排序所拥有的已删除的对象</span><span class="sxs-lookup"><span data-stu-id="e346f-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e346f-108">权限</span><span class="sxs-lookup"><span data-stu-id="e346f-108">Permissions</span></span>

<span data-ttu-id="e346f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="e346f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="e346f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e346f-111">Permission type</span></span> | <span data-ttu-id="e346f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e346f-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="e346f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e346f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e346f-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e346f-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e346f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e346f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e346f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e346f-116">Not supported.</span></span> |
| <span data-ttu-id="e346f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e346f-117">Application</span></span> | <span data-ttu-id="e346f-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e346f-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e346f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e346f-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="e346f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e346f-120">Request headers</span></span>

| <span data-ttu-id="e346f-121">Name</span><span class="sxs-lookup"><span data-stu-id="e346f-121">Name</span></span>          | <span data-ttu-id="e346f-122">说明</span><span class="sxs-lookup"><span data-stu-id="e346f-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="e346f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e346f-123">Authorization</span></span> | <span data-ttu-id="e346f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e346f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e346f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e346f-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="e346f-127">在请求正文需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="e346f-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="e346f-128">参数</span><span class="sxs-lookup"><span data-stu-id="e346f-128">Parameter</span></span>    | <span data-ttu-id="e346f-129">Type</span><span class="sxs-lookup"><span data-stu-id="e346f-129">Type</span></span> |<span data-ttu-id="e346f-130">说明</span><span class="sxs-lookup"><span data-stu-id="e346f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e346f-131">userId</span><span class="sxs-lookup"><span data-stu-id="e346f-131">userId</span></span>|<span data-ttu-id="e346f-132">String</span><span class="sxs-lookup"><span data-stu-id="e346f-132">String</span></span>|<span data-ttu-id="e346f-133">所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="e346f-133">ID of the owner.</span></span>|
|<span data-ttu-id="e346f-134">type</span><span class="sxs-lookup"><span data-stu-id="e346f-134">type</span></span>|<span data-ttu-id="e346f-135">字符串</span><span class="sxs-lookup"><span data-stu-id="e346f-135">String</span></span>|<span data-ttu-id="e346f-136">要返回; 的拥有对象的类型`Group`目前唯一受支持的值。</span><span class="sxs-lookup"><span data-stu-id="e346f-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="e346f-137">响应</span><span class="sxs-lookup"><span data-stu-id="e346f-137">Response</span></span>

<span data-ttu-id="e346f-138">成功的请求返回`200 OK`响应代码;响应对象包含[目录 （已删除项）](../resources/directory.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="e346f-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="e346f-139">示例</span><span class="sxs-lookup"><span data-stu-id="e346f-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e346f-140">请求</span><span class="sxs-lookup"><span data-stu-id="e346f-140">Request</span></span>

<span data-ttu-id="e346f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e346f-141">Here is an example of the request.</span></span>

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

###### <a name="response"></a><span data-ttu-id="e346f-142">响应</span><span class="sxs-lookup"><span data-stu-id="e346f-142">Response</span></span>

<span data-ttu-id="e346f-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e346f-143">Here is an example of the response.</span></span> <span data-ttu-id="e346f-144">注意： 为了简单起见，此响应对象可能被截断。</span><span class="sxs-lookup"><span data-stu-id="e346f-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="e346f-145">从实际的调用返回所有支持的属性。</span><span class="sxs-lookup"><span data-stu-id="e346f-145">All supported properties are returned from actual calls.</span></span>

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


