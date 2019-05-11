---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccfb4aad51d8c0436f6cb8446775c93551d5c99a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940692"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="9333a-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9333a-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="9333a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9333a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9333a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9333a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9333a-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="9333a-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="9333a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9333a-107">Methods</span></span>
|<span data-ttu-id="9333a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9333a-108">Method</span></span>|<span data-ttu-id="9333a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9333a-109">Return Type</span></span>|<span data-ttu-id="9333a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9333a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9333a-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="9333a-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="9333a-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9333a-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="9333a-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9333a-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="9333a-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="9333a-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="9333a-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="9333a-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="9333a-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9333a-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9333a-117">属性</span><span class="sxs-lookup"><span data-stu-id="9333a-117">Properties</span></span>
|<span data-ttu-id="9333a-118">属性</span><span class="sxs-lookup"><span data-stu-id="9333a-118">Property</span></span>|<span data-ttu-id="9333a-119">类型</span><span class="sxs-lookup"><span data-stu-id="9333a-119">Type</span></span>|<span data-ttu-id="9333a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9333a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9333a-121">displayName</span><span class="sxs-lookup"><span data-stu-id="9333a-121">displayName</span></span>|<span data-ttu-id="9333a-122">String</span><span class="sxs-lookup"><span data-stu-id="9333a-122">String</span></span>|<span data-ttu-id="9333a-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="9333a-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="9333a-124">id</span><span class="sxs-lookup"><span data-stu-id="9333a-124">id</span></span>|<span data-ttu-id="9333a-125">String</span><span class="sxs-lookup"><span data-stu-id="9333a-125">String</span></span>|<span data-ttu-id="9333a-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9333a-126">Key of the entity.</span></span>|
|<span data-ttu-id="9333a-127">version</span><span class="sxs-lookup"><span data-stu-id="9333a-127">version</span></span>|<span data-ttu-id="9333a-128">String</span><span class="sxs-lookup"><span data-stu-id="9333a-128">String</span></span>|<span data-ttu-id="9333a-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9333a-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9333a-130">关系</span><span class="sxs-lookup"><span data-stu-id="9333a-130">Relationships</span></span>
<span data-ttu-id="9333a-131">无</span><span class="sxs-lookup"><span data-stu-id="9333a-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9333a-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9333a-132">JSON Representation</span></span>
<span data-ttu-id="9333a-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9333a-133">Here is a JSON representation of the resource.</span></span>
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




