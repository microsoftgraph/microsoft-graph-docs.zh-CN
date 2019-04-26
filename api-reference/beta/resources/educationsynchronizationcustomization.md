---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体的学校数据配置文件同步的设置。 自定义项可应用于要同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397f4d732bc25d086b2aeae6efc697d2048e6a03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334091"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="7a5fc-104">educationSynchronizationCustomization 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a5fc-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a5fc-105">提供用于自定义资源实体的学校数据配置文件同步的设置。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="7a5fc-106">自定义项可应用于要同步的所有实体。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="7a5fc-107">**注意:\*\*\*\*synchronizationStartDate**属性仅适用于**StudentEnrollment**实体。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="7a5fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a5fc-108">Properties</span></span>

| <span data-ttu-id="7a5fc-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a5fc-109">Property</span></span> | <span data-ttu-id="7a5fc-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a5fc-110">Type</span></span> | <span data-ttu-id="7a5fc-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a5fc-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7a5fc-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="7a5fc-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="7a5fc-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7a5fc-113">collection of string</span></span> |  <span data-ttu-id="7a5fc-114">要同步的属性名称的集合。如果设置为 null, 则将同步所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="7a5fc-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="7a5fc-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="7a5fc-116">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a5fc-116">DateTime</span></span> |  <span data-ttu-id="7a5fc-117">同步应开始的日期。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-117">The date that the synchronization should start.</span></span> <span data-ttu-id="7a5fc-118">此值应设置为将来日期。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-118">This value should be set to a future date.</span></span> <span data-ttu-id="7a5fc-119">如果设置为 null, 则在配置文件设置完成时将同步资源。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="7a5fc-120">**注意:** 这仅适用于**StudentEnrollment**属性。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="7a5fc-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="7a5fc-121">**isSyncDeferred**</span></span> |<span data-ttu-id="7a5fc-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5fc-122">Boolean</span></span> | <span data-ttu-id="7a5fc-123">指示是否将父实体的同步延迟到更高的日期。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="7a5fc-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="7a5fc-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="7a5fc-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5fc-125">Boolean</span></span> |  <span data-ttu-id="7a5fc-126">指示是否可由同步覆盖资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7a5fc-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="7a5fc-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a5fc-127">JSON representation</span></span>
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
