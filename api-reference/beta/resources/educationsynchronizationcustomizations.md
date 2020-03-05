---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项（如果有）。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2ff93d6a91d522c5d1140035e278e9832332321
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500448"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="8c747-103">educationSynchronizationCustomizations 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c747-103">educationSynchronizationCustomizations resource type</span></span>

<span data-ttu-id="8c747-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8c747-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c747-105">包含要同步的实体的列表及其[自定义项](educationsynchronizationcustomization.md)（如果有）。</span><span class="sxs-lookup"><span data-stu-id="8c747-105">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="8c747-106">**注意：** 要同步的属性的自定义不应用于**studentEnrollment**和**teacherRoster**实体。</span><span class="sxs-lookup"><span data-stu-id="8c747-106">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="8c747-107">此资源是以下数据提供程序的成员：</span><span class="sxs-lookup"><span data-stu-id="8c747-107">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="8c747-108">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="8c747-108">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="8c747-109">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="8c747-109">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="8c747-110">属性</span><span class="sxs-lookup"><span data-stu-id="8c747-110">Properties</span></span>

| <span data-ttu-id="8c747-111">属性</span><span class="sxs-lookup"><span data-stu-id="8c747-111">Property</span></span> | <span data-ttu-id="8c747-112">类型</span><span class="sxs-lookup"><span data-stu-id="8c747-112">Type</span></span> | <span data-ttu-id="8c747-113">说明</span><span class="sxs-lookup"><span data-stu-id="8c747-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8c747-114">**虽然**</span><span class="sxs-lookup"><span data-stu-id="8c747-114">**school**</span></span> | [<span data-ttu-id="8c747-115">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-115">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="8c747-116">自定义的学校实体。</span><span class="sxs-lookup"><span data-stu-id="8c747-116">Customization for a school entity.</span></span>        |
| <span data-ttu-id="8c747-117">**section**</span><span class="sxs-lookup"><span data-stu-id="8c747-117">**section**</span></span> | [<span data-ttu-id="8c747-118">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-118">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="8c747-119">节实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="8c747-119">Customization for a section entity.</span></span>         |
| <span data-ttu-id="8c747-120">**student**</span><span class="sxs-lookup"><span data-stu-id="8c747-120">**student**</span></span> | [<span data-ttu-id="8c747-121">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-121">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="8c747-122">学生实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="8c747-122">Customization for a student entity.</span></span>         |
| <span data-ttu-id="8c747-123">**teacher**</span><span class="sxs-lookup"><span data-stu-id="8c747-123">**teacher**</span></span> | [<span data-ttu-id="8c747-124">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-124">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="8c747-125">为教师实体自定义。</span><span class="sxs-lookup"><span data-stu-id="8c747-125">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="8c747-126">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="8c747-126">**studentEnrollment**</span></span> | [<span data-ttu-id="8c747-127">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-127">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="8c747-128">学生注册的自定义。</span><span class="sxs-lookup"><span data-stu-id="8c747-128">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="8c747-129">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="8c747-129">**teacherRoster**</span></span> | [<span data-ttu-id="8c747-130">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="8c747-130">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="8c747-131">教师名单的自定义。</span><span class="sxs-lookup"><span data-stu-id="8c747-131">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8c747-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c747-132">JSON representation</span></span>
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
