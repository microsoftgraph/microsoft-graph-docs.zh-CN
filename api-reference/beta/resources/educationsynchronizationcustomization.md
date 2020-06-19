---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体的学校数据配置文件同步的设置。 自定义项可应用于要同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4aab80a23b72b599df7627f5734d04ad9aef0bbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790934"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="f2c57-104">educationSynchronizationCustomization 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2c57-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="f2c57-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c57-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c57-106">提供用于自定义资源实体的学校数据配置文件同步的设置。</span><span class="sxs-lookup"><span data-stu-id="f2c57-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="f2c57-107">自定义项可应用于要同步的所有实体。</span><span class="sxs-lookup"><span data-stu-id="f2c57-107">The customization can be applied to all the entities being synchronized.</span></span>

## <a name="properties"></a><span data-ttu-id="f2c57-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2c57-108">Properties</span></span>

| <span data-ttu-id="f2c57-109">属性</span><span class="sxs-lookup"><span data-stu-id="f2c57-109">Property</span></span>                 | <span data-ttu-id="f2c57-110">类型</span><span class="sxs-lookup"><span data-stu-id="f2c57-110">Type</span></span>              | <span data-ttu-id="f2c57-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2c57-111">Description</span></span>                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f2c57-112">optionalPropertiesToSync</span><span class="sxs-lookup"><span data-stu-id="f2c57-112">optionalPropertiesToSync</span></span> | <span data-ttu-id="f2c57-113">String collection</span><span class="sxs-lookup"><span data-stu-id="f2c57-113">String collection</span></span> | <span data-ttu-id="f2c57-114">要同步的属性名称的集合。如果设置为 null，则将同步所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2c57-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span> <span data-ttu-id="f2c57-115">**不适用于学生注册或教师名册**</span><span class="sxs-lookup"><span data-stu-id="f2c57-115">**Does not apply to Student Enrollments or Teacher Rosters**</span></span>                                                            |
| <span data-ttu-id="f2c57-116">synchronizationStartDate</span><span class="sxs-lookup"><span data-stu-id="f2c57-116">synchronizationStartDate</span></span> | <span data-ttu-id="f2c57-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="f2c57-117">DateTime</span></span>          | <span data-ttu-id="f2c57-118">同步应开始的日期。</span><span class="sxs-lookup"><span data-stu-id="f2c57-118">The date that the synchronization should start.</span></span> <span data-ttu-id="f2c57-119">此值应设置为将来日期。</span><span class="sxs-lookup"><span data-stu-id="f2c57-119">This value should be set to a future date.</span></span> <span data-ttu-id="f2c57-120">如果设置为 null，则在配置文件设置完成时将同步资源。</span><span class="sxs-lookup"><span data-stu-id="f2c57-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="f2c57-121">**仅适用于学生注册**</span><span class="sxs-lookup"><span data-stu-id="f2c57-121">**Only applies to Student Enrollments**</span></span> |
| <span data-ttu-id="f2c57-122">isSyncDeferred</span><span class="sxs-lookup"><span data-stu-id="f2c57-122">isSyncDeferred</span></span>           | <span data-ttu-id="f2c57-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="f2c57-123">Boolean</span></span>           | <span data-ttu-id="f2c57-124">指示是否将父实体的同步延迟到更高的日期。</span><span class="sxs-lookup"><span data-stu-id="f2c57-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span>                                                                                                                                    |
| <span data-ttu-id="f2c57-125">allowDisplayNameUpdate</span><span class="sxs-lookup"><span data-stu-id="f2c57-125">allowDisplayNameUpdate</span></span>   | <span data-ttu-id="f2c57-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="f2c57-126">Boolean</span></span>           | <span data-ttu-id="f2c57-127">指示是否可由同步覆盖资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f2c57-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="f2c57-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2c57-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```
