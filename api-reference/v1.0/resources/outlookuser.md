---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 27d7e91223a763720cdb70d6b857f91c0955b5ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447253"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="e5fd6-103">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5fd6-103">outlookUser resource type</span></span>

<span data-ttu-id="e5fd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e5fd6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="e5fd6-105">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="e5fd6-106">方法</span><span class="sxs-lookup"><span data-stu-id="e5fd6-106">Methods</span></span>

| <span data-ttu-id="e5fd6-107">方法</span><span class="sxs-lookup"><span data-stu-id="e5fd6-107">Method</span></span>           | <span data-ttu-id="e5fd6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5fd6-108">Return Type</span></span>    |<span data-ttu-id="e5fd6-109">说明</span><span class="sxs-lookup"><span data-stu-id="e5fd6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5fd6-110">Create category</span><span class="sxs-lookup"><span data-stu-id="e5fd6-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="e5fd6-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="e5fd6-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="e5fd6-112">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="e5fd6-113">List categories</span><span class="sxs-lookup"><span data-stu-id="e5fd6-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="e5fd6-114">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5fd6-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="e5fd6-115">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="e5fd6-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="e5fd6-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="e5fd6-117">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5fd6-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="e5fd6-118">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="e5fd6-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="e5fd6-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="e5fd6-120">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5fd6-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="e5fd6-121">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="e5fd6-122">属性</span><span class="sxs-lookup"><span data-stu-id="e5fd6-122">Properties</span></span>
<span data-ttu-id="e5fd6-123">无</span><span class="sxs-lookup"><span data-stu-id="e5fd6-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e5fd6-124">关系</span><span class="sxs-lookup"><span data-stu-id="e5fd6-124">Relationships</span></span>
| <span data-ttu-id="e5fd6-125">关系</span><span class="sxs-lookup"><span data-stu-id="e5fd6-125">Relationship</span></span> | <span data-ttu-id="e5fd6-126">类型</span><span class="sxs-lookup"><span data-stu-id="e5fd6-126">Type</span></span>   |<span data-ttu-id="e5fd6-127">说明</span><span class="sxs-lookup"><span data-stu-id="e5fd6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5fd6-128">masterCategories</span><span class="sxs-lookup"><span data-stu-id="e5fd6-128">masterCategories</span></span>|<span data-ttu-id="e5fd6-129">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5fd6-129">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="e5fd6-130">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="e5fd6-130">A list of categories defined for the user.</span></span> | 

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
