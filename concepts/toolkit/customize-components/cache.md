---
title: Microsoft Graph Toolkit缓存
description: 解释缓存的工作原理以及如何配置提供给开发人员的选项
localization_priority: Normal
author: adchau
ms.openlocfilehash: f51b4f188fe8ec70f75a50e1d9de049459c97e14
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658704"
---
# <a name="microsoft-graph-toolkit-caching"></a><span data-ttu-id="d97b5-103">Microsoft Graph Toolkit缓存</span><span class="sxs-lookup"><span data-stu-id="d97b5-103">Microsoft Graph Toolkit caching</span></span>

<span data-ttu-id="d97b5-104">Microsoft Graph Toolkit支持缓存选择 Microsoft Graph API 调用。</span><span class="sxs-lookup"><span data-stu-id="d97b5-104">The Microsoft Graph Toolkit supports caching of select Microsoft Graph API calls.</span></span> <span data-ttu-id="d97b5-105">目前，对用户、人员、联系人和照片终结点的调用默认缓存在三个 IndexedDB 存储中。</span><span class="sxs-lookup"><span data-stu-id="d97b5-105">Currently, calls to the users, person, contact, and photo endpoints are cached by default in three IndexedDB stores.</span></span>

<span data-ttu-id="d97b5-106">您可以在开发人员面板上查看缓存。</span><span class="sxs-lookup"><span data-stu-id="d97b5-106">You can view the cache on the developer panel.</span></span> <span data-ttu-id="d97b5-107">在 **"应用程序"\*\*\*\*选项卡上的"** 存储"窗格中，转到 **"IndexedDB"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="d97b5-107">On the **Application** tab, in the **Storage** pane, go to the **IndexedDB** tab.</span></span>

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a><span data-ttu-id="d97b5-109">缓存配置</span><span class="sxs-lookup"><span data-stu-id="d97b5-109">Cache configuration</span></span>

<span data-ttu-id="d97b5-110">可以通过静态类对象读取和写入缓存 `CacheService.config` 选项。</span><span class="sxs-lookup"><span data-stu-id="d97b5-110">You can read and write the cache options through the static class `CacheService.config` object.</span></span> <span data-ttu-id="d97b5-111">它的格式如下所示。</span><span class="sxs-lookup"><span data-stu-id="d97b5-111">It is formatted as shown.</span></span>

```TypeScript
let config = {
  defaultInvalidationPeriod: number,
  isEnabled: boolean,
  people: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  photos: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  users: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  presence: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  groups: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
};
```

<span data-ttu-id="d97b5-112">在 config 对象中，单个缓存无效时段默认为 `null` `defaultInvalidationPeriod` 3，600，000 毫秒，默认值为 60 (60 分钟) 。</span><span class="sxs-lookup"><span data-stu-id="d97b5-112">Individual cache invalidation periods are defaulted to `null` in the config object, and default to the general `defaultInvalidationPeriod` value of 3,600,000 ms (60 minutes).</span></span> <span data-ttu-id="d97b5-113">传入的任何值 `config.x.invalidationPeriod` 都将替代 `defaultInvalidationPeriod` 。</span><span class="sxs-lookup"><span data-stu-id="d97b5-113">Any value passed into `config.x.invalidationPeriod` will override `defaultInvalidationPeriod`.</span></span>

<span data-ttu-id="d97b5-114">状态存储是唯一的例外，其默认值为 300000 毫秒（即 5 分钟）。</span><span class="sxs-lookup"><span data-stu-id="d97b5-114">The presence store is the only exception, and has a default value of 300000 ms, or 5 minutes.</span></span>

### <a name="examples"></a><span data-ttu-id="d97b5-115">示例</span><span class="sxs-lookup"><span data-stu-id="d97b5-115">Examples</span></span>

<span data-ttu-id="d97b5-116">若要单独禁用存储，只需将存储中的配置属性的值设置为 `isEnabled` false：</span><span class="sxs-lookup"><span data-stu-id="d97b5-116">To individual disable a store simply set the value of `isEnabled` in that store's config properties to false:</span></span>
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
<span data-ttu-id="d97b5-117">禁用缓存不会 **清除** 缓存。</span><span class="sxs-lookup"><span data-stu-id="d97b5-117">Disabling the cache does **not** clear the cache.</span></span>

<span data-ttu-id="d97b5-118">更改验证期类似：</span><span class="sxs-lookup"><span data-stu-id="d97b5-118">Changing the invalditation period is similar:</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a><span data-ttu-id="d97b5-119">清除缓存</span><span class="sxs-lookup"><span data-stu-id="d97b5-119">Clearing the cache</span></span>

<span data-ttu-id="d97b5-120">当用户退出时，将自动清除缓存。也可以手动清除它。</span><span class="sxs-lookup"><span data-stu-id="d97b5-120">The cache is automatically cleared when the user signs out. It can also be cleared manually.</span></span>

<span data-ttu-id="d97b5-121">清除缓存中所有存储时，类的方法将清除 CacheService 维护的所有 `clearCaches()` `CacheService` 存储。</span><span class="sxs-lookup"><span data-stu-id="d97b5-121">The clear all the stores in the cache, the `clearCaches()` method of the `CacheService` class will clear every store maintained by the CacheService.</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a><span data-ttu-id="d97b5-122">创建自己的缓存存储</span><span class="sxs-lookup"><span data-stu-id="d97b5-122">Creating your own cache stores</span></span>

<span data-ttu-id="d97b5-123">如果要为自定义组件创建和填充自己的缓存存储，可以使用 `CacheService` 静态类。</span><span class="sxs-lookup"><span data-stu-id="d97b5-123">If you want to create and populate your own cache stores for your custom components, you can use the `CacheService` static class.</span></span>

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> <span data-ttu-id="d97b5-124">**注意：** 调用 `storeName` 中引用的项 `getCache()` 必须与对象中列出的存储之一 `CacheSchema` 匹配。</span><span class="sxs-lookup"><span data-stu-id="d97b5-124">**Note:** The `storeName` you reference in the call to `getCache()` must match one of the stores listed in your `CacheSchema` object.</span></span>

<span data-ttu-id="d97b5-125">该对象 `CacheSchema` 是键/值对的字典。</span><span class="sxs-lookup"><span data-stu-id="d97b5-125">The `CacheSchema` object is a dictionary with the key/value pairs.</span></span>

```TypeScript
import { CacheSchema } from '@microsoft/mgt';
const cacheSchema: CacheSchema = {
  name: string,
  stores: {
    store1: {},
    store2: {},
    ...
  },
  version: number
};
```

<span data-ttu-id="d97b5-126">以下示例演示缓存实现。</span><span class="sxs-lookup"><span data-stu-id="d97b5-126">The following example shows the cache implementation.</span></span>

```TypeScript
import { CacheItem, CacheSchema, CacheService, CacheStore } from '@microsoft/mgt';

const cacheSchema: CacheSchema = {
  name: 'users',
  stores: {
    users: {},
    usersQuery: {}
  },
  version: 1
};

interface CacheUser extends CacheItem {
  user?: string;
}

// retrieves invalidation time from cache config
const getUserInvalidationTime = (): number =>
  CacheService.config.users.invalidationPeriod || CacheService.config.defaultInvalidationPeriod;

// checks for if cache is enabled
const usersCacheEnabled = (): boolean => CacheService.config.users.isEnabled && CacheService.config.isEnabled;

// declare the desired cache store
let cache: CacheStore<CacheUser>

// check if the cache is enabled
if (usersCacheEnabled()) {
  cache = CacheService.getCache<CacheUser>(cacheSchema, 'users');
  const user = await cache.getValue(query);

  // check if an item is retrieved, and if it's not expired
  if (user && getUserInvalidationTime() > Date.now() - user.timeCached) {
    return JSON.parse(user.user);
  }
}

// graph call
const graphRes = graph
  .api('me')
  .middlewareOptions(prepScopes('user.read'))
  .get();

// store graph result into the cache if cache is enabled
if (usersCacheEnabled()) {
  cache.putValue(userId, { user: JSON.stringify(graphRes) });
}
```
