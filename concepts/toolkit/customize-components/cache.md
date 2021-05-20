---
title: Microsoft Graph Toolkit缓存
description: 解释缓存的工作原理以及如何配置提供给开发人员的选项
localization_priority: Normal
author: adchau
ms.openlocfilehash: 7bb13e97cc6ef0fa77ba05afb27a065f934e1f42
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579933"
---
# <a name="microsoft-graph-toolkit-caching"></a><span data-ttu-id="4a2b3-103">Microsoft Graph Toolkit缓存</span><span class="sxs-lookup"><span data-stu-id="4a2b3-103">Microsoft Graph Toolkit caching</span></span>

<span data-ttu-id="4a2b3-104">Microsoft Graph Toolkit支持缓存选择 Microsoft Graph API 调用。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-104">The Microsoft Graph Toolkit supports caching of select Microsoft Graph API calls.</span></span> <span data-ttu-id="4a2b3-105">呼叫按实体（如人员、联系人、照片）进行缓存。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-105">Calls are being cached per entity, such as people, contact, photo.</span></span> <span data-ttu-id="4a2b3-106">这允许一个组件检索数据和其他组件以重复使用它，而无需调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-106">This allows one component to retrieve the data and other components to reuse it without calling Microsoft Graph.</span></span>

> [!TIP]
> <span data-ttu-id="4a2b3-107">有关每个组件缓存哪些实体的信息，请参阅组件的文档。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-107">For more information about which entities are cached by each component, see the component's documentation.</span></span>

<span data-ttu-id="4a2b3-108">由 mgt 创建的用于缓存的数据库的前缀为 `mgt-` 。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-108">Databases created by mgt for caching are prefixed with `mgt-`.</span></span> <span data-ttu-id="4a2b3-109">每个实体的数据都存储在单独的对象存储中。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-109">The data for each entity is stored in a separate object store.</span></span> <span data-ttu-id="4a2b3-110">若要检查缓存，请使用开发人员面板中的"应用程序"选项卡 (F12 工具) - 在"存储"部分下，单击 **"IndexedDB"** 选项卡。 </span><span class="sxs-lookup"><span data-stu-id="4a2b3-110">To inspect the cache, use the **Application** tab in the developer panel (F12 tools) - under the **Storage** section, click on the **IndexedDB** tab.</span></span> 

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a><span data-ttu-id="4a2b3-112">缓存配置</span><span class="sxs-lookup"><span data-stu-id="4a2b3-112">Cache configuration</span></span>

<span data-ttu-id="4a2b3-113">可以通过静态类对象读取和写入缓存 `CacheService.config` 选项。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-113">You can read and write the cache options through the static class `CacheService.config` object.</span></span> <span data-ttu-id="4a2b3-114">它的格式如下所示。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-114">It is formatted as shown.</span></span>

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
  response: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  files: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  fileLists: {
    invalidationPeriod: number,
    isEnabled: boolean
  }
};
```

<span data-ttu-id="4a2b3-115">在 config 对象中，单个缓存无效时段默认为 ，默认为 60 分钟内的常规值 `null` `defaultInvalidationPeriod` 3，600，000 ms (60 分钟) 。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-115">Individual cache invalidation periods are defaulted to `null` in the config object, and default to the general `defaultInvalidationPeriod` value of 3,600,000 ms (60 minutes).</span></span> <span data-ttu-id="4a2b3-116">传入的任何值 `config.x.invalidationPeriod` 都将替代 `defaultInvalidationPeriod` 。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-116">Any value passed into `config.x.invalidationPeriod` will override `defaultInvalidationPeriod`.</span></span>

<span data-ttu-id="4a2b3-117">状态存储是唯一的例外，其默认值为 300000 毫秒（即 5 分钟）。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-117">The presence store is the only exception, and has a default value of 300000 ms, or 5 minutes.</span></span>

### <a name="examples"></a><span data-ttu-id="4a2b3-118">示例</span><span class="sxs-lookup"><span data-stu-id="4a2b3-118">Examples</span></span>

<span data-ttu-id="4a2b3-119">若要单独禁用存储，只需将存储的 config 属性的值设置为 `isEnabled` false：</span><span class="sxs-lookup"><span data-stu-id="4a2b3-119">To individual disable a store simply set the value of `isEnabled` in that store's config properties to false:</span></span>
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
<span data-ttu-id="4a2b3-120">禁用缓存不会 **清除** 缓存。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-120">Disabling the cache does **not** clear the cache.</span></span>

<span data-ttu-id="4a2b3-121">更改失效期类似：</span><span class="sxs-lookup"><span data-stu-id="4a2b3-121">Changing the invalidation period is similar:</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a><span data-ttu-id="4a2b3-122">清除缓存</span><span class="sxs-lookup"><span data-stu-id="4a2b3-122">Clearing the cache</span></span>

<span data-ttu-id="4a2b3-123">当用户退出时，将自动清除缓存。也可以手动清除它。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-123">The cache is automatically cleared when the user signs out. It can also be cleared manually.</span></span>

<span data-ttu-id="4a2b3-124">如果清除缓存中所有的存储，类的 方法将清除 CacheService 维护的所有 `clearCaches()` `CacheService` 存储。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-124">The clear all the stores in the cache, the `clearCaches()` method of the `CacheService` class will clear every store maintained by the CacheService.</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a><span data-ttu-id="4a2b3-125">创建自己的缓存存储</span><span class="sxs-lookup"><span data-stu-id="4a2b3-125">Creating your own cache stores</span></span>

<span data-ttu-id="4a2b3-126">如果要为自定义组件创建和填充自己的缓存存储，可以使用静态 `CacheService` 类。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-126">If you want to create and populate your own cache stores for your custom components, you can use the `CacheService` static class.</span></span>

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> <span data-ttu-id="4a2b3-127">**注意：** 调用 `storeName` 中引用的 必须与 `getCache()` 对象中列出的存储之一 `CacheSchema` 匹配。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-127">**Note:** The `storeName` you reference in the call to `getCache()` must match one of the stores listed in your `CacheSchema` object.</span></span>

<span data-ttu-id="4a2b3-128">对象 `CacheSchema` 是键/值对的字典。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-128">The `CacheSchema` object is a dictionary with the key/value pairs.</span></span>

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

<span data-ttu-id="4a2b3-129">以下示例演示缓存实现。</span><span class="sxs-lookup"><span data-stu-id="4a2b3-129">The following example shows the cache implementation.</span></span>

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
