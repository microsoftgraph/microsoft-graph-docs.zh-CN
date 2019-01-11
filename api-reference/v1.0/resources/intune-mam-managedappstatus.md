---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13bf28c0244a3288b949ebf718e3d5ce97ceb60c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890382"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="af08f-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="af08f-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="af08f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="af08f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af08f-105">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="af08f-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="af08f-106">方法</span><span class="sxs-lookup"><span data-stu-id="af08f-106">Methods</span></span>
|<span data-ttu-id="af08f-107">方法</span><span class="sxs-lookup"><span data-stu-id="af08f-107">Method</span></span>|<span data-ttu-id="af08f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="af08f-108">Return Type</span></span>|<span data-ttu-id="af08f-109">说明</span><span class="sxs-lookup"><span data-stu-id="af08f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af08f-110">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="af08f-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="af08f-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af08f-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="af08f-112">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af08f-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="af08f-113">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="af08f-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="af08f-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="af08f-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="af08f-115">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af08f-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af08f-116">属性</span><span class="sxs-lookup"><span data-stu-id="af08f-116">Properties</span></span>
|<span data-ttu-id="af08f-117">属性</span><span class="sxs-lookup"><span data-stu-id="af08f-117">Property</span></span>|<span data-ttu-id="af08f-118">类型</span><span class="sxs-lookup"><span data-stu-id="af08f-118">Type</span></span>|<span data-ttu-id="af08f-119">说明</span><span class="sxs-lookup"><span data-stu-id="af08f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af08f-120">displayName</span><span class="sxs-lookup"><span data-stu-id="af08f-120">displayName</span></span>|<span data-ttu-id="af08f-121">String</span><span class="sxs-lookup"><span data-stu-id="af08f-121">String</span></span>|<span data-ttu-id="af08f-122">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="af08f-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="af08f-123">id</span><span class="sxs-lookup"><span data-stu-id="af08f-123">id</span></span>|<span data-ttu-id="af08f-124">String</span><span class="sxs-lookup"><span data-stu-id="af08f-124">String</span></span>|<span data-ttu-id="af08f-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af08f-125">Key of the entity.</span></span>|
|<span data-ttu-id="af08f-126">version</span><span class="sxs-lookup"><span data-stu-id="af08f-126">version</span></span>|<span data-ttu-id="af08f-127">String</span><span class="sxs-lookup"><span data-stu-id="af08f-127">String</span></span>|<span data-ttu-id="af08f-128">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="af08f-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af08f-129">关系</span><span class="sxs-lookup"><span data-stu-id="af08f-129">Relationships</span></span>
<span data-ttu-id="af08f-130">无</span><span class="sxs-lookup"><span data-stu-id="af08f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af08f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af08f-131">JSON Representation</span></span>
<span data-ttu-id="af08f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af08f-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



