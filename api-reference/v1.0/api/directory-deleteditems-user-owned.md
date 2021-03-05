---
title: 列出用户拥有的已删除项目
description: '检索指定用户拥有的最近删除的项目的列表。  '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7c947d6ebb8a1f268728c07be64451e230497fb6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434473"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="70b0a-103">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="70b0a-103">List deleted items owned by a user</span></span>

<span data-ttu-id="70b0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70b0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70b0a-105">检索指定用户拥有的最近删除的项目的列表。</span><span class="sxs-lookup"><span data-stu-id="70b0a-105">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="70b0a-106">目前，仅用户拥有的应用程序和组资源支持列表已删除[](../resources/application.md)的项目功能[](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="70b0a-106">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="70b0a-107">这是一项服务操作，这意味着它不支持分页。</span><span class="sxs-lookup"><span data-stu-id="70b0a-107">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="70b0a-108">API 最多返回 1，000 个已删除对象，这些对象由用户拥有，按 ID 排序。</span><span class="sxs-lookup"><span data-stu-id="70b0a-108">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="70b0a-109">权限</span><span class="sxs-lookup"><span data-stu-id="70b0a-109">Permissions</span></span>

<span data-ttu-id="70b0a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70b0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70b0a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="70b0a-112">Permission type</span></span> | <span data-ttu-id="70b0a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70b0a-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="70b0a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70b0a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="70b0a-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b0a-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="70b0a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70b0a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="70b0a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="70b0a-117">Not supported.</span></span> |
| <span data-ttu-id="70b0a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="70b0a-118">Application</span></span> | <span data-ttu-id="70b0a-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b0a-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="70b0a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70b0a-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="70b0a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="70b0a-121">Request headers</span></span>

| <span data-ttu-id="70b0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="70b0a-122">Name</span></span>          | <span data-ttu-id="70b0a-123">说明</span><span class="sxs-lookup"><span data-stu-id="70b0a-123">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="70b0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="70b0a-124">Authorization</span></span> | <span data-ttu-id="70b0a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70b0a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70b0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70b0a-127">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="70b0a-128">请求正文需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="70b0a-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="70b0a-129">参数</span><span class="sxs-lookup"><span data-stu-id="70b0a-129">Parameter</span></span>    | <span data-ttu-id="70b0a-130">类型</span><span class="sxs-lookup"><span data-stu-id="70b0a-130">Type</span></span> |<span data-ttu-id="70b0a-131">描述</span><span class="sxs-lookup"><span data-stu-id="70b0a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70b0a-132">userId</span><span class="sxs-lookup"><span data-stu-id="70b0a-132">userId</span></span>|<span data-ttu-id="70b0a-133">String</span><span class="sxs-lookup"><span data-stu-id="70b0a-133">String</span></span>|<span data-ttu-id="70b0a-134">所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="70b0a-134">ID of the owner.</span></span>|
|<span data-ttu-id="70b0a-135">type</span><span class="sxs-lookup"><span data-stu-id="70b0a-135">type</span></span>|<span data-ttu-id="70b0a-136">String</span><span class="sxs-lookup"><span data-stu-id="70b0a-136">String</span></span>|<span data-ttu-id="70b0a-137">要返回的拥有对象的类型; `Group` 当前是唯一受支持的值。</span><span class="sxs-lookup"><span data-stu-id="70b0a-137">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="70b0a-138">响应</span><span class="sxs-lookup"><span data-stu-id="70b0a-138">Response</span></span>

<span data-ttu-id="70b0a-139">成功的请求返回 `200 OK` 响应代码;响应对象包括 ([已删除) ](../resources/directory.md) 目录。</span><span class="sxs-lookup"><span data-stu-id="70b0a-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="70b0a-140">示例</span><span class="sxs-lookup"><span data-stu-id="70b0a-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70b0a-141">请求</span><span class="sxs-lookup"><span data-stu-id="70b0a-141">Request</span></span>

<span data-ttu-id="70b0a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70b0a-142">Here is an example of the request.</span></span>

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

###### <a name="response"></a><span data-ttu-id="70b0a-143">响应</span><span class="sxs-lookup"><span data-stu-id="70b0a-143">Response</span></span>

<span data-ttu-id="70b0a-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70b0a-144">Here is an example of the response.</span></span> <span data-ttu-id="70b0a-145">注意：为了简洁起见，可能会截断此响应对象。</span><span class="sxs-lookup"><span data-stu-id="70b0a-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="70b0a-146">所有支持的属性都从实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="70b0a-146">All supported properties are returned from actual calls.</span></span>

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
