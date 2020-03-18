---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 292cd8c17702705774b650c257c4ae9ce1ff0ff3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781416"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="968dd-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="968dd-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="968dd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="968dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="968dd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="968dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="968dd-106">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="968dd-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="968dd-107">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="968dd-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="968dd-108">方法</span><span class="sxs-lookup"><span data-stu-id="968dd-108">Methods</span></span>
|<span data-ttu-id="968dd-109">方法</span><span class="sxs-lookup"><span data-stu-id="968dd-109">Method</span></span>|<span data-ttu-id="968dd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="968dd-110">Return Type</span></span>|<span data-ttu-id="968dd-111">说明</span><span class="sxs-lookup"><span data-stu-id="968dd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="968dd-112">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="968dd-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="968dd-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="968dd-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="968dd-114">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="968dd-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="968dd-115">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="968dd-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="968dd-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="968dd-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="968dd-117">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="968dd-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="968dd-118">属性</span><span class="sxs-lookup"><span data-stu-id="968dd-118">Properties</span></span>
|<span data-ttu-id="968dd-119">属性</span><span class="sxs-lookup"><span data-stu-id="968dd-119">Property</span></span>|<span data-ttu-id="968dd-120">类型</span><span class="sxs-lookup"><span data-stu-id="968dd-120">Type</span></span>|<span data-ttu-id="968dd-121">说明</span><span class="sxs-lookup"><span data-stu-id="968dd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="968dd-122">displayName</span><span class="sxs-lookup"><span data-stu-id="968dd-122">displayName</span></span>|<span data-ttu-id="968dd-123">String</span><span class="sxs-lookup"><span data-stu-id="968dd-123">String</span></span>|<span data-ttu-id="968dd-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="968dd-124">Friendly name of the status report.</span></span> <span data-ttu-id="968dd-125">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="968dd-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="968dd-126">id</span><span class="sxs-lookup"><span data-stu-id="968dd-126">id</span></span>|<span data-ttu-id="968dd-127">String</span><span class="sxs-lookup"><span data-stu-id="968dd-127">String</span></span>|<span data-ttu-id="968dd-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="968dd-128">Key of the entity.</span></span> <span data-ttu-id="968dd-129">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="968dd-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="968dd-130">version</span><span class="sxs-lookup"><span data-stu-id="968dd-130">version</span></span>|<span data-ttu-id="968dd-131">String</span><span class="sxs-lookup"><span data-stu-id="968dd-131">String</span></span>|<span data-ttu-id="968dd-132">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="968dd-132">Version of the entity.</span></span> <span data-ttu-id="968dd-133">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="968dd-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="968dd-134">content</span><span class="sxs-lookup"><span data-stu-id="968dd-134">content</span></span>|[<span data-ttu-id="968dd-135">Json</span><span class="sxs-lookup"><span data-stu-id="968dd-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="968dd-136">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="968dd-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="968dd-137">关系</span><span class="sxs-lookup"><span data-stu-id="968dd-137">Relationships</span></span>
<span data-ttu-id="968dd-138">无</span><span class="sxs-lookup"><span data-stu-id="968dd-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="968dd-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="968dd-139">JSON Representation</span></span>
<span data-ttu-id="968dd-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="968dd-140">Here is a JSON representation of the resource.</span></span>
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



