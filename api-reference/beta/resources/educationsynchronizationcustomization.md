---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513604"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="7e10c-104">educationSynchronizationCustomization 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e10c-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e10c-105">提供用于自定义资源实体学校数据配置文件同步设置。</span><span class="sxs-lookup"><span data-stu-id="7e10c-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="7e10c-106">自定义项可以应用于正在同步的所有实体。</span><span class="sxs-lookup"><span data-stu-id="7e10c-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="7e10c-107">**注意：\*\*\*\*SynchronizationStartDate**属性仅适用于**StudentEnrollment**实体。</span><span class="sxs-lookup"><span data-stu-id="7e10c-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="7e10c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e10c-108">Properties</span></span>

| <span data-ttu-id="7e10c-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e10c-109">Property</span></span> | <span data-ttu-id="7e10c-110">类型</span><span class="sxs-lookup"><span data-stu-id="7e10c-110">Type</span></span> | <span data-ttu-id="7e10c-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e10c-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7e10c-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="7e10c-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="7e10c-113">Collection of String</span><span class="sxs-lookup"><span data-stu-id="7e10c-113">collection of string</span></span> |  <span data-ttu-id="7e10c-114">要同步的属性名称的集合。如果设置为 null，所有属性将都为同步。</span><span class="sxs-lookup"><span data-stu-id="7e10c-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="7e10c-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="7e10c-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="7e10c-116">日期/时间</span><span class="sxs-lookup"><span data-stu-id="7e10c-116">DateTime</span></span> |  <span data-ttu-id="7e10c-117">同步的开始日期。</span><span class="sxs-lookup"><span data-stu-id="7e10c-117">The date that the synchronization should start.</span></span> <span data-ttu-id="7e10c-118">此值应设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="7e10c-118">This value should be set to a future date.</span></span> <span data-ttu-id="7e10c-119">如果配置文件安装完成后，将会同步设置为 null，资源。</span><span class="sxs-lookup"><span data-stu-id="7e10c-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="7e10c-120">**注意：** 这仅适用于**StudentEnrollment**属性。</span><span class="sxs-lookup"><span data-stu-id="7e10c-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="7e10c-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="7e10c-121">**isSyncDeferred**</span></span> |<span data-ttu-id="7e10c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e10c-122">Boolean</span></span> | <span data-ttu-id="7e10c-123">指示是否对父实体的同步推迟到以后。</span><span class="sxs-lookup"><span data-stu-id="7e10c-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="7e10c-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="7e10c-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="7e10c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e10c-125">Boolean</span></span> |  <span data-ttu-id="7e10c-126">指示是否可以通过同步来覆盖资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e10c-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="7e10c-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e10c-127">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
