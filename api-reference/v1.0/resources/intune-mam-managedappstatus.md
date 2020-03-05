---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: deaca18dd8a11c930bdd052a6e3c1f94f0de1a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448324"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="6563e-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="6563e-103">managedAppStatus resource type</span></span>

<span data-ttu-id="6563e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6563e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6563e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6563e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6563e-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="6563e-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="6563e-107">方法</span><span class="sxs-lookup"><span data-stu-id="6563e-107">Methods</span></span>
|<span data-ttu-id="6563e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6563e-108">Method</span></span>|<span data-ttu-id="6563e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6563e-109">Return Type</span></span>|<span data-ttu-id="6563e-110">说明</span><span class="sxs-lookup"><span data-stu-id="6563e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6563e-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="6563e-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="6563e-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6563e-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="6563e-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6563e-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="6563e-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6563e-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="6563e-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6563e-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="6563e-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6563e-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6563e-117">属性</span><span class="sxs-lookup"><span data-stu-id="6563e-117">Properties</span></span>
|<span data-ttu-id="6563e-118">属性</span><span class="sxs-lookup"><span data-stu-id="6563e-118">Property</span></span>|<span data-ttu-id="6563e-119">类型</span><span class="sxs-lookup"><span data-stu-id="6563e-119">Type</span></span>|<span data-ttu-id="6563e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6563e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6563e-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6563e-121">displayName</span></span>|<span data-ttu-id="6563e-122">String</span><span class="sxs-lookup"><span data-stu-id="6563e-122">String</span></span>|<span data-ttu-id="6563e-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6563e-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="6563e-124">id</span><span class="sxs-lookup"><span data-stu-id="6563e-124">id</span></span>|<span data-ttu-id="6563e-125">String</span><span class="sxs-lookup"><span data-stu-id="6563e-125">String</span></span>|<span data-ttu-id="6563e-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6563e-126">Key of the entity.</span></span>|
|<span data-ttu-id="6563e-127">version</span><span class="sxs-lookup"><span data-stu-id="6563e-127">version</span></span>|<span data-ttu-id="6563e-128">String</span><span class="sxs-lookup"><span data-stu-id="6563e-128">String</span></span>|<span data-ttu-id="6563e-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6563e-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6563e-130">关系</span><span class="sxs-lookup"><span data-stu-id="6563e-130">Relationships</span></span>
<span data-ttu-id="6563e-131">无</span><span class="sxs-lookup"><span data-stu-id="6563e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6563e-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6563e-132">JSON Representation</span></span>
<span data-ttu-id="6563e-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6563e-133">Here is a JSON representation of the resource.</span></span>
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




