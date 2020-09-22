---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2fee186f7398c361e6ef02c56ecca299796bd4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030183"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="bd07e-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd07e-103">managedAppStatus resource type</span></span>

<span data-ttu-id="bd07e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd07e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd07e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd07e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd07e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd07e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd07e-107">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="bd07e-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="bd07e-108">方法</span><span class="sxs-lookup"><span data-stu-id="bd07e-108">Methods</span></span>
|<span data-ttu-id="bd07e-109">方法</span><span class="sxs-lookup"><span data-stu-id="bd07e-109">Method</span></span>|<span data-ttu-id="bd07e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bd07e-110">Return Type</span></span>|<span data-ttu-id="bd07e-111">说明</span><span class="sxs-lookup"><span data-stu-id="bd07e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd07e-112">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="bd07e-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="bd07e-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bd07e-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="bd07e-114">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd07e-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="bd07e-115">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="bd07e-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="bd07e-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="bd07e-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="bd07e-117">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd07e-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd07e-118">属性</span><span class="sxs-lookup"><span data-stu-id="bd07e-118">Properties</span></span>
|<span data-ttu-id="bd07e-119">属性</span><span class="sxs-lookup"><span data-stu-id="bd07e-119">Property</span></span>|<span data-ttu-id="bd07e-120">类型</span><span class="sxs-lookup"><span data-stu-id="bd07e-120">Type</span></span>|<span data-ttu-id="bd07e-121">说明</span><span class="sxs-lookup"><span data-stu-id="bd07e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd07e-122">displayName</span><span class="sxs-lookup"><span data-stu-id="bd07e-122">displayName</span></span>|<span data-ttu-id="bd07e-123">String</span><span class="sxs-lookup"><span data-stu-id="bd07e-123">String</span></span>|<span data-ttu-id="bd07e-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="bd07e-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="bd07e-125">id</span><span class="sxs-lookup"><span data-stu-id="bd07e-125">id</span></span>|<span data-ttu-id="bd07e-126">String</span><span class="sxs-lookup"><span data-stu-id="bd07e-126">String</span></span>|<span data-ttu-id="bd07e-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd07e-127">Key of the entity.</span></span>|
|<span data-ttu-id="bd07e-128">version</span><span class="sxs-lookup"><span data-stu-id="bd07e-128">version</span></span>|<span data-ttu-id="bd07e-129">String</span><span class="sxs-lookup"><span data-stu-id="bd07e-129">String</span></span>|<span data-ttu-id="bd07e-130">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="bd07e-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd07e-131">关系</span><span class="sxs-lookup"><span data-stu-id="bd07e-131">Relationships</span></span>
<span data-ttu-id="bd07e-132">无</span><span class="sxs-lookup"><span data-stu-id="bd07e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd07e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd07e-133">JSON Representation</span></span>
<span data-ttu-id="bd07e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd07e-134">Here is a JSON representation of the resource.</span></span>
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






