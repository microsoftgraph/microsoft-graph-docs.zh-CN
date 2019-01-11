---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6a4f15266ebfda3e2af43a5d39e28803fe9d87b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837371"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="f73d8-103">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f73d8-103">outlookUser resource type</span></span>


<span data-ttu-id="f73d8-104">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="f73d8-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="f73d8-105">方法</span><span class="sxs-lookup"><span data-stu-id="f73d8-105">Methods</span></span>

| <span data-ttu-id="f73d8-106">方法</span><span class="sxs-lookup"><span data-stu-id="f73d8-106">Method</span></span>           | <span data-ttu-id="f73d8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f73d8-107">Return Type</span></span>    |<span data-ttu-id="f73d8-108">说明</span><span class="sxs-lookup"><span data-stu-id="f73d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f73d8-109">Create category</span><span class="sxs-lookup"><span data-stu-id="f73d8-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="f73d8-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="f73d8-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="f73d8-111">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="f73d8-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="f73d8-112">List categories</span><span class="sxs-lookup"><span data-stu-id="f73d8-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="f73d8-113">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f73d8-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="f73d8-114">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="f73d8-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="f73d8-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="f73d8-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="f73d8-116">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f73d8-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="f73d8-117">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="f73d8-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="f73d8-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="f73d8-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="f73d8-119">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f73d8-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="f73d8-120">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="f73d8-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="f73d8-121">属性</span><span class="sxs-lookup"><span data-stu-id="f73d8-121">Properties</span></span>
<span data-ttu-id="f73d8-122">无</span><span class="sxs-lookup"><span data-stu-id="f73d8-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f73d8-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="f73d8-123">Relationships</span></span>
| <span data-ttu-id="f73d8-124">关系</span><span class="sxs-lookup"><span data-stu-id="f73d8-124">Relationship</span></span> | <span data-ttu-id="f73d8-125">类型</span><span class="sxs-lookup"><span data-stu-id="f73d8-125">Type</span></span>   |<span data-ttu-id="f73d8-126">说明</span><span class="sxs-lookup"><span data-stu-id="f73d8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f73d8-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="f73d8-127">masterCategories</span></span>|<span data-ttu-id="f73d8-128">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f73d8-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="f73d8-129">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="f73d8-129">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
