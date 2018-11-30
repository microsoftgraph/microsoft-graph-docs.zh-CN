---
title: educationSynchronizationCustomizations 资源类型
description: 如果有，包含与同步和其自定义的实体列表。
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045739"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="6fd1a-103">educationSynchronizationCustomizations 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="6fd1a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fd1a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6fd1a-106">如果有，包含同步和其[自定义项](educationsynchronizationcustomization.md)的实体列表。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="6fd1a-107">**注意：** 要同步的属性的自定义不适用于**studentEnrollment**和**teacherRoster**实体。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="6fd1a-108">此资源是以下数据提供程序的成员：</span><span class="sxs-lookup"><span data-stu-id="6fd1a-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="6fd1a-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="6fd1a-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="6fd1a-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="6fd1a-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="6fd1a-111">属性</span><span class="sxs-lookup"><span data-stu-id="6fd1a-111">Properties</span></span>

| <span data-ttu-id="6fd1a-112">属性</span><span class="sxs-lookup"><span data-stu-id="6fd1a-112">Property</span></span> | <span data-ttu-id="6fd1a-113">类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-113">Type</span></span> | <span data-ttu-id="6fd1a-114">说明</span><span class="sxs-lookup"><span data-stu-id="6fd1a-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6fd1a-115">**学校**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-115">**school**</span></span> | [<span data-ttu-id="6fd1a-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6fd1a-117">学校实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="6fd1a-118">**section**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-118">**section**</span></span> | [<span data-ttu-id="6fd1a-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6fd1a-120">针对部分实体的自定义项。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="6fd1a-121">**student**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-121">**student**</span></span> | [<span data-ttu-id="6fd1a-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6fd1a-123">学生实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="6fd1a-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-124">**teacher**</span></span> | [<span data-ttu-id="6fd1a-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6fd1a-126">教师实体的自定义。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="6fd1a-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-127">**studentEnrollment**</span></span> | [<span data-ttu-id="6fd1a-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6fd1a-129">针对学生注册自定义项。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="6fd1a-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="6fd1a-130">**teacherRoster**</span></span> | [<span data-ttu-id="6fd1a-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6fd1a-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="6fd1a-132">针对教师名单的自定义项。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6fd1a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fd1a-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
