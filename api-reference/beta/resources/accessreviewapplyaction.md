---
title: accessReviewApplyAction 资源类型
description: 表示访问评审实例完成后对已审阅用户要执行的操作。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7360c2a3a058eb4f884cb786c05a83efe09a6193
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133537"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="eba3f-103">accessReviewApplyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="eba3f-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="eba3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba3f-105">表示在 [accessReviewScheduleDefinition 的 accessReviewScheduleSettings](accessreviewschedulesettings.md) 中应用操作 [的基本类](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="eba3f-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="eba3f-106">支持的派生类型：</span><span class="sxs-lookup"><span data-stu-id="eba3f-106">Supported derived types:</span></span>

- <span data-ttu-id="eba3f-107">**removeAccessApplyAction** 是 accessReviewApplyAction 的派生类型，指示在完成审阅后删除正在审阅的实体的访问权限。</span><span class="sxs-lookup"><span data-stu-id="eba3f-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="eba3f-108">这是 accessReviewScheduleSettings 中的 applyActions 属性的默认类型，不需要指定。</span><span class="sxs-lookup"><span data-stu-id="eba3f-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="eba3f-109">**disableAndDeleteUserApplyAction** 是 accessReviewApplyAction 的派生类型，指示在完成审阅后禁用和删除正在审阅的用户。</span><span class="sxs-lookup"><span data-stu-id="eba3f-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="eba3f-110">这是非默认类型，需要在 accessReviewScheduleSettings 中指定。</span><span class="sxs-lookup"><span data-stu-id="eba3f-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="eba3f-111">属性</span><span class="sxs-lookup"><span data-stu-id="eba3f-111">Properties</span></span>
<span data-ttu-id="eba3f-112">无。</span><span class="sxs-lookup"><span data-stu-id="eba3f-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="eba3f-113">关系</span><span class="sxs-lookup"><span data-stu-id="eba3f-113">Relationships</span></span>
<span data-ttu-id="eba3f-114">无。</span><span class="sxs-lookup"><span data-stu-id="eba3f-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="eba3f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eba3f-115">JSON representation</span></span>
<span data-ttu-id="eba3f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eba3f-116">The following is a JSON representation of the resource.</span></span>
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
