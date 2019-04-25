---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项 (如果有)。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543197"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="f0ee2-103">educationSynchronizationCustomizations 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0ee2-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0ee2-104">包含要同步的实体的列表及其[自定义项](educationsynchronizationcustomization.md)(如果有)。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="f0ee2-105">**注意:** 要同步的属性的自定义不应用于**studentEnrollment**和**teacherRoster**实体。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="f0ee2-106">此资源是以下数据提供程序的成员:</span><span class="sxs-lookup"><span data-stu-id="f0ee2-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="f0ee2-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="f0ee2-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="f0ee2-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="f0ee2-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="f0ee2-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0ee2-109">Properties</span></span>

| <span data-ttu-id="f0ee2-110">属性</span><span class="sxs-lookup"><span data-stu-id="f0ee2-110">Property</span></span> | <span data-ttu-id="f0ee2-111">类型</span><span class="sxs-lookup"><span data-stu-id="f0ee2-111">Type</span></span> | <span data-ttu-id="f0ee2-112">说明</span><span class="sxs-lookup"><span data-stu-id="f0ee2-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f0ee2-113">**虽然**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-113">**school**</span></span> | [<span data-ttu-id="f0ee2-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f0ee2-115">自定义的学校实体。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="f0ee2-116">**section**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-116">**section**</span></span> | [<span data-ttu-id="f0ee2-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f0ee2-118">节实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="f0ee2-119">**student**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-119">**student**</span></span> | [<span data-ttu-id="f0ee2-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f0ee2-121">学生实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="f0ee2-122">**teacher**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-122">**teacher**</span></span> | [<span data-ttu-id="f0ee2-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f0ee2-124">为教师实体自定义。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="f0ee2-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-125">**studentEnrollment**</span></span> | [<span data-ttu-id="f0ee2-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="f0ee2-127">学生注册的自定义。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="f0ee2-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="f0ee2-128">**teacherRoster**</span></span> | [<span data-ttu-id="f0ee2-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="f0ee2-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="f0ee2-130">教师名单的自定义。</span><span class="sxs-lookup"><span data-stu-id="f0ee2-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f0ee2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0ee2-131">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
