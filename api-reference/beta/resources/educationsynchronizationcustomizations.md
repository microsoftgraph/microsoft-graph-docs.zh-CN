---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项（如果有）。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6df720b8f0e02ba24f3972833a6a76219d327925
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790927"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="7db7d-103">educationSynchronizationCustomizations 资源类型</span><span class="sxs-lookup"><span data-stu-id="7db7d-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="7db7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7db7d-105">包含要同步的实体的列表及其自定义项（如果有）。</span><span class="sxs-lookup"><span data-stu-id="7db7d-105">Contains the list of entities to sync and their customizations, if any.</span></span>

> [!NOTE]
> <span data-ttu-id="7db7d-106">要同步的属性的自定义不适用于学生注册或教师名册。</span><span class="sxs-lookup"><span data-stu-id="7db7d-106">Customization of properties to sync does not apply to the Student Enrollments or  Teacher Rosters.</span></span>

<span data-ttu-id="7db7d-107">此资源是以下数据提供程序的成员：</span><span class="sxs-lookup"><span data-stu-id="7db7d-107">This resource is member of the following data providers:</span></span>

- [<span data-ttu-id="7db7d-108">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="7db7d-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
- [<span data-ttu-id="7db7d-109">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="7db7d-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="7db7d-110">属性</span><span class="sxs-lookup"><span data-stu-id="7db7d-110">Properties</span></span>

| <span data-ttu-id="7db7d-111">属性</span><span class="sxs-lookup"><span data-stu-id="7db7d-111">Property</span></span>          | <span data-ttu-id="7db7d-112">类型</span><span class="sxs-lookup"><span data-stu-id="7db7d-112">Type</span></span>                                    | <span data-ttu-id="7db7d-113">说明</span><span class="sxs-lookup"><span data-stu-id="7db7d-113">Description</span></span>                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="7db7d-114">虽然</span><span class="sxs-lookup"><span data-stu-id="7db7d-114">school</span></span>            | <span data-ttu-id="7db7d-115">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-115">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-116">学校实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-116">Customizations for School entities.</span></span>     |
| <span data-ttu-id="7db7d-117">section</span><span class="sxs-lookup"><span data-stu-id="7db7d-117">section</span></span>           | <span data-ttu-id="7db7d-118">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-118">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-119">节实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-119">Customizations for Section entities.</span></span>    |
| <span data-ttu-id="7db7d-120">student</span><span class="sxs-lookup"><span data-stu-id="7db7d-120">student</span></span>           | <span data-ttu-id="7db7d-121">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-121">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-122">学生实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-122">Customizations for Student entities.</span></span>    |
| <span data-ttu-id="7db7d-123">teacher</span><span class="sxs-lookup"><span data-stu-id="7db7d-123">teacher</span></span>           | <span data-ttu-id="7db7d-124">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-124">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-125">教师实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-125">Customizations for Teacher entities.</span></span>    |
| <span data-ttu-id="7db7d-126">studentEnrollment</span><span class="sxs-lookup"><span data-stu-id="7db7d-126">studentEnrollment</span></span> | <span data-ttu-id="7db7d-127">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-127">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-128">学生登记的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-128">Customizations for Student Enrollments.</span></span> |
| <span data-ttu-id="7db7d-129">teacherRoster</span><span class="sxs-lookup"><span data-stu-id="7db7d-129">teacherRoster</span></span>     | <span data-ttu-id="7db7d-130">[educationSynchronizationCustomization]</span><span class="sxs-lookup"><span data-stu-id="7db7d-130">[educationSynchronizationCustomization]</span></span> | <span data-ttu-id="7db7d-131">教师名册的自定义项。</span><span class="sxs-lookup"><span data-stu-id="7db7d-131">Customizations for Teacher Rosters.</span></span>     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a><span data-ttu-id="7db7d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7db7d-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```
