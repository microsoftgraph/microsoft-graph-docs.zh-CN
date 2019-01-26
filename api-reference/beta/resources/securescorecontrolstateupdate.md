---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含控件状态更新的用户的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574388"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="3d059-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d059-103">secureScoreControlStateUpdate resource type</span></span>

> <span data-ttu-id="3d059-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3d059-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d059-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d059-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d059-106">包含由用户更新控件状态的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。</span><span class="sxs-lookup"><span data-stu-id="3d059-106">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="3d059-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d059-107">Property</span></span>         | <span data-ttu-id="3d059-108">类型</span><span class="sxs-lookup"><span data-stu-id="3d059-108">Type</span></span>           |<span data-ttu-id="3d059-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d059-109">Description</span></span>                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| <span data-ttu-id="3d059-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3d059-110">assignedTo</span></span>      | <span data-ttu-id="3d059-111">string</span><span class="sxs-lookup"><span data-stu-id="3d059-111">string</span></span>         | <span data-ttu-id="3d059-112">分配将执行的操作的用户控件</span><span class="sxs-lookup"><span data-stu-id="3d059-112">Assign the control to the user who will take the action</span></span>     |
| <span data-ttu-id="3d059-113">批注</span><span class="sxs-lookup"><span data-stu-id="3d059-113">comment</span></span>         | <span data-ttu-id="3d059-114">string</span><span class="sxs-lookup"><span data-stu-id="3d059-114">string</span></span>         | <span data-ttu-id="3d059-115">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="3d059-115">Provides optional comment about the control</span></span>                 |
| <span data-ttu-id="3d059-116">state</span><span class="sxs-lookup"><span data-stu-id="3d059-116">state</span></span>           | <span data-ttu-id="3d059-117">string</span><span class="sxs-lookup"><span data-stu-id="3d059-117">string</span></span>         | <span data-ttu-id="3d059-118">可以使用修补程序命令修改控件的状态 (例如： 忽略，第三方等)</span><span class="sxs-lookup"><span data-stu-id="3d059-118">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
| <span data-ttu-id="3d059-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="3d059-119">updatedBy</span></span>       | <span data-ttu-id="3d059-120">string</span><span class="sxs-lookup"><span data-stu-id="3d059-120">string</span></span>         |<span data-ttu-id="3d059-121">更新租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="3d059-121">ID of the user who updated tenant state</span></span>                      |
| <span data-ttu-id="3d059-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d059-122">updatedDateTime</span></span> | <span data-ttu-id="3d059-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d059-123">DateTimeOffset</span></span> |<span data-ttu-id="3d059-124">在哪个控件更新状态的时间</span><span class="sxs-lookup"><span data-stu-id="3d059-124">Time at which control state was updated</span></span>                      |
 

## <a name="json-representation"></a><span data-ttu-id="3d059-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d059-125">JSON representation</span></span>
 <span data-ttu-id="3d059-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d059-126">The following is a JSON representation of the resource.</span></span>

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "DateTimeOffset"
}
```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
