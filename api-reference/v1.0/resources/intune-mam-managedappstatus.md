---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca78f4dd9a191819e7f5e74ecea491ce7ceb7ec2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354287"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="53e87-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="53e87-103">managedAppStatus resource type</span></span>

<span data-ttu-id="53e87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53e87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53e87-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53e87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e87-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="53e87-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="53e87-107">方法</span><span class="sxs-lookup"><span data-stu-id="53e87-107">Methods</span></span>
|<span data-ttu-id="53e87-108">方法</span><span class="sxs-lookup"><span data-stu-id="53e87-108">Method</span></span>|<span data-ttu-id="53e87-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="53e87-109">Return Type</span></span>|<span data-ttu-id="53e87-110">说明</span><span class="sxs-lookup"><span data-stu-id="53e87-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53e87-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="53e87-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="53e87-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53e87-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="53e87-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53e87-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="53e87-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="53e87-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="53e87-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="53e87-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="53e87-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53e87-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53e87-117">属性</span><span class="sxs-lookup"><span data-stu-id="53e87-117">Properties</span></span>
|<span data-ttu-id="53e87-118">属性</span><span class="sxs-lookup"><span data-stu-id="53e87-118">Property</span></span>|<span data-ttu-id="53e87-119">类型</span><span class="sxs-lookup"><span data-stu-id="53e87-119">Type</span></span>|<span data-ttu-id="53e87-120">说明</span><span class="sxs-lookup"><span data-stu-id="53e87-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e87-121">displayName</span><span class="sxs-lookup"><span data-stu-id="53e87-121">displayName</span></span>|<span data-ttu-id="53e87-122">String</span><span class="sxs-lookup"><span data-stu-id="53e87-122">String</span></span>|<span data-ttu-id="53e87-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="53e87-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="53e87-124">id</span><span class="sxs-lookup"><span data-stu-id="53e87-124">id</span></span>|<span data-ttu-id="53e87-125">String</span><span class="sxs-lookup"><span data-stu-id="53e87-125">String</span></span>|<span data-ttu-id="53e87-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53e87-126">Key of the entity.</span></span>|
|<span data-ttu-id="53e87-127">version</span><span class="sxs-lookup"><span data-stu-id="53e87-127">version</span></span>|<span data-ttu-id="53e87-128">String</span><span class="sxs-lookup"><span data-stu-id="53e87-128">String</span></span>|<span data-ttu-id="53e87-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="53e87-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e87-130">关系</span><span class="sxs-lookup"><span data-stu-id="53e87-130">Relationships</span></span>
<span data-ttu-id="53e87-131">无</span><span class="sxs-lookup"><span data-stu-id="53e87-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e87-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53e87-132">JSON Representation</span></span>
<span data-ttu-id="53e87-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e87-133">Here is a JSON representation of the resource.</span></span>
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







