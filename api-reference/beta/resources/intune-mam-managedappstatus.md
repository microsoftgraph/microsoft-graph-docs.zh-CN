---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc9f6596e9d9361a8c211809bf0f621fe36bcd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153156"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="7589b-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="7589b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="7589b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7589b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7589b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7589b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7589b-106">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="7589b-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7589b-107">方法</span><span class="sxs-lookup"><span data-stu-id="7589b-107">Methods</span></span>
|<span data-ttu-id="7589b-108">方法</span><span class="sxs-lookup"><span data-stu-id="7589b-108">Method</span></span>|<span data-ttu-id="7589b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7589b-109">Return Type</span></span>|<span data-ttu-id="7589b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7589b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7589b-111">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="7589b-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="7589b-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7589b-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="7589b-113">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7589b-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="7589b-114">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7589b-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="7589b-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7589b-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="7589b-116">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7589b-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7589b-117">属性</span><span class="sxs-lookup"><span data-stu-id="7589b-117">Properties</span></span>
|<span data-ttu-id="7589b-118">属性</span><span class="sxs-lookup"><span data-stu-id="7589b-118">Property</span></span>|<span data-ttu-id="7589b-119">类型</span><span class="sxs-lookup"><span data-stu-id="7589b-119">Type</span></span>|<span data-ttu-id="7589b-120">说明</span><span class="sxs-lookup"><span data-stu-id="7589b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7589b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="7589b-121">displayName</span></span>|<span data-ttu-id="7589b-122">String</span><span class="sxs-lookup"><span data-stu-id="7589b-122">String</span></span>|<span data-ttu-id="7589b-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="7589b-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="7589b-124">id</span><span class="sxs-lookup"><span data-stu-id="7589b-124">id</span></span>|<span data-ttu-id="7589b-125">字符串</span><span class="sxs-lookup"><span data-stu-id="7589b-125">String</span></span>|<span data-ttu-id="7589b-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7589b-126">Key of the entity.</span></span>|
|<span data-ttu-id="7589b-127">version</span><span class="sxs-lookup"><span data-stu-id="7589b-127">version</span></span>|<span data-ttu-id="7589b-128">String</span><span class="sxs-lookup"><span data-stu-id="7589b-128">String</span></span>|<span data-ttu-id="7589b-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="7589b-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7589b-130">关系</span><span class="sxs-lookup"><span data-stu-id="7589b-130">Relationships</span></span>
<span data-ttu-id="7589b-131">无</span><span class="sxs-lookup"><span data-stu-id="7589b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7589b-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7589b-132">JSON Representation</span></span>
<span data-ttu-id="7589b-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7589b-133">Here is a JSON representation of the resource.</span></span>
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




