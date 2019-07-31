---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项 (如果有)。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d31be9bd808f411c1e208ab953784fdefd65fdda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972437"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="0df4e-103">educationSynchronizationCustomizations 资源类型</span><span class="sxs-lookup"><span data-stu-id="0df4e-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df4e-104">包含要同步的实体的列表及其[自定义项](educationsynchronizationcustomization.md)(如果有)。</span><span class="sxs-lookup"><span data-stu-id="0df4e-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="0df4e-105">**注意:** 要同步的属性的自定义不应用于**studentEnrollment**和**teacherRoster**实体。</span><span class="sxs-lookup"><span data-stu-id="0df4e-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="0df4e-106">此资源是以下数据提供程序的成员:</span><span class="sxs-lookup"><span data-stu-id="0df4e-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="0df4e-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="0df4e-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="0df4e-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="0df4e-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="0df4e-109">属性</span><span class="sxs-lookup"><span data-stu-id="0df4e-109">Properties</span></span>

| <span data-ttu-id="0df4e-110">属性</span><span class="sxs-lookup"><span data-stu-id="0df4e-110">Property</span></span> | <span data-ttu-id="0df4e-111">类型</span><span class="sxs-lookup"><span data-stu-id="0df4e-111">Type</span></span> | <span data-ttu-id="0df4e-112">说明</span><span class="sxs-lookup"><span data-stu-id="0df4e-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0df4e-113">**虽然**</span><span class="sxs-lookup"><span data-stu-id="0df4e-113">**school**</span></span> | [<span data-ttu-id="0df4e-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="0df4e-115">自定义的学校实体。</span><span class="sxs-lookup"><span data-stu-id="0df4e-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="0df4e-116">**section**</span><span class="sxs-lookup"><span data-stu-id="0df4e-116">**section**</span></span> | [<span data-ttu-id="0df4e-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="0df4e-118">节实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="0df4e-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="0df4e-119">**student**</span><span class="sxs-lookup"><span data-stu-id="0df4e-119">**student**</span></span> | [<span data-ttu-id="0df4e-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="0df4e-121">学生实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="0df4e-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="0df4e-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="0df4e-122">**teacher**</span></span> | [<span data-ttu-id="0df4e-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="0df4e-124">为教师实体自定义。</span><span class="sxs-lookup"><span data-stu-id="0df4e-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="0df4e-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="0df4e-125">**studentEnrollment**</span></span> | [<span data-ttu-id="0df4e-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="0df4e-127">学生注册的自定义。</span><span class="sxs-lookup"><span data-stu-id="0df4e-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="0df4e-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="0df4e-128">**teacherRoster**</span></span> | [<span data-ttu-id="0df4e-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="0df4e-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="0df4e-130">教师名单的自定义。</span><span class="sxs-lookup"><span data-stu-id="0df4e-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0df4e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0df4e-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
