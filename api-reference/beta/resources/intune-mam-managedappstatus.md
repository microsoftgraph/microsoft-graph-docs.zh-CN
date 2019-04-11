---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6df9c36f15e3e20389dfc46d306b896c3fe77b5b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799144"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="dcc8a-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcc8a-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="dcc8a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcc8a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcc8a-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="dcc8a-107">方法</span><span class="sxs-lookup"><span data-stu-id="dcc8a-107">Methods</span></span>
|<span data-ttu-id="dcc8a-108">方法</span><span class="sxs-lookup"><span data-stu-id="dcc8a-108">Method</span></span>|<span data-ttu-id="dcc8a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="dcc8a-109">Return Type</span></span>|<span data-ttu-id="dcc8a-110">说明</span><span class="sxs-lookup"><span data-stu-id="dcc8a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dcc8a-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="dcc8a-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="dcc8a-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dcc8a-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="dcc8a-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="dcc8a-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dcc8a-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="dcc8a-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dcc8a-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="dcc8a-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dcc8a-117">属性</span><span class="sxs-lookup"><span data-stu-id="dcc8a-117">Properties</span></span>
|<span data-ttu-id="dcc8a-118">属性</span><span class="sxs-lookup"><span data-stu-id="dcc8a-118">Property</span></span>|<span data-ttu-id="dcc8a-119">类型</span><span class="sxs-lookup"><span data-stu-id="dcc8a-119">Type</span></span>|<span data-ttu-id="dcc8a-120">说明</span><span class="sxs-lookup"><span data-stu-id="dcc8a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcc8a-121">displayName</span><span class="sxs-lookup"><span data-stu-id="dcc8a-121">displayName</span></span>|<span data-ttu-id="dcc8a-122">String</span><span class="sxs-lookup"><span data-stu-id="dcc8a-122">String</span></span>|<span data-ttu-id="dcc8a-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="dcc8a-124">id</span><span class="sxs-lookup"><span data-stu-id="dcc8a-124">id</span></span>|<span data-ttu-id="dcc8a-125">String</span><span class="sxs-lookup"><span data-stu-id="dcc8a-125">String</span></span>|<span data-ttu-id="dcc8a-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-126">Key of the entity.</span></span>|
|<span data-ttu-id="dcc8a-127">version</span><span class="sxs-lookup"><span data-stu-id="dcc8a-127">version</span></span>|<span data-ttu-id="dcc8a-128">String</span><span class="sxs-lookup"><span data-stu-id="dcc8a-128">String</span></span>|<span data-ttu-id="dcc8a-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcc8a-130">关系</span><span class="sxs-lookup"><span data-stu-id="dcc8a-130">Relationships</span></span>
<span data-ttu-id="dcc8a-131">无</span><span class="sxs-lookup"><span data-stu-id="dcc8a-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcc8a-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcc8a-132">JSON Representation</span></span>
<span data-ttu-id="dcc8a-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcc8a-133">Here is a JSON representation of the resource.</span></span>
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





