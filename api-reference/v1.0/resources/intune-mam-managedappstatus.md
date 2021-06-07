---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 034a7961cedb5fe6e73ce4ac04774e6c64596428
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751655"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="2d674-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d674-103">managedAppStatus resource type</span></span>

<span data-ttu-id="2d674-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d674-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d674-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d674-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d674-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="2d674-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="2d674-107">Methods</span><span class="sxs-lookup"><span data-stu-id="2d674-107">Methods</span></span>
|<span data-ttu-id="2d674-108">方法</span><span class="sxs-lookup"><span data-stu-id="2d674-108">Method</span></span>|<span data-ttu-id="2d674-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d674-109">Return Type</span></span>|<span data-ttu-id="2d674-110">Description</span><span class="sxs-lookup"><span data-stu-id="2d674-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d674-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="2d674-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="2d674-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d674-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="2d674-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d674-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="2d674-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="2d674-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="2d674-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="2d674-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="2d674-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d674-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d674-117">属性</span><span class="sxs-lookup"><span data-stu-id="2d674-117">Properties</span></span>
|<span data-ttu-id="2d674-118">属性</span><span class="sxs-lookup"><span data-stu-id="2d674-118">Property</span></span>|<span data-ttu-id="2d674-119">类型</span><span class="sxs-lookup"><span data-stu-id="2d674-119">Type</span></span>|<span data-ttu-id="2d674-120">说明</span><span class="sxs-lookup"><span data-stu-id="2d674-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d674-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2d674-121">displayName</span></span>|<span data-ttu-id="2d674-122">String</span><span class="sxs-lookup"><span data-stu-id="2d674-122">String</span></span>|<span data-ttu-id="2d674-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2d674-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="2d674-124">id</span><span class="sxs-lookup"><span data-stu-id="2d674-124">id</span></span>|<span data-ttu-id="2d674-125">String</span><span class="sxs-lookup"><span data-stu-id="2d674-125">String</span></span>|<span data-ttu-id="2d674-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2d674-126">Key of the entity.</span></span>|
|<span data-ttu-id="2d674-127">version</span><span class="sxs-lookup"><span data-stu-id="2d674-127">version</span></span>|<span data-ttu-id="2d674-128">String</span><span class="sxs-lookup"><span data-stu-id="2d674-128">String</span></span>|<span data-ttu-id="2d674-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2d674-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d674-130">关系</span><span class="sxs-lookup"><span data-stu-id="2d674-130">Relationships</span></span>
<span data-ttu-id="2d674-131">无</span><span class="sxs-lookup"><span data-stu-id="2d674-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d674-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d674-132">JSON Representation</span></span>
<span data-ttu-id="2d674-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d674-133">Here is a JSON representation of the resource.</span></span>
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




