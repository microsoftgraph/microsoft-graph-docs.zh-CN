---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 980521b7f58338501d69ec83a6fc68b591c8688c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967905"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="012d1-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="012d1-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="012d1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="012d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="012d1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="012d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="012d1-106">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="012d1-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="012d1-107">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="012d1-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="012d1-108">方法</span><span class="sxs-lookup"><span data-stu-id="012d1-108">Methods</span></span>
|<span data-ttu-id="012d1-109">方法</span><span class="sxs-lookup"><span data-stu-id="012d1-109">Method</span></span>|<span data-ttu-id="012d1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="012d1-110">Return Type</span></span>|<span data-ttu-id="012d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="012d1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="012d1-112">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="012d1-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="012d1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="012d1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="012d1-114">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="012d1-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="012d1-115">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="012d1-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="012d1-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="012d1-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="012d1-117">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="012d1-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="012d1-118">属性</span><span class="sxs-lookup"><span data-stu-id="012d1-118">Properties</span></span>
|<span data-ttu-id="012d1-119">属性</span><span class="sxs-lookup"><span data-stu-id="012d1-119">Property</span></span>|<span data-ttu-id="012d1-120">类型</span><span class="sxs-lookup"><span data-stu-id="012d1-120">Type</span></span>|<span data-ttu-id="012d1-121">说明</span><span class="sxs-lookup"><span data-stu-id="012d1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="012d1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="012d1-122">displayName</span></span>|<span data-ttu-id="012d1-123">String</span><span class="sxs-lookup"><span data-stu-id="012d1-123">String</span></span>|<span data-ttu-id="012d1-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="012d1-124">Friendly name of the status report.</span></span> <span data-ttu-id="012d1-125">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="012d1-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="012d1-126">id</span><span class="sxs-lookup"><span data-stu-id="012d1-126">id</span></span>|<span data-ttu-id="012d1-127">String</span><span class="sxs-lookup"><span data-stu-id="012d1-127">String</span></span>|<span data-ttu-id="012d1-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="012d1-128">Key of the entity.</span></span> <span data-ttu-id="012d1-129">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="012d1-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="012d1-130">version</span><span class="sxs-lookup"><span data-stu-id="012d1-130">version</span></span>|<span data-ttu-id="012d1-131">String</span><span class="sxs-lookup"><span data-stu-id="012d1-131">String</span></span>|<span data-ttu-id="012d1-132">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="012d1-132">Version of the entity.</span></span> <span data-ttu-id="012d1-133">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="012d1-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="012d1-134">content</span><span class="sxs-lookup"><span data-stu-id="012d1-134">content</span></span>|[<span data-ttu-id="012d1-135">Json</span><span class="sxs-lookup"><span data-stu-id="012d1-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="012d1-136">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="012d1-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="012d1-137">关系</span><span class="sxs-lookup"><span data-stu-id="012d1-137">Relationships</span></span>
<span data-ttu-id="012d1-138">无</span><span class="sxs-lookup"><span data-stu-id="012d1-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="012d1-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="012d1-139">JSON Representation</span></span>
<span data-ttu-id="012d1-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="012d1-140">Here is a JSON representation of the resource.</span></span>
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





