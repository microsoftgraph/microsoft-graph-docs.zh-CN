---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258861"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="5da13-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="5da13-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="5da13-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5da13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5da13-105">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="5da13-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="5da13-106">方法</span><span class="sxs-lookup"><span data-stu-id="5da13-106">Methods</span></span>
|<span data-ttu-id="5da13-107">方法</span><span class="sxs-lookup"><span data-stu-id="5da13-107">Method</span></span>|<span data-ttu-id="5da13-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5da13-108">Return Type</span></span>|<span data-ttu-id="5da13-109">说明</span><span class="sxs-lookup"><span data-stu-id="5da13-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5da13-110">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="5da13-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="5da13-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5da13-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="5da13-112">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5da13-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="5da13-113">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5da13-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="5da13-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5da13-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="5da13-115">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5da13-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5da13-116">属性</span><span class="sxs-lookup"><span data-stu-id="5da13-116">Properties</span></span>
|<span data-ttu-id="5da13-117">属性</span><span class="sxs-lookup"><span data-stu-id="5da13-117">Property</span></span>|<span data-ttu-id="5da13-118">类型</span><span class="sxs-lookup"><span data-stu-id="5da13-118">Type</span></span>|<span data-ttu-id="5da13-119">说明</span><span class="sxs-lookup"><span data-stu-id="5da13-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5da13-120">displayName</span><span class="sxs-lookup"><span data-stu-id="5da13-120">displayName</span></span>|<span data-ttu-id="5da13-121">String</span><span class="sxs-lookup"><span data-stu-id="5da13-121">String</span></span>|<span data-ttu-id="5da13-122">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5da13-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="5da13-123">id</span><span class="sxs-lookup"><span data-stu-id="5da13-123">id</span></span>|<span data-ttu-id="5da13-124">字符串</span><span class="sxs-lookup"><span data-stu-id="5da13-124">String</span></span>|<span data-ttu-id="5da13-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5da13-125">Key of the entity.</span></span>|
|<span data-ttu-id="5da13-126">version</span><span class="sxs-lookup"><span data-stu-id="5da13-126">version</span></span>|<span data-ttu-id="5da13-127">String</span><span class="sxs-lookup"><span data-stu-id="5da13-127">String</span></span>|<span data-ttu-id="5da13-128">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5da13-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5da13-129">关系</span><span class="sxs-lookup"><span data-stu-id="5da13-129">Relationships</span></span>
<span data-ttu-id="5da13-130">无</span><span class="sxs-lookup"><span data-stu-id="5da13-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5da13-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5da13-131">JSON Representation</span></span>
<span data-ttu-id="5da13-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5da13-132">Here is a JSON representation of the resource.</span></span>
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



