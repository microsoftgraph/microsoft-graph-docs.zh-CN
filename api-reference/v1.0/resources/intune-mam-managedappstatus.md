---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f8d41d1768f843ea5d2c6e4c61256cdfbc1d629
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988231"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="17e37-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="17e37-103">managedAppStatus resource type</span></span>

<span data-ttu-id="17e37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17e37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17e37-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17e37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17e37-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="17e37-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="17e37-107">方法</span><span class="sxs-lookup"><span data-stu-id="17e37-107">Methods</span></span>
|<span data-ttu-id="17e37-108">方法</span><span class="sxs-lookup"><span data-stu-id="17e37-108">Method</span></span>|<span data-ttu-id="17e37-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="17e37-109">Return Type</span></span>|<span data-ttu-id="17e37-110">说明</span><span class="sxs-lookup"><span data-stu-id="17e37-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17e37-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="17e37-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="17e37-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17e37-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="17e37-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17e37-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="17e37-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="17e37-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="17e37-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="17e37-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="17e37-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17e37-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17e37-117">属性</span><span class="sxs-lookup"><span data-stu-id="17e37-117">Properties</span></span>
|<span data-ttu-id="17e37-118">属性</span><span class="sxs-lookup"><span data-stu-id="17e37-118">Property</span></span>|<span data-ttu-id="17e37-119">类型</span><span class="sxs-lookup"><span data-stu-id="17e37-119">Type</span></span>|<span data-ttu-id="17e37-120">说明</span><span class="sxs-lookup"><span data-stu-id="17e37-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17e37-121">displayName</span><span class="sxs-lookup"><span data-stu-id="17e37-121">displayName</span></span>|<span data-ttu-id="17e37-122">String</span><span class="sxs-lookup"><span data-stu-id="17e37-122">String</span></span>|<span data-ttu-id="17e37-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="17e37-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="17e37-124">id</span><span class="sxs-lookup"><span data-stu-id="17e37-124">id</span></span>|<span data-ttu-id="17e37-125">String</span><span class="sxs-lookup"><span data-stu-id="17e37-125">String</span></span>|<span data-ttu-id="17e37-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="17e37-126">Key of the entity.</span></span>|
|<span data-ttu-id="17e37-127">version</span><span class="sxs-lookup"><span data-stu-id="17e37-127">version</span></span>|<span data-ttu-id="17e37-128">String</span><span class="sxs-lookup"><span data-stu-id="17e37-128">String</span></span>|<span data-ttu-id="17e37-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="17e37-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17e37-130">关系</span><span class="sxs-lookup"><span data-stu-id="17e37-130">Relationships</span></span>
<span data-ttu-id="17e37-131">无</span><span class="sxs-lookup"><span data-stu-id="17e37-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17e37-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17e37-132">JSON Representation</span></span>
<span data-ttu-id="17e37-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17e37-133">Here is a JSON representation of the resource.</span></span>
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









