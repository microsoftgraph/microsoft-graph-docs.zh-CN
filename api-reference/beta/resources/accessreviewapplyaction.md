---
title: accessReviewApplyAction 资源类型
description: 表示在完成访问审核实例后要对审阅的用户执行的操作。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000832"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="19eb8-103">accessReviewApplyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="19eb8-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="19eb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19eb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19eb8-105">表示在[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的[accessReviewScheduleSettings](accessreviewschedulesettings.md)中应用操作的基类。</span><span class="sxs-lookup"><span data-stu-id="19eb8-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="19eb8-106">支持的派生类型：</span><span class="sxs-lookup"><span data-stu-id="19eb8-106">Supported derived types:</span></span>

- <span data-ttu-id="19eb8-107">**removeAccessApplyAction** 是 accessReviewApplyAction 的派生类型，它指示删除完成评审时审阅的实体的访问权限。</span><span class="sxs-lookup"><span data-stu-id="19eb8-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="19eb8-108">这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，无需指定。</span><span class="sxs-lookup"><span data-stu-id="19eb8-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="19eb8-109">**disableAndDeleteUserApplyAction** 是 accessReviewApplyAction 的派生类型，它指示在完成审阅时禁用和删除要审阅的用户。</span><span class="sxs-lookup"><span data-stu-id="19eb8-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="19eb8-110">这是非默认类型，需要在 accessReviewScheduleSettings 中指定。</span><span class="sxs-lookup"><span data-stu-id="19eb8-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="19eb8-111">属性</span><span class="sxs-lookup"><span data-stu-id="19eb8-111">Properties</span></span>
<span data-ttu-id="19eb8-112">无。</span><span class="sxs-lookup"><span data-stu-id="19eb8-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="19eb8-113">关系</span><span class="sxs-lookup"><span data-stu-id="19eb8-113">Relationships</span></span>
<span data-ttu-id="19eb8-114">无。</span><span class="sxs-lookup"><span data-stu-id="19eb8-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="19eb8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19eb8-115">JSON representation</span></span>
<span data-ttu-id="19eb8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19eb8-116">The following is a JSON representation of the resource.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
