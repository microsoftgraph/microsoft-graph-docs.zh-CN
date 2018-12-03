---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 '
ms.openlocfilehash: 51799e01e5ab48fc5e686d72d2bdb5c85f191e1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042562"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="0870f-104">educationSynchronizationCustomization 资源类型</span><span class="sxs-lookup"><span data-stu-id="0870f-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="0870f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0870f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0870f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0870f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0870f-107">提供用于自定义资源实体学校数据配置文件同步设置。</span><span class="sxs-lookup"><span data-stu-id="0870f-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="0870f-108">自定义项可以应用于正在同步的所有实体。</span><span class="sxs-lookup"><span data-stu-id="0870f-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="0870f-109">**注意：\*\*\*\*SynchronizationStartDate**属性仅适用于**StudentEnrollment**实体。</span><span class="sxs-lookup"><span data-stu-id="0870f-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="0870f-110">属性</span><span class="sxs-lookup"><span data-stu-id="0870f-110">Properties</span></span>

| <span data-ttu-id="0870f-111">属性</span><span class="sxs-lookup"><span data-stu-id="0870f-111">Property</span></span> | <span data-ttu-id="0870f-112">类型</span><span class="sxs-lookup"><span data-stu-id="0870f-112">Type</span></span> | <span data-ttu-id="0870f-113">Description</span><span class="sxs-lookup"><span data-stu-id="0870f-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0870f-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="0870f-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="0870f-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0870f-115">collection of string</span></span> |  <span data-ttu-id="0870f-116">要同步的属性名称的集合。如果设置为 null，所有属性将都为同步。</span><span class="sxs-lookup"><span data-stu-id="0870f-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="0870f-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="0870f-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="0870f-118">DateTime</span><span class="sxs-lookup"><span data-stu-id="0870f-118">DateTime</span></span> |  <span data-ttu-id="0870f-119">同步的开始日期。</span><span class="sxs-lookup"><span data-stu-id="0870f-119">The date that the synchronization should start.</span></span> <span data-ttu-id="0870f-120">此值应设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="0870f-120">This value should be set to a future date.</span></span> <span data-ttu-id="0870f-121">如果配置文件安装完成后，将会同步设置为 null，资源。</span><span class="sxs-lookup"><span data-stu-id="0870f-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="0870f-122">**注意：** 这仅适用于**StudentEnrollment**属性。</span><span class="sxs-lookup"><span data-stu-id="0870f-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="0870f-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="0870f-123">**isSyncDeferred**</span></span> |<span data-ttu-id="0870f-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="0870f-124">Boolean</span></span> | <span data-ttu-id="0870f-125">指示是否对父实体的同步推迟到以后。</span><span class="sxs-lookup"><span data-stu-id="0870f-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="0870f-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="0870f-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="0870f-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="0870f-127">Boolean</span></span> |  <span data-ttu-id="0870f-128">指示是否可以通过同步来覆盖资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0870f-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="0870f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0870f-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
