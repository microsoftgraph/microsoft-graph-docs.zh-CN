---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 178bc51d6293947f425dd3580a0bc9f9af208f7c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367026"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="f3e86-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3e86-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="f3e86-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3e86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3e86-105">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="f3e86-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f3e86-106">方法</span><span class="sxs-lookup"><span data-stu-id="f3e86-106">Methods</span></span>
|<span data-ttu-id="f3e86-107">方法</span><span class="sxs-lookup"><span data-stu-id="f3e86-107">Method</span></span>|<span data-ttu-id="f3e86-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f3e86-108">Return Type</span></span>|<span data-ttu-id="f3e86-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3e86-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3e86-110">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="f3e86-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="f3e86-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f3e86-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="f3e86-112">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f3e86-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="f3e86-113">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f3e86-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="f3e86-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="f3e86-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="f3e86-115">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f3e86-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3e86-116">属性</span><span class="sxs-lookup"><span data-stu-id="f3e86-116">Properties</span></span>
|<span data-ttu-id="f3e86-117">属性</span><span class="sxs-lookup"><span data-stu-id="f3e86-117">Property</span></span>|<span data-ttu-id="f3e86-118">类型</span><span class="sxs-lookup"><span data-stu-id="f3e86-118">Type</span></span>|<span data-ttu-id="f3e86-119">说明</span><span class="sxs-lookup"><span data-stu-id="f3e86-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3e86-120">displayName</span><span class="sxs-lookup"><span data-stu-id="f3e86-120">displayName</span></span>|<span data-ttu-id="f3e86-121">String</span><span class="sxs-lookup"><span data-stu-id="f3e86-121">String</span></span>|<span data-ttu-id="f3e86-122">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f3e86-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="f3e86-123">id</span><span class="sxs-lookup"><span data-stu-id="f3e86-123">id</span></span>|<span data-ttu-id="f3e86-124">String</span><span class="sxs-lookup"><span data-stu-id="f3e86-124">String</span></span>|<span data-ttu-id="f3e86-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f3e86-125">Key of the entity.</span></span>|
|<span data-ttu-id="f3e86-126">version</span><span class="sxs-lookup"><span data-stu-id="f3e86-126">version</span></span>|<span data-ttu-id="f3e86-127">String</span><span class="sxs-lookup"><span data-stu-id="f3e86-127">String</span></span>|<span data-ttu-id="f3e86-128">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f3e86-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3e86-129">关系</span><span class="sxs-lookup"><span data-stu-id="f3e86-129">Relationships</span></span>
<span data-ttu-id="f3e86-130">无</span><span class="sxs-lookup"><span data-stu-id="f3e86-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3e86-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3e86-131">JSON Representation</span></span>
<span data-ttu-id="f3e86-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3e86-132">Here is a JSON representation of the resource.</span></span>
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




