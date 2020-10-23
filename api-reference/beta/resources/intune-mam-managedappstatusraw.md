---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 039a3f49c877a9c54d11a88351fa6e5fd6c349d4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702346"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="5faa4-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="5faa4-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="5faa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5faa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5faa4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5faa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5faa4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5faa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5faa4-107">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="5faa4-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="5faa4-108">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5faa4-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5faa4-109">Methods</span><span class="sxs-lookup"><span data-stu-id="5faa4-109">Methods</span></span>
|<span data-ttu-id="5faa4-110">方法</span><span class="sxs-lookup"><span data-stu-id="5faa4-110">Method</span></span>|<span data-ttu-id="5faa4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5faa4-111">Return Type</span></span>|<span data-ttu-id="5faa4-112">说明</span><span class="sxs-lookup"><span data-stu-id="5faa4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5faa4-113">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="5faa4-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="5faa4-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5faa4-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="5faa4-115">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5faa4-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="5faa4-116">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5faa4-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="5faa4-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5faa4-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="5faa4-118">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5faa4-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5faa4-119">属性</span><span class="sxs-lookup"><span data-stu-id="5faa4-119">Properties</span></span>
|<span data-ttu-id="5faa4-120">属性</span><span class="sxs-lookup"><span data-stu-id="5faa4-120">Property</span></span>|<span data-ttu-id="5faa4-121">类型</span><span class="sxs-lookup"><span data-stu-id="5faa4-121">Type</span></span>|<span data-ttu-id="5faa4-122">说明</span><span class="sxs-lookup"><span data-stu-id="5faa4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5faa4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="5faa4-123">displayName</span></span>|<span data-ttu-id="5faa4-124">String</span><span class="sxs-lookup"><span data-stu-id="5faa4-124">String</span></span>|<span data-ttu-id="5faa4-125">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5faa4-125">Friendly name of the status report.</span></span> <span data-ttu-id="5faa4-126">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5faa4-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5faa4-127">id</span><span class="sxs-lookup"><span data-stu-id="5faa4-127">id</span></span>|<span data-ttu-id="5faa4-128">String</span><span class="sxs-lookup"><span data-stu-id="5faa4-128">String</span></span>|<span data-ttu-id="5faa4-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5faa4-129">Key of the entity.</span></span> <span data-ttu-id="5faa4-130">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5faa4-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5faa4-131">version</span><span class="sxs-lookup"><span data-stu-id="5faa4-131">version</span></span>|<span data-ttu-id="5faa4-132">String</span><span class="sxs-lookup"><span data-stu-id="5faa4-132">String</span></span>|<span data-ttu-id="5faa4-133">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5faa4-133">Version of the entity.</span></span> <span data-ttu-id="5faa4-134">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5faa4-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5faa4-135">content</span><span class="sxs-lookup"><span data-stu-id="5faa4-135">content</span></span>|[<span data-ttu-id="5faa4-136">Json</span><span class="sxs-lookup"><span data-stu-id="5faa4-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="5faa4-137">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="5faa4-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5faa4-138">关系</span><span class="sxs-lookup"><span data-stu-id="5faa4-138">Relationships</span></span>
<span data-ttu-id="5faa4-139">无</span><span class="sxs-lookup"><span data-stu-id="5faa4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5faa4-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5faa4-140">JSON Representation</span></span>
<span data-ttu-id="5faa4-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5faa4-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```





