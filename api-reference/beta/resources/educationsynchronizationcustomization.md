---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体的学校数据配置文件同步的设置。 自定义项可应用于要同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 368117a5293f4ede59282fa1ced12d024976de52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500462"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="612e8-104">educationSynchronizationCustomization 资源类型</span><span class="sxs-lookup"><span data-stu-id="612e8-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="612e8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="612e8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="612e8-106">提供用于自定义资源实体的学校数据配置文件同步的设置。</span><span class="sxs-lookup"><span data-stu-id="612e8-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="612e8-107">自定义项可应用于要同步的所有实体。</span><span class="sxs-lookup"><span data-stu-id="612e8-107">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="612e8-108">**注意：\*\*\*\*SynchronizationStartDate**属性仅适用于**StudentEnrollment**实体。</span><span class="sxs-lookup"><span data-stu-id="612e8-108">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="612e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="612e8-109">Properties</span></span>

| <span data-ttu-id="612e8-110">属性</span><span class="sxs-lookup"><span data-stu-id="612e8-110">Property</span></span> | <span data-ttu-id="612e8-111">类型</span><span class="sxs-lookup"><span data-stu-id="612e8-111">Type</span></span> | <span data-ttu-id="612e8-112">说明</span><span class="sxs-lookup"><span data-stu-id="612e8-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="612e8-113">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="612e8-113">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="612e8-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="612e8-114">collection of string</span></span> |  <span data-ttu-id="612e8-115">要同步的属性名称的集合。如果设置为 null，则将同步所有属性。</span><span class="sxs-lookup"><span data-stu-id="612e8-115">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="612e8-116">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="612e8-116">**synchronizationStartDate**</span></span> | <span data-ttu-id="612e8-117">日期时间</span><span class="sxs-lookup"><span data-stu-id="612e8-117">DateTime</span></span> |  <span data-ttu-id="612e8-118">同步应开始的日期。</span><span class="sxs-lookup"><span data-stu-id="612e8-118">The date that the synchronization should start.</span></span> <span data-ttu-id="612e8-119">此值应设置为将来日期。</span><span class="sxs-lookup"><span data-stu-id="612e8-119">This value should be set to a future date.</span></span> <span data-ttu-id="612e8-120">如果设置为 null，则在配置文件设置完成时将同步资源。</span><span class="sxs-lookup"><span data-stu-id="612e8-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="612e8-121">**注意：** 这仅适用于**StudentEnrollment**属性。</span><span class="sxs-lookup"><span data-stu-id="612e8-121">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="612e8-122">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="612e8-122">**isSyncDeferred**</span></span> |<span data-ttu-id="612e8-123">布尔</span><span class="sxs-lookup"><span data-stu-id="612e8-123">Boolean</span></span> | <span data-ttu-id="612e8-124">指示是否将父实体的同步延迟到更高的日期。</span><span class="sxs-lookup"><span data-stu-id="612e8-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="612e8-125">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="612e8-125">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="612e8-126">布尔</span><span class="sxs-lookup"><span data-stu-id="612e8-126">Boolean</span></span> |  <span data-ttu-id="612e8-127">指示是否可由同步覆盖资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="612e8-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="612e8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="612e8-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
