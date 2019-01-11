---
title: provisionedPlan 资源类型
description: 用户 实体和 组织 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837252"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="f90ce-103">provisionedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="f90ce-103">provisionedPlan resource type</span></span>

> <span data-ttu-id="f90ce-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f90ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f90ce-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f90ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f90ce-106">[用户](user.md) 实体和 [组织](organization.md) 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="f90ce-106">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="f90ce-107">属性</span><span class="sxs-lookup"><span data-stu-id="f90ce-107">Properties</span></span>
| <span data-ttu-id="f90ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="f90ce-108">Property</span></span>     | <span data-ttu-id="f90ce-109">类型</span><span class="sxs-lookup"><span data-stu-id="f90ce-109">Type</span></span>   |<span data-ttu-id="f90ce-110">说明</span><span class="sxs-lookup"><span data-stu-id="f90ce-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f90ce-111">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f90ce-111">capabilityStatus</span></span>|<span data-ttu-id="f90ce-112">String</span><span class="sxs-lookup"><span data-stu-id="f90ce-112">String</span></span>|<span data-ttu-id="f90ce-113">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="f90ce-113">For example, “Enabled”.</span></span>|
|<span data-ttu-id="f90ce-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="f90ce-114">provisioningStatus</span></span>|<span data-ttu-id="f90ce-115">String</span><span class="sxs-lookup"><span data-stu-id="f90ce-115">String</span></span>|<span data-ttu-id="f90ce-116">例如，“Success”。</span><span class="sxs-lookup"><span data-stu-id="f90ce-116">For example, “Success”.</span></span>|
|<span data-ttu-id="f90ce-117">service</span><span class="sxs-lookup"><span data-stu-id="f90ce-117">service</span></span>|<span data-ttu-id="f90ce-118">String</span><span class="sxs-lookup"><span data-stu-id="f90ce-118">String</span></span>|<span data-ttu-id="f90ce-119">服务名称；例如，“AccessControlS2S”</span><span class="sxs-lookup"><span data-stu-id="f90ce-119">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f90ce-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f90ce-120">JSON representation</span></span>

<span data-ttu-id="f90ce-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f90ce-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
