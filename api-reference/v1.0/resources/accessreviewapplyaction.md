---
title: accessReviewApplyAction 资源类型
description: 表示访问评审实例完成后对被审阅用户要执行的操作。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4a96ed1009a8af4404c50041258e784d8bd04030
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031034"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="c6fcf-103">accessReviewApplyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6fcf-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="c6fcf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6fcf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6fcf-105">表示在 [accessReviewScheduleDefinition 的 accessReviewScheduleSettings](accessreviewschedulesettings.md) 中应用操作 [的基本类](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="c6fcf-106">支持的派生类型：</span><span class="sxs-lookup"><span data-stu-id="c6fcf-106">Supported derived types:</span></span>

- <span data-ttu-id="c6fcf-107">[removeAccessApplyAction](removeaccessapplyaction.md) 是 accessReviewApplyAction 的派生类型，指示在完成审阅后删除正在审阅的实体的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-107">[removeAccessApplyAction](removeaccessapplyaction.md) is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="c6fcf-108">这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，不需要指定。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="c6fcf-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) 是 accessReviewApplyAction 的派生类型，指示在完成审阅后禁用和删除正在审阅的用户。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="c6fcf-110">这是非默认类型，需要在 accessReviewScheduleSettings 中指定。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="c6fcf-111">属性</span><span class="sxs-lookup"><span data-stu-id="c6fcf-111">Properties</span></span>
<span data-ttu-id="c6fcf-112">无。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="c6fcf-113">关系</span><span class="sxs-lookup"><span data-stu-id="c6fcf-113">Relationships</span></span>
<span data-ttu-id="c6fcf-114">无。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6fcf-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6fcf-115">JSON representation</span></span>
<span data-ttu-id="c6fcf-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6fcf-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

