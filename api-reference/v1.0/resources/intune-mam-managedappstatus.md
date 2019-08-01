---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eef17c260d868b05280a41f14e797c928c432002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037889"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="c1ec0-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1ec0-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="c1ec0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ec0-105">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="c1ec0-106">方法</span><span class="sxs-lookup"><span data-stu-id="c1ec0-106">Methods</span></span>
|<span data-ttu-id="c1ec0-107">方法</span><span class="sxs-lookup"><span data-stu-id="c1ec0-107">Method</span></span>|<span data-ttu-id="c1ec0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1ec0-108">Return Type</span></span>|<span data-ttu-id="c1ec0-109">说明</span><span class="sxs-lookup"><span data-stu-id="c1ec0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1ec0-110">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="c1ec0-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="c1ec0-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1ec0-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="c1ec0-112">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="c1ec0-113">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c1ec0-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="c1ec0-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c1ec0-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="c1ec0-115">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1ec0-116">属性</span><span class="sxs-lookup"><span data-stu-id="c1ec0-116">Properties</span></span>
|<span data-ttu-id="c1ec0-117">属性</span><span class="sxs-lookup"><span data-stu-id="c1ec0-117">Property</span></span>|<span data-ttu-id="c1ec0-118">类型</span><span class="sxs-lookup"><span data-stu-id="c1ec0-118">Type</span></span>|<span data-ttu-id="c1ec0-119">说明</span><span class="sxs-lookup"><span data-stu-id="c1ec0-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ec0-120">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ec0-120">displayName</span></span>|<span data-ttu-id="c1ec0-121">String</span><span class="sxs-lookup"><span data-stu-id="c1ec0-121">String</span></span>|<span data-ttu-id="c1ec0-122">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="c1ec0-123">id</span><span class="sxs-lookup"><span data-stu-id="c1ec0-123">id</span></span>|<span data-ttu-id="c1ec0-124">String</span><span class="sxs-lookup"><span data-stu-id="c1ec0-124">String</span></span>|<span data-ttu-id="c1ec0-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-125">Key of the entity.</span></span>|
|<span data-ttu-id="c1ec0-126">version</span><span class="sxs-lookup"><span data-stu-id="c1ec0-126">version</span></span>|<span data-ttu-id="c1ec0-127">String</span><span class="sxs-lookup"><span data-stu-id="c1ec0-127">String</span></span>|<span data-ttu-id="c1ec0-128">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1ec0-129">关系</span><span class="sxs-lookup"><span data-stu-id="c1ec0-129">Relationships</span></span>
<span data-ttu-id="c1ec0-130">无</span><span class="sxs-lookup"><span data-stu-id="c1ec0-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1ec0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1ec0-131">JSON Representation</span></span>
<span data-ttu-id="c1ec0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ec0-132">Here is a JSON representation of the resource.</span></span>
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



